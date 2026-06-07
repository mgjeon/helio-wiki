---
title: DEM Tools Comparison
created: 2026-06-07
updated: 2026-06-07
type: comparison
tags: [solar-physics, dem, comparison]
sources: [raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md]
confidence: medium
---

# DEM Tools Comparison

DEM tools in the supplied source list cover regularized inversion, MCMC, general toolkit workflows, and machine-learning DEM estimation. Source: [[differential-emission-measure]]

| Tool | Main role | Inputs/context | Notes |
| --- | --- | --- | --- |
| [[demreg]] | Regularized DEM inversion | DEM source-list grouping | Original/source implementation in the list. Source: https://github.com/ianan/demreg |
| [[demregpy]] | Python DEMReg implementation/wrapper | DEM source-list grouping | Python-oriented option. Source: https://github.com/alasdairwilson/demregpy |
| [[demcmc]] | MCMC DEM estimation | DEM source-list grouping | Useful when posterior/uncertainty exploration is central. Source: https://github.com/dstansby/demcmc |
| [[emtoolkit]] | Emission-measure analysis toolkit | DEM source-list grouping | Broader toolkit-style entry. Source: https://github.com/jeplowman/EMToolKit |
| [[deepem]] | Deep-learning DEM inversion | DEM source-list grouping | ML-oriented entry. Source: https://github.com/PaulJWright/DeepEM |
| [[sunkit-dem]] | SunPy-affiliated DEM package | SunPy ecosystem context | Prefer for SunPy-style workflows when feature fit is adequate. Source: https://github.com/sunpy/sunkit-dem |

## Selection notes

- Use [[demreg]]/[[demregpy]] for regularized-inversion workflows. Source: https://github.com/ianan/demreg, https://github.com/alasdairwilson/demregpy
- Use [[demcmc]] when uncertainty sampling is more important than speed. Source: https://github.com/dstansby/demcmc
- Treat [[deepem]] as a machine-learning DEM entry whose training data and generalization assumptions should be checked before production use. Source: https://github.com/PaulJWright/DeepEM
