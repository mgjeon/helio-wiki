---
title: POP-CORN
created: 2026-06-08
updated: 2026-06-08
type: software
tags: [solar-physics, space-weather, heliophysics, coronal-hole, neural-network, solar-wind, forecasting, image-processing]
sources: [https://arxiv.org/abs/2603.25591]
confidence: medium
---

# POP-CORN

POP-CORN is presented as a neural-network coronal-hole detection tool, with validation focused on identifying large-scale coronal holes in solar EUV imagery [arXiv:2603.25591](https://arxiv.org/abs/2603.25591).

## Scientific purpose

- Coronal holes are important sources of high-speed solar wind streams; their morphology and distribution influence the solar-wind structure observed at 1 au [arXiv:2603.25591](https://arxiv.org/abs/2603.25591).
- POP-CORN therefore sits at the interface between remote-sensing image segmentation and [[ambient-solar-wind-modeling]].

## Methods and algorithms

- Uses neural networks for coronal-hole detection in solar corona images [arXiv:2603.25591](https://arxiv.org/abs/2603.25591).

## Recommended use cases

- Automated coronal-hole boundary detection feeding solar-wind source-region analysis.
- Benchmarking AI-based coronal-hole segmentation against more traditional thresholding or rule-based pipelines.

## Uncertainties

- **Uncertain:** repository URL, model weights, training-data availability, license, and installation route were not verified from a primary software repository during this update.

## Related wiki pages

- [[ambient-solar-wind-modeling]]
- [[solar-wind-tools]]
- [[chmap]]
