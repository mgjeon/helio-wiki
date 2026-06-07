---
title: Heliosphere Workflow Map
created: 2026-06-07
updated: 2026-06-08
type: concept
tags: [solar-physics, space-weather, workflow, heliosphere]
sources: [raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md, raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md, https://arxiv.org/abs/2603.25591, https://arxiv.org/abs/2604.22741, https://arxiv.org/abs/2606.01893]
confidence: medium
---

# Heliosphere Workflow Map

The supplied resources can be read as an observation-to-modeling workflow rather than as independent links. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md

## Observation to forecasting path

1. Solar observations and data access: [[joint-science-operations-center-jsoc-data-products]], [[drms]], [[nso-global-oscillation-network-group-gong]], [[client-python]]. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
2. Magnetogram processing and active-region products: [[sharps]], [[smarps]], [[artop]], [[solar-data-access]]. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md
3. Coronal magnetic-field modeling: [[pfss-tools]], [[nlfff-tools]], [[coronal-magnetic-field-modeling]]. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md
4. Field-line tracing and topology analysis: [[qsl-tools]], [[streamtracer]], [[flhtools]], [[sunkit-pyvista]]. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md
5. Ambient solar-wind and heliosphere modeling: [[solar-wind-tools]], [[mas]], [[swig]], [[hux]], [[huxt]], [[pop-corn]]. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md, https://arxiv.org/abs/2603.25591
6. CME reconstruction, propagation, and ICME interpretation: [[cme-tools]], [[cme-structure-models]], [[cme-propagation-models]], [[atharv]]. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md, https://arxiv.org/abs/2606.01893
7. Thermal diagnostics and emission modeling: [[dem-tools]], [[fiasco]], [[synthesizar]], [[ebtelplusplus]], [[pydrad]]. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md

## Interpretation

- PFSS and solar-wind tools form the clearest bridge between photospheric magnetic maps and heliospheric forecasting. Source: [[ambient-solar-wind-modeling]]
- CME structure tools estimate geometry, while propagation tools estimate arrival behavior or heliospheric evolution. Source: [[cme-structure-models]], [[cme-propagation-models]]
- Newer pipeline-oriented packages such as [[swdatatoolkit]] sit across multiple workflow stages because they combine data acquisition, preprocessing, feature extraction, and magnetic-field analysis. Source: https://arxiv.org/abs/2604.22741
- DEM and loop/heating tools are adjacent to space-weather modeling but mainly support coronal plasma diagnostics and synthetic observables. Source: [[differential-emission-measure]], [[coronal-heating-and-loop-synthesis]]
