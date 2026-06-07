---
title: PFSS Tools Comparison
created: 2026-06-07
updated: 2026-06-07
type: comparison
tags: [solar-physics, magnetic-field, pfss, comparison]
sources: [raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md, raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md]
confidence: medium
---

# PFSS Tools Comparison

PFSS tools in this wiki support potential-field coronal modeling from photospheric/synoptic magnetic maps, with different emphasis on research scripts, package interfaces, and downstream solar-wind workflows. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md

| Tool | Main role | Inputs/context | Notes |
| --- | --- | --- | --- |
| [[pfss]] | Finite-difference PFSS model in a spherical shell | HMI, GONG, NSO/KPVT/SOLIS-style synoptic maps are mentioned in its README notes | Compact research code from the Yeates grouping. Source: https://github.com/antyeates1983/pfss |
| [[pfsspy]] | Python PFSS package | Synoptic maps and SunPy-oriented workflows | Archived/no longer developed per README note in page. Source: https://github.com/dstansby/pfsspy |
| [[sunkit-magex]] | SunPy-affiliated magnetic extrapolation package | Built on SunPy/Astropy; currently supports PFSS according to README note | Natural successor-style option for SunPy users. Source: https://github.com/sunpy/sunkit-magex |
| [[mas]] | MHD coronal model rather than PFSS-only tool | Predictive Science modeling context | Useful as a higher-physics coronal-model comparator. Source: https://github.com/predsci/MAS |

## Selection notes

- Use [[sunkit-magex]] when a maintained SunPy-affiliated Python interface is preferred. Source: https://github.com/sunpy/sunkit-magex
- Use [[pfss]] or [[pfsspy]] as reference implementations or for reproducing workflows documented around those repositories. Source: https://github.com/antyeates1983/pfss, https://github.com/dstansby/pfsspy
- Compare PFSS output with [[mas]], [[swig]], [[hux]], or [[huxt]] when the research question moves toward solar-wind or heliospheric forecasting. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
