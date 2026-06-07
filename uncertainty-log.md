---
title: Uncertainty Log
created: 2026-06-07
updated: 2026-06-07
type: summary
tags: [solar-physics, space-weather, uncertainty, verification]
sources: [/Users/mausr/Downloads/wiki.zip, _meta/source-inspection.json]
confidence: medium
---

# Uncertainty Log

This page records open questions, missing details, and claims that need primary-source verification before they are treated as stable wiki knowledge.

## Open questions

- [[nf2]] training guidance: Which architecture, learning-rate, and sampling choices are recommended for different active-region and full-disk use cases?
- [[nf2]] multi-height data: Which instruments and input formats are supported for multi-height magnetic observations, and how is noise handled?
- [[pinn-me]] preprocessing: What normalization, wavelength calibration, and spectropolarimetric quality-control steps are recommended before inversion?
- [[sunerf]] observation model: How should stray light, point-spread functions, and instrument cross-calibration be represented in neural tomographic reconstruction?
- [[pfss-tools]] source-surface choice: How sensitive are open-field maps and downstream solar-wind predictions to the chosen source-surface radius?
- [[qsl-tools]] boundary conditions: How do periodic, open, and finite-domain assumptions differ across QSL and field-line tracing tools?
- [[solar-wind-tools]] parameter choices: How strongly do WSA, DCHB, current-sheet, and boundary-condition choices change wind-speed predictions?
- [[dem-tools]] cross-calibration: How do DEMReg, demregpy, demcmc, EMToolKit, DeepEM, and sunkit-dem compare on the same benchmark datasets?
- [[mas]] heating models: Which coronal-heating parameterizations are supported, and how do they affect predicted coronal and heliospheric structure?

## Merge cautions from the external wiki

- Verify licenses, maintainers, institutions, and development status before importing those fields from `/Users/mausr/Downloads/wiki.zip`.
- Replace cursor-style citations from the external wiki with explicit repository, documentation, paper, or official-site URLs.
- Prefer individual software pages as canonical homes for facts; grouped prose should live in concept or comparison pages.
