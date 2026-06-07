---
title: Solar Wind Tools Comparison
created: 2026-06-07
updated: 2026-06-08
type: comparison
tags: [solar-physics, solar-wind, heliosphere, forecasting, comparison]
sources: [raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md, https://arxiv.org/abs/2603.25591, https://arxiv.org/abs/2604.22741]
confidence: medium
---

# Solar Wind Tools Comparison

Ambient solar-wind resources connect magnetic maps, coronal models, heliospheric propagation, validation, and in-situ observations. Source: [[ambient-solar-wind-modeling]]

| Tool/resource | Main role | Inputs/context | Notes |
| --- | --- | --- | --- |
| [[mas]] | Coronal MHD modeling | Predictive Science source-list grouping | Higher-physics coronal-model entry. Source: https://github.com/predsci/MAS |
| [[swig]] | Solar-wind generation | Predictive Science source-list grouping | Solar-wind model support from Predictive Science. Source: https://github.com/predsci/SWiG |
| [[hux]] | Heliospheric Upwind eXtrapolation model | Ambient solar-wind source-list grouping | Computational heliospheric propagation context. Source: https://github.com/predsci/HUX |
| [[huxt]] | Efficient solar-wind model | University of Reading source-list grouping | Forecasting-oriented HUXt ecosystem. Source: https://github.com/University-of-Reading-Space-Science/HUXt |
| [[wsa-enlil-at-swpc-3-nasa-ccmc]] | WSA-ENLIL model page | CCMC operational/model context | Important operational comparison point. Source: https://ccmc.gsfc.nasa.gov/models/WSA-Enlil-at-SWPC~3/ |
| [[www-swpc-noaa-govreal-time-solar-wind]] | Real-time solar-wind data product | NOAA SWPC observations | Observation/validation resource rather than model code. Source: https://www.swpc.noaa.gov/products/real-time-solar-wind |
| [[client-python]] | HAPI Python client | Heliophysics data access | Supports retrieval of interoperable time-series data. Source: https://github.com/hapi-server/client-python |
| [[pop-corn]] | Neural-network coronal-hole detection | EUV coronal-hole imagery | Upstream source-region segmentation for high-speed solar-wind workflows. Source: https://arxiv.org/abs/2603.25591 |
| [[swdatatoolkit]] | Python data acquisition/preprocessing library | Solar and space-weather data products | Data pipeline layer spanning downloading, preprocessing, feature extraction, and magnetic-field analysis. Source: https://arxiv.org/abs/2604.22741 |

## Selection notes

- Use [[mas]] and [[swig]] when coronal model physics and Predictive Science workflows are central. Source: https://github.com/predsci/MAS, https://github.com/predsci/SWiG
- Use [[hux]] or [[huxt]] for computationally efficient heliospheric solar-wind propagation workflows. Source: https://github.com/predsci/HUX, https://github.com/University-of-Reading-Space-Science/HUXt
- Use NOAA SWPC, HAPI, JSOC, GONG, and synoptic-map pages as data inputs or validation context rather than as substitutable model codes. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
- Use [[pop-corn]] when the workflow needs AI-assisted coronal-hole boundary detection before solar-wind source-region or high-speed stream analysis. Source: https://arxiv.org/abs/2603.25591
- Use [[swdatatoolkit]] when the bottleneck is data acquisition, preprocessing, and feature extraction rather than heliospheric propagation physics. Source: https://arxiv.org/abs/2604.22741
