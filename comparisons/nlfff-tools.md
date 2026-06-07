---
title: NLFFF And Magnetic Inversion Tools Comparison
created: 2026-06-07
updated: 2026-06-07
type: comparison
tags: [solar-physics, magnetic-field, nlfff, neural-field, pinn, comparison]
sources: [raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md]
confidence: medium
---

# NLFFF And Magnetic Inversion Tools Comparison

This grouping covers neural/nonlinear magnetic-field extrapolation, Milne-Eddington inversion, and supporting magnetic-modeling repositories. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md

| Tool | Main role | Inputs/context | Notes |
| --- | --- | --- | --- |
| [[nf2]] | Neural non-linear force-free magnetic-field extrapolation | HMI/SHARP, full-disk, synoptic, benchmark data are noted on the page | Python framework with training, export, and evaluation interfaces. Source: https://github.com/RobertJaro/NF2 |
| [[pinn-me]] | Physics-informed Milne-Eddington inversion | Solar magnetic-field inversion context | Adjacent to extrapolation because it estimates field parameters from observations. Source: https://github.com/RobertJaro/pinn-me |
| [[magnetic-modeling-codes]] | Collection of magnetic modeling codes | Magnetic-field modeling source-list grouping | Use as a repository-level pointer where algorithm details need source inspection. Source: https://github.com/njuguoyang/magnetic_modeling_codes |
| [[sft-data]] | Surface flux transport data/tooling | Yeates magnetic-field workflow context | Supports upstream magnetic-map evolution workflows. Source: https://github.com/antyeates1983/sft_data |

## Selection notes

- Use [[nf2]] when the task is explicitly NLFFF/neural-field extrapolation and Python/GPU workflows are acceptable. Source: https://github.com/RobertJaro/NF2
- Use [[pinn-me]] for Milne-Eddington inversion problems rather than coronal volume extrapolation. Source: https://github.com/RobertJaro/pinn-me
- Treat collection repositories such as [[magnetic-modeling-codes]] as pointers until their individual algorithms are inspected in depth. Source: https://github.com/njuguoyang/magnetic_modeling_codes
