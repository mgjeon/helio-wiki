---
title: Wiki Index
created: 2026-06-07
updated: 2026-06-07
type: summary
tags: [solar-physics, space-weather, index]
sources: [raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md, raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md]
confidence: high
---

# Wiki Index

> Solar physics and space weather software knowledge base. Last updated: 2026-06-07 | Total pages: 107

Landing page: [[README]].

## Support
- [[SCHEMA]] — conventions, frontmatter, and tag taxonomy.
- [[agent-update-guidelines]] — operating instructions for future LLM agents updating the wiki.
- [[llm-collaboration-hub]] — dynamic coordination hub for LLM improvement discussions and change history.
- [[log]] — chronological ingest log.
- [[glossary]] — short definitions for recurring heliophysics terms.
- [[uncertainty-log]] — open verification questions and merge cautions.

## Ecosystem
- [[overview]] — Ecosystem-level orientation for the heliosphere wiki.
- [[taxonomy]] — Compact method/data/software taxonomy.
- [[workflow-map]] — Observation-to-forecasting workflow map.

## Comparisons
- [[pfss-tools]] — PFSS and potential-field tooling.
- [[nlfff-tools]] — NLFFF, neural-field, and magnetic-field inversion tooling.
- [[qsl-tools]] — QSL and field-line topology tooling.
- [[dem-tools]] — Differential emission measure software.
- [[cme-tools]] — CME structure and propagation tooling.
- [[solar-wind-tools]] — Ambient solar-wind modeling and data tools.
- [[external-wiki-comparison]] — Comparison with the independently generated wiki archive and improvement directions.

## Concepts
- [[active-region-parameters]] — Active Region Parameters.
- [[ambient-solar-wind-modeling]] — Ambient Solar Wind Modeling.
- [[cme-propagation-models]] — CME Propagation Models.
- [[cme-structure-models]] — CME Structure Models.
- [[coronal-heating-and-loop-synthesis]] — Coronal Heating and Loop Synthesis.
- [[coronal-magnetic-field-modeling]] — Coronal Magnetic Field Modeling.
- [[differential-emission-measure]] — Differential Emission Measure Software.
- [[heliosphere-model]] — Heliosphere Model.
- [[qsl-and-field-line-topology]] — QSL and Field-Line Topology.
- [[solar-data-access]] — Solar Data Access.

## Queries
- [[jsoc-sharp-pipeline-structure]] — JSOC SHARP/HARP/HMI vector-field pipeline structure, algorithms, code paths, product series, and caveats.

## Software

### Active Region Parameters
- [[artop]] — Active Region Topology (ARTop) - a tool for studying topological quantities in solar active regions. Source: https://github.com/DavidMacT/ARTop
- [[sharps]] — The Solar Dynamics Observatory (SDO) takes about a terabyte and a half of data a day, which is more data than any other satellite in the NASA Heliophysics Divis. Source: https://github.com/mbobra/SHARPs
- [[smarps]] — We derived Space-weather MDI Active Region Patches, or SMARPs, from maps of the solar surface magnetic field taken by the Michelson Doppler Imager (MDI) aboard . Source: https://github.com/mbobra/SMARPs

### Ambient Solar Wind Model
- [[client-python]] — **HAPI Client for Python**. Source: https://github.com/hapi-server/client-python
- [[deepwiki-comproj]] — https://deepwiki.com/JSOC-SDP/proj/. Source: https://deepwiki.com/JSOC-SDP/proj/
- [[forecast-products-the-space-weather-forecast-laboratory]] — Forecast Products - The Space Weather Forecast Laboratory. Source: https://research.reading.ac.uk/met-spate/huxt-forecast/
- [[hux]] — Abstract. Source: https://github.com/predsci/HUX
- [[hux-paper3]] — Evaluating the Heliospheric Upwind eXtrapolation (HUX) Technique developed by Riley et al. [1, 2] to map solar wind streams radially between different regions i. Source: https://github.com/predsci/HUX-paper3
- [[huxt]] — HUXt - a computationally efficient solar wind model. Source: https://github.com/University-of-Reading-Space-Science/HUXt
- [[jsoc-sdp-drms-deepwiki]] — JSOC-SDP/drms | DeepWiki. Source: https://deepwiki.com/JSOC-SDP/drms
- [[nso-global-oscillation-network-group-gong]] — NSO: Global Oscillation Network Group (GONG). Source: https://gong.nso.edu/
- [[parameter-estimation-solar-wind]] — Bayesian Inference and Global Sensitivity Analysis for Ambient Solar Wind Prediction. Source: https://github.com/opaliss/Parameter_Estimation_Solar_Wind
- [[pfsspy]] — From David Stansby, the lead author of *pfsspy*:. Source: https://github.com/dstansby/pfsspy
- [[solarmach]] — solarmach. Source: https://github.com/jgieseler/solarmach
- [[synoptic-group-zero-point-corrected-magnetogram-synoptic-map-images]] — Synoptic Group Zero Point Corrected Magnetogram Synoptic Map Images. Source: https://magmap.nso.edu/index.html
- [[synoptic-maps-nso-national-solar-observatory]] — Synoptic Maps - NSO - National Solar Observatory. Source: https://nso.edu/data/nisp-data/synoptic-maps/
- [[unifying-the-validation-of-ambient-solar-wind-models]] — Redirecting. Source: https://doi.org/10.1016/j.asr.2022.05.026
- [[wsa-enlil-at-swpc-3-nasa-ccmc]] — WSA-Enlil-at-SWPC 3 | NASA CCMC. Source: https://ccmc.gsfc.nasa.gov/models/WSA-Enlil-at-SWPC~3/
- [[www-swpc-noaa-govreal-time-solar-wind]] — https://www.swpc.noaa.gov/products/real-time-solar-wind. Source: https://www.swpc.noaa.gov/products/real-time-solar-wind
- [[www-swpc-noaa-govwsa-enlil-solar-wind-prediction]] — https://www.swpc.noaa.gov/products/wsa-enlil-solar-wind-prediction. Source: https://www.swpc.noaa.gov/products/wsa-enlil-solar-wind-prediction

### Barnes
- [[ebtelplusplus]] — ebtelplusplus. Source: https://github.com/rice-solar-physics/ebtelplusplus
- [[fiasco]] — fiasco. Source: https://github.com/wtbarnes/fiasco
- [[greensfield]] — greensfield. Source: https://github.com/wtbarnes/greensfield
- [[pydrad]] — pydrad. Source: https://github.com/rice-solar-physics/pydrad
- [[synthesizar]] — synthesizAR. Source: https://github.com/wtbarnes/synthesizAR

### CME Propagation Model
- [[beacon2science]] — Beacon2Science: Enhancing STEREO/HI beacon data with machine learning for efficient CME tracking. Source: https://github.com/lelouedec/beacon2science
- [[cme-propagation-through-the-heliosphere-status-and-future-of-observations-and-model-development]] — https://www.sciencedirect.com/science/article/pii/S0273117723005239. Source: https://www.sciencedirect.com/science/article/pii/S0273117723005239
- [[dbm]] — P-DBM : Probabilistic Drag Based Model. Source: https://github.com/astronish16/DBM
- [[dbm-cdbm-201510-nasa-ccmc]] — DBM cdbm_201510 | NASA CCMC. Source: https://ccmc.gsfc.nasa.gov/models/DBM~cdbm_201510/
- [[drag-based-model-dbm-tools-for-forecast-of-coronal-mass-ejection-arrival-time-and-speed]] — Frontiers | Drag-Based Model (DBM) Tools for Forecast of Coronal Mass Ejection Arrival Time and Speed. Source: https://www.frontiersin.org/journals/astronomy-and-space-sciences/articles/10.3389/fspas.2021.639986/full
- [[elevohi]] — ELEvoHI. Source: https://github.com/tamerstorfer/ELEvoHI
- [[stereo-science-center-home-page]] — STEREO - Science Center Home Page. Source: https://stereo-ssc.nascom.nasa.gov/
- [[stereo-hi-data-processing]] — STEREO-HI-Data-Processing. Source: https://github.com/maikebauer/STEREO-HI-Data-Processing
- [[the-soho-lasco-instrument-homepage]] — The SOHO/LASCO Instrument Homepage. Source: https://lasco-www.nrl.navy.mil/index.php

### CME Structure Model
- [[cone-model-for-cme]] — Cone Model for CME. Source: https://github.com/astronish16/Cone_Model_for_CME
- [[gcs-benchmarking]] — GCS-Benchmarking. Source: https://github.com/KeyanGootkin/GCS-Benchmarking
- [[gcs-python]] — GCS in Python. Source: https://github.com/johan12345/gcs_python
- [[numerical-modeling-of-solar-wind-and-coronal-mass-ejection-in-the-inner-heliosphere-a-review]] — Frontiers | Numerical modeling of solar wind and coronal mass ejection in the inner heliosphere: A review. Source: https://doi.org/10.3389/fspas.2023.1105797
- [[pythea]] — PyThea: A software package to reconstruct the 3D structure of CMEs and shock waves. Source: https://github.com/AthKouloumvakos/PyThea
- [[stereocat]] — StereoCat. Source: https://ccmc.gsfc.nasa.gov/analysis/stereo/

### DEM
- [[deepem]] — DeepEM: A Deep Learning Approach for DEM Inversion. Source: https://github.com/PaulJWright/DeepEM
- [[demcmc]] — demcmc. Source: https://github.com/dstansby/demcmc
- [[demreg]] — DEMReg. Source: https://github.com/ianan/demreg
- [[demregpy]] — demregpy. Source: https://github.com/alasdairwilson/demregpy
- [[emtoolkit]] — EMToolKit. Source: https://github.com/jeplowman/EMToolKit
- [[sunkit-dem]] — ``sunkit-dem``. Source: https://github.com/sunpy/sunkit-dem

### GX Simulator
- [[gx-simulator]] — GX_SIMULATOR. Source: https://github.com/Gelu-Nita/GX_SIMULATOR

### Guo
- [[magnetic-modeling-codes]] — Magnetic Modeling Codes. Source: https://github.com/njuguoyang/magnetic_modeling_codes

### Heliosphere Model
- [[heliophysics-educational-resources]] — Heliophysics Educational Resources | Heliophysics. Source: https://heliophysics.ucar.edu/resources

### JSOC
- [[drms]] — TGT_BIN		:= $(TGT_BIN) $(TGT_$(d)). Source: https://github.com/JSOC-SDP/drms
- [[joint-science-operations-center-jsoc-data-products]] — Joint Science Operations Center (JSOC) Data Products. Source: http://jsoc.stanford.edu/
- [[proj]] — smpl_03.c	prints a list of the data series known to DRMS - a simple. Source: https://github.com/JSOC-SDP/proj
- [[workflow]] — Also some reference versions of HMI observables code,. Source: https://github.com/JSOC-SDP/workflow

### Jarolim
- [[nf2]] — Neural Network Force-Free Magnetic Field Extrapolation - NF2. Source: https://github.com/RobertJaro/NF2
- [[pinn-me]] — A Physics-Informed Neural Network Framework for Accurate Milne-Eddington Inversions of Solar Magnetic Fields. Source: https://github.com/RobertJaro/pinn-me
- [[sunerf]] — SuNeRF. Source: https://github.com/RobertJaro/SuNeRF

### Predictive Science
- [[chmap]] — CHMAP: Coronal Hole Mapping and Analysis Pipeline. Source: https://github.com/predsci/CHMAP
- [[mapflpy]] — :alt: Python Versions. Source: https://github.com/predsci/mapflpy
- [[mas]] — Magnetohydrodynamic Algorithm outside a Sphere. Source: https://github.com/predsci/MAS
- [[oft]] — OFT: Open Source Flux Transport. Source: https://github.com/predsci/OFT
- [[predictive-science-inc-home]] — Predictive Science Inc. - Home. Source: https://www.predsci.com/portal/home.php
- [[psi-io]] — :alt: Python Versions. Source: https://github.com/predsci/psi-io
- [[pyvisual]] — :alt: Python Versions. Source: https://github.com/predsci/pyvisual
- [[swig]] — SWiG: Solar Wind Generator. Source: https://github.com/predsci/SWiG

### QSL
- [[fastqsl]] — FastQSL. Source: https://github.com/el2718/FastQSL
- [[fastqsl-2]] — FastQSL. Source: https://github.com/peijin94/FastQSL
- [[fastqsl2]] — FastQSL 2. Source: https://github.com/el2718/FastQSL2
- [[ufit]] — UFiT - Universal Fieldline Tracer. Source: https://github.com/Valentin-Aslanyan/UFiT

### Sunpy
- [[streamtracer]] — Python library to calculate streamlines. Source: https://github.com/sunpy/streamtracer
- [[sunkit-magex]] — ``sunkit-magex`` is a Python software package that provides a set of tools for the modelling of magnetic field data.. Source: https://github.com/sunpy/sunkit-magex
- [[sunkit-pyvista]] — 3D visualisation of solar physics data with pyvista.. Source: https://github.com/sunpy/sunkit-pyvista

### Yeates
- [[flhtools]] — flhtools. Source: https://github.com/antyeates1983/flhtools
- [[pfss]] — pfss. Source: https://github.com/antyeates1983/pfss
- [[sft-data]] — sft_data. Source: https://github.com/antyeates1983/sft_data
- [[sharps-bmrs]] — sharps-bmrs. Source: https://github.com/antyeates1983/sharps-bmrs
- [[sphtools]] — sphtools. Source: https://github.com/antyeates1983/sphtools
