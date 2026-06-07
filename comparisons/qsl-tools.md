---
title: QSL And Field-Line Tools Comparison
created: 2026-06-07
updated: 2026-06-07
type: comparison
tags: [solar-physics, qsl, field-line-tracing, comparison]
sources: [raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md]
confidence: medium
---

# QSL And Field-Line Tools Comparison

QSL and field-line tools are used after a magnetic-field model or vector field is available; they help analyze connectivity, topology, and field-line geometry. Source: [[qsl-and-field-line-topology]]

| Tool | Main role | Inputs/context | Notes |
| --- | --- | --- | --- |
| [[fastqsl]] | FastQSL implementation | QSL source-list grouping | One of multiple FastQSL repositories in the supplied list. Source: https://github.com/el2718/FastQSL |
| [[fastqsl2]] | FastQSL 2 implementation | QSL source-list grouping | Distinct repository from the original FastQSL page. Source: https://github.com/el2718/FastQSL2 |
| [[fastqsl-2]] | Alternative FastQSL repository | QSL source-list grouping | Keep distinct until provenance and differences are manually reviewed. Source: https://github.com/peijin94/FastQSL |
| [[ufit]] | Universal field-line tracer | Field-line tracing/topology context | Adjacent to QSL workflows. Source: https://github.com/Valentin-Aslanyan/UFiT |
| [[streamtracer]] | Python streamline calculation library | SunPy-related field-line tracing context | Useful as supporting infrastructure rather than QSL-specific tooling. Source: https://github.com/sunpy/streamtracer |

## Selection notes

- Compare the three FastQSL pages before choosing one for reproducibility; the wiki preserves them as distinct sources because they have distinct URLs. Source: raw/transcripts/Solar-Physics-Codes-Magnetic-Fields-Active-Region-DEM_1.md
- Use [[ufit]] or [[streamtracer]] when the task is field-line tracing rather than squashing-factor/QSL computation. Source: https://github.com/Valentin-Aslanyan/UFiT, https://github.com/sunpy/streamtracer
