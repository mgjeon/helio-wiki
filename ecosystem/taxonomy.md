---
title: Heliosphere Wiki Taxonomy
created: 2026-06-07
updated: 2026-06-07
type: concept
tags: [solar-physics, space-weather, taxonomy]
sources: [raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md, raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md, SCHEMA.md]
confidence: medium
---

# Heliosphere Wiki Taxonomy

The wiki uses method, data, and software tags from [[SCHEMA]] to group tools by scientific role rather than only by source-list section. Source: [[SCHEMA]]

## Methods

- Potential-field and PFSS modeling: [[pfss]], [[pfsspy]], [[sunkit-magex]], [[pfss-tools]]. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
- NLFFF, neural-field, and magnetic inversion methods: [[nf2]], [[pinn-me]], [[magnetic-modeling-codes]], [[nlfff-tools]]. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md
- QSL and field-line topology: [[fastqsl]], [[fastqsl2]], [[fastqsl-2]], [[ufit]], [[qsl-tools]]. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md
- CME geometry and propagation: [[cone-model-for-cme]], [[pythea]], [[gcs-python]], [[dbm]], [[elevohi]], [[cme-tools]]. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
- DEM inversion and thermal diagnostics: [[demreg]], [[demregpy]], [[demcmc]], [[emtoolkit]], [[deepem]], [[sunkit-dem]], [[dem-tools]]. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md

## Data and observations

- Magnetogram/synoptic inputs: [[joint-science-operations-center-jsoc-data-products]], [[drms]], [[nso-global-oscillation-network-group-gong]], [[synoptic-maps-nso-national-solar-observatory]]. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md
- In-situ and heliospheric data: [[www-swpc-noaa-govreal-time-solar-wind]], [[client-python]], [[stereo-science-center-home-page]], [[the-soho-lasco-instrument-homepage]]. Source: raw/transcripts/Solar-Physics-Codes-Solar-Wind-CME_1.md

## Software status markers

- `maintained`, `inactive`, and `research-code` tags should be interpreted cautiously unless a page cites explicit repository or documentation evidence. Source: [[SCHEMA]]
- Pages with `confidence: low` or explicit **Uncertain** notes need future source verification before being treated as stable references. Source: [[SCHEMA]]
