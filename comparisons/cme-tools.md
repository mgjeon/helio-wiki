---
title: CME Tools Comparison
created: 2026-06-07
updated: 2026-06-07
type: comparison
tags: [solar-physics, cme, gcs, cone-model, drag-based-model, comparison]
sources: [raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md]
confidence: medium
---

# CME Tools Comparison

CME tools split into structure/reconstruction resources and propagation/arrival resources. Source: [[cme-structure-models]], [[cme-propagation-models]]

| Tool | Main role | Inputs/context | Notes |
| --- | --- | --- | --- |
| [[cone-model-for-cme]] | Cone-model CME geometry | CME structure source-list grouping | Geometric reconstruction style entry. Source: https://github.com/astronish16/Cone_Model_for_CME |
| [[pythea]] | 3D CME/shock reconstruction package | CME structure source-list grouping | Reconstructs 3D structure according to page title. Source: https://github.com/AthKouloumvakos/PyThea |
| [[gcs-python]] | Graduated Cylindrical Shell modeling in Python | CME structure source-list grouping | Python GCS implementation. Source: https://github.com/johan12345/gcs_python |
| [[gcs-benchmarking]] | GCS benchmarking | CME structure source-list grouping | Comparison/benchmarking support. Source: https://github.com/KeyanGootkin/GCS-Benchmarking |
| [[dbm]] | Drag-Based Model implementation | CME propagation source-list grouping | Arrival-time/speed forecasting context. Source: https://github.com/astronish16/DBM |
| [[elevohi]] | HI-based CME propagation modeling | CME propagation source-list grouping | Heliospheric imager context. Source: https://github.com/tamerstorfer/ELEvoHI |
| [[beacon2science]] | ML-enhanced STEREO/HI beacon data | CME tracking/source-list grouping | Data enhancement rather than standalone physics propagation. Source: https://github.com/lelouedec/beacon2science |

## Selection notes

- Use structure tools such as [[pythea]], [[gcs-python]], and [[cone-model-for-cme]] when the question is CME geometry. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
- Use [[dbm]] or [[elevohi]] when the question is heliospheric propagation or arrival behavior. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
- Use [[stereo-science-center-home-page]] and [[the-soho-lasco-instrument-homepage]] as observational context for CME workflows. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
