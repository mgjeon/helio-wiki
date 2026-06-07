---
title: Wiki-Based Ecosystem Briefing Format
created: 2026-06-08
updated: 2026-06-08
type: query
tags: [solar-physics, space-weather, wiki, briefing, synthesis]
sources: [index.md, ecosystem/overview.md, ecosystem/taxonomy.md, ecosystem/workflow-map.md, comparisons/pfss-tools.md, comparisons/nlfff-tools.md, comparisons/qsl-tools.md, comparisons/dem-tools.md, comparisons/cme-tools.md, comparisons/solar-wind-tools.md]
confidence: high
---

# Wiki-Based Ecosystem Briefing Format

This note records the preferred meaning of a solar/space-weather software ecosystem "briefing" when the request is not primarily for current NOAA/arXiv updates. The goal is to turn stored wiki knowledge into a readable synthesis that helps the user maintain an active mental model of the tool ecosystem.

## Intended briefing style

A wiki-based briefing should use the current LLM wiki as the source base and should not primarily chase new external updates. It should answer:

- What tools are currently represented in the wiki?
- What scientific problems and workflow stages do they cover?
- What algorithms or modeling assumptions distinguish them?
- What do tools in the same family have in common?
- Where do they differ in inputs, outputs, speed, physics fidelity, uncertainty treatment, and research use?
- What are the likely strengths, limitations, and open verification points?
- How do the tools connect conceptually and in code/data workflows?
- How could a researcher combine them into concrete study designs?

## Recommended structure

1. **Reading thesis** — one paragraph summarizing the ecosystem as a workflow, not a list.
2. **Workflow map** — observation/data access → magnetograms/active regions → coronal fields → topology/QSL → solar wind/heliosphere → CME structure/propagation → DEM/thermal diagnostics.
3. **Tool families** — one section per family:
   - PFSS / potential-field tools: [[pfss]], [[pfsspy]], [[sunkit-magex]], [[mas]] as higher-physics comparator.
   - NLFFF / magnetic inversion: [[nf2]], [[pinn-me]], [[magnetic-modeling-codes]], [[sft-data]].
   - QSL / field-line topology: [[fastqsl]], [[fastqsl2]], [[fastqsl-2]], [[ufit]], [[streamtracer]].
   - Ambient solar wind: [[mas]], [[swig]], [[hux]], [[huxt]], [[wsa-enlil-at-swpc-3-nasa-ccmc]], [[pop-corn]], [[swdatatoolkit]].
   - CME tools: [[cone-model-for-cme]], [[pythea]], [[gcs-python]], [[gcs-benchmarking]], [[atharv]], [[dbm]], [[elevohi]], [[beacon2science]].
   - DEM / thermal diagnostics: [[demreg]], [[demregpy]], [[demcmc]], [[emtoolkit]], [[deepem]], [[sunkit-dem]].
4. **Commonality/difference table** — compare inputs, outputs, core model, uncertainty handling, computational cost, maturity, and best-fit research question.
5. **Code/data connection graph** — explain likely handoffs, e.g. JSOC/GONG/HAPI data → PFSS/MAS/NF2 → field-line/QSL analysis → solar-wind/CME propagation → validation against SWPC/in-situ observations.
6. **Research-use recipes** — 3–5 concrete study patterns, such as comparing PFSS vs MHD open flux, evaluating CME arrival forecasts, or testing DEM uncertainty under different inversion methods.
7. **What to inspect next** — list wiki pages whose confidence is medium/low or whose repository details remain uncertain.

## Tone and constraints

- Prefer explanatory prose that the user can read to refresh understanding.
- Use tables only when they improve comparison; avoid dumping every URL.
- Make clear when a statement is based only on currently stored wiki knowledge.
- Distinguish code maturity from scientific method: a strong algorithm may live in research code, while a convenient package may implement a simpler model.
- If a briefing reveals missing conceptual glue, update comparison/concept pages rather than leaving the synthesis only in chat.

## Short prompt template

> Using only `/Users/mausr/wiki`, write a readable ecosystem briefing. Explain the current tool families, algorithms, commonalities/differences, strengths/limitations, code/data connections, and concrete research-use recipes. Do not focus on latest NOAA/arXiv updates unless they are already in the wiki. Update the wiki if the synthesis reveals useful durable structure.
