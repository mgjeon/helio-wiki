---
title: JSOC SHARP Pipeline Structure and Algorithms
created: 2026-06-07
updated: 2026-06-07
type: query
tags: [solar-physics, space-weather, active-region, hmi, jsoc, magnetic-field, forecasting]
sources: [http://jsoc.stanford.edu/HMI/Vector_products.html, http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm, https://github.com/JSOC-SDP/proj, https://github.com/JSOC-SDP/workflow, https://github.com/mbobra/SHARPs]
confidence: high
---

# JSOC SHARP Pipeline Structure and Algorithms

This page records the Q&A synthesis of the current JSOC SHARP pipeline: how HMI observations become tracked Space-weather HMI Active Region Patches, disambiguated vector fields, CEA products, and space-weather keywords. Related pages: [[sharps]], [[proj]], [[workflow]], [[active-region-parameters]], [[solar-data-access]], [[coronal-magnetic-field-modeling]].

## One-line summary

The JSOC SHARP pipeline combines an HMI active-region tracking pipeline with the HMI vector magnetogram pipeline: HMI filtergrams are calibrated into Stokes parameters, LOS magnetograms and intensity images identify and track HARPs, VFISV inverts Stokes profiles inside the tracked regions, a minimum-energy method resolves the 180-degree azimuth ambiguity, and `sharp.c` packages native CCD and CEA-remapped products plus space-weather summary keywords. Source: http://jsoc.stanford.edu/HMI/Vector_products.html; Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm

## High-level data flow

```text
HMI filtergrams
  -> calibrated / registered Stokes I,Q,U,V 720s products
  -> LOS magnetogram + continuum/intensity products
  -> Marmask segmentation
  -> HARP detection, tracking, and DRMS ingestion
  -> VFISV Milne-Eddington inversion
  -> 180-degree azimuth disambiguation
  -> SHARP native CCD cutouts and CEA remaps
  -> space-weather keywords
```

The primary SHARP data series are `hmi.sharp_720s`, `hmi.sharp_cea_720s`, `hmi.sharp_720s_nrt`, and `hmi.sharp_cea_720s_nrt`. The CEA series provides vector components as `Br`, `Bt`, and `Bp`, while the native CCD series provides field strength, inclination, azimuth, and related maps. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm

## 1. HMI vector-field precursor products

The vector magnetic field is derived from full-disk HMI filtergrams observed in polarized light at multiple wavelengths across a spectral line. The filtergrams are calibrated, registered, and combined into Stokes polarization parameters, which are then inverted with VFISV. The final vector-field step resolves the azimuthal direction of the transverse field. Source: http://jsoc.stanford.edu/HMI/Vector_products.html

## 2. Active-region mask generation

The mask stage uses LOS magnetograms and continuum/intensity images, commonly `hmi.M_720s` and `hmi.Ic_noLimbDark_720s`, to generate active-region masks such as `hmi.Marmask_720s`. The public JSOC module `hmi_segment_module.c` documents typical production usage with `xm='hmi.M_720s[...]'`, `xp='hmi.Ic_noLimbDark_720s[...]'`, and `model=/builtin/hmi.M_Ic_noLimbDark_720s.production`. Source: https://github.com/JSOC-SDP/proj/blob/main/mag/ident/apps/hmi_segment_module.c

The segmentation core, `hmi_segment`, combines magnetogram and intensity inputs with model parameters, disk geometry, and Markov-random-field-style spatial smoothness. Its code calls probability/model and MRF helpers such as `mixNprob2d`, `makemrfdiscwts`, `mrf_segment_wts`, `clean_edge_label`, and `roi_stats_mag`. Source: https://github.com/JSOC-SDP/proj/blob/main/mag/ident/libs/mexfunctions/hmi_segment.c

## 3. HARP detection, grouping, tracking, and ingestion

A HARP is an HMI Active Region Patch: one tracked magnetic region crossing the visible disk. HARPs are conceptually similar to NOAA active-region numbers but are assigned by the HMI pipeline and can exist before NOAA numbers are assigned or for smaller magnetic regions. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm

The HARP grouping routine `hmi_patch` finds active-region patches in a mask image, returns bounding boxes, and optionally returns region statistics. Its key operations are: make a binary active mask, smooth it on the projected solar sphere, threshold the smoothed mask, identify connected components, compute bounding boxes, and calculate region statistics. Source: https://github.com/JSOC-SDP/proj/blob/main/mag/harp/libs/matlab/mfile-mex/hmi-mask-patch/hmi_patch.c

The spherical smoothing routine `smoothsphere` smooths on projected-sphere geometry using a radially symmetric kernel whose distance is computed in normalized 3D coordinates. The connected-component routine `concomponent` labels binary active masks using 4- or 8-neighbor connectivity, with 8-neighbor behavior documented as the default. Source: https://github.com/JSOC-SDP/proj/blob/main/mag/harp/libs/matlab/mfile-mex/hmi-mask-patch/smoothsphere.c; Source: https://github.com/JSOC-SDP/proj/blob/main/mag/harp/libs/matlab/mfile-mex/hmi-mask-patch/concomponent.c

The top-level HARP driver `track_and_ingest_mharp.sh` runs tracking from an input mask series and ingests tracks into HARP DRMS series. `ingest_mharp.c` documents that a Matlab tracker creates filesystem products including HARP lists, geometry files, statistics summaries, and region-mask FITS files, after which the ingestor writes them to JSOC/DRMS. Source: https://github.com/JSOC-SDP/proj/blob/main/mag/harp/scripts/track_and_ingest_mharp.sh; Source: https://github.com/JSOC-SDP/proj/blob/main/mag/harp/apps/ingest_mharp.c

## 4. Definitive versus near-real-time products

Near-real-time HARPs are calculated as soon as possible and their heliographic bounding boxes can change with time. Definitive HARPs are defined after disk passage or about five days after disappearance; their heliographic bounding boxes are constant over the disk passage. NRT and definitive HARPNUM values can differ because NRT regions can later merge or be reinterpreted. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm

## 5. VFISV inversion

Within the HARP bounding region, the HMI Stokes `I,Q,U,V` data are inverted with VFISV, the Very Fast Inversion of the Stokes Vector. VFISV assumes a Milne-Eddington atmosphere and returns vector magnetic-field parameters, Doppler velocity, thermodynamic parameters, and uncertainty estimates. The SHARP documentation states that the fill factor is assumed unity. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm

## 6. 180-degree azimuth ambiguity resolution

The transverse-field azimuth has a 180-degree ambiguity. SHARP uses a minimum-energy method for the reported azimuth and field components, with weak-field alternative solutions recorded for diagnostics. The public wrapper `disambig_v3.c` calls the Fortran ambiguity code, handles geometry/ephemeris, builds bitmaps/noise masks, and writes `disambig` and `conf_disambig` products. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm; Source: https://github.com/JSOC-SDP/proj/blob/main/mag/ambig/apps/disambig_v3.c

The documented `DISAMBIG` bits are: lowest bit for the minimum-energy solution, middle bit for a random weak-field solution, and higher bit for a radial-acute weak-field solution; strong-field pixels use the minimum-energy solution. `CONF_DISAMBIG` values include `0` for not disambiguated, `50` for weak-field method applied, `60` for smoothing applied, and `90` for annealed/high-confidence strong-field pixels. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm

## 7. SHARP product creation and CEA remapping

The `sharp.c` module creates both native SHARP cutouts and CEA SHARP products from HARP and vector-field inputs. Its comments describe two outputs: a CEA-remapped product with remapped magnetogram, bitmap, continuum, Doppler, vector field, and space-weather indices; and a cutout product with HARP-sized native CCD segments. Source: https://github.com/JSOC-SDP/proj/blob/main/sharp/apps/sharp.c

For CEA products, image-coordinate vectors are transformed into heliographic components. The helper `img2helioVector.c` states that it uses the Hagyard and Gary-Hagyard vector-transformation formulae to transform image-coordinate vector components into heliographic components at each location. Source: https://github.com/JSOC-SDP/proj/blob/main/sharp/apps/img2helioVector.c

## 8. BITMAP and pixel selection

`BITMAP` encodes whether pixels lie inside or outside the smooth HARP bounding curve and whether they are weak or strong field. The `sw_functions.c` comments define representative values: `1` weak field outside the curve, `2` strong field outside the curve, `33` weak field inside the curve, and `34` strong field inside the curve. Source: https://github.com/JSOC-SDP/proj/blob/main/sharp/apps/sw_functions.c

Space-weather vector-field keywords are computed only on selected pixels. The SHARP documentation says these are the logical AND of pixels within the smooth bounding curve and pixels above the noise threshold in `CONF_DISAMBIG`. The code implements this selection with thresholds equivalent to high-confidence `conf_disambig` and inside-region `bitmap` values. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm; Source: https://github.com/JSOC-SDP/proj/blob/main/sharp/apps/sw_functions.c

## 9. Space-weather keyword algorithms

The SHARP keyword code computes vector-field quantities including `USFLUX`, `MEANGAM`, `MEANGBT`, `MEANGBZ`, `MEANGBH`, `MEANJZD`, `TOTUSJZ`, `MEANALP`, `MEANJZH`, `TOTUSJH`, `ABSNJZH`, `SAVNCPP`, `MEANPOT`, `TOTPOT`, `MEANSHR`, and `SHRGT45`. It also computes LOS quantities such as `R_VALUE`, `MEANGBL`, `USFLUXL`, and `CMASKL`. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm; Source: https://github.com/JSOC-SDP/proj/blob/main/sharp/apps/sw_functions.c; Source: https://github.com/mbobra/SHARPs/blob/master/calculate_sharpkeys.py

The implementation calculates flux sums with pixel-area factors, horizontal and total field magnitudes from vector components, derivatives with finite differences, vertical current density from horizontal-field derivatives, helicity from current and vertical field, potential fields with Green's functions, and shear/free-energy quantities by comparing observed and potential fields. The official SHARP page states that derivative-dependent quantities use a finite-difference method with a 9-point stencil and that the potential field uses Green's functions with a monopole depth of `0.00001` pixels. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm

## 10. Workflow orchestration

Operationally, JSOC workflow scripts connect the stages as task dependencies. The public workflow repository includes update scripts for `Marmask`, `Harp`, `VFISV`, vector products, `B_720s`, `sharp`, and `sharp_nrt`. Source: https://github.com/JSOC-SDP/workflow

A practical dependency chain is therefore: input HMI observables become available; Marmask segmentation runs; HARP tracking/ingestion runs; VFISV/vector and disambiguation tasks run; SHARP tasks create native and CEA products; web/export/image products can then be generated. Source: https://github.com/JSOC-SDP/workflow

## Caveats

The official SHARP documentation warns that the products should not be used uncritically. Limitations include HMI spatial and spectral resolution, known and unknown systematic errors, orbital effects, and imperfections in inversion and disambiguation. NRT products are faster and less final than definitive products. Source: http://jsoc.stanford.edu/doc/data/hmi/sharp/sharp.htm
