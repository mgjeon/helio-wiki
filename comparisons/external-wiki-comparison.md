---
title: External Wiki Comparison
created: 2026-06-07
updated: 2026-06-07
type: comparison
tags: [solar-physics, space-weather, wiki, comparison, documentation]
sources: [/Users/mausr/Downloads/wiki.zip, README.md, SCHEMA.md, _meta/source-inspection.json]
confidence: medium
---

# External Wiki Comparison

This page compares the current wiki with the independently generated wiki in `/Users/mausr/Downloads/wiki.zip`. The external wiki was generated from the same original link-only source material, but it made different tradeoffs: fewer pages, richer narrative entries, and more explicit uncertainty tracking.

## Baseline snapshot

Counts below describe the current wiki before this comparison pass added [[external-wiki-comparison]], [[glossary]], and [[uncertainty-log]].

| Area | Current wiki | External wiki |
| --- | --- | --- |
| Markdown pages | 101 | 17 |
| Approximate words | 24,624 | 9,989 |
| Software pages | 76 | 10 |
| Median software page length | 254 words | 699 words |
| Core structure | `software/`, `concepts/`, `comparisons/`, `ecosystem/`, `raw/`, `_meta/` | `software/`, `ecosystem/`, plus `glossary.md`, `sources.md`, `uncertainty-log.md` |
| Citation style | Explicit source URLs and local source files | Non-portable cursor-style references from the other LLM session |
| Strength | Coverage, provenance, Obsidian hygiene, source inspection metadata | Reader-oriented explanations, use-case framing, limitations, uncertainty prompts |
| Weakness | Many software pages read like repository inspection records | Much lower coverage and weaker reproducibility of citations |

## What the current wiki does better

- Coverage is substantially broader. The current wiki represents 76 unique inspected URLs, while the external wiki deeply describes only a selected subset.
- Provenance is stronger. Current pages cite explicit URLs, raw transcript files, and `_meta/source-inspection.json`; the external wiki uses citation tokens that are not independently resolvable outside the generation session.
- The current wiki has an explicit operating model: [[SCHEMA]], [[log]], raw transcript preservation, source inspection metadata, and Obsidian graph cleanup.
- The current wiki has better granularity for navigation and maintenance. Separate pages exist for concepts, comparison groups, individual tools, and source-list artifacts.

## What the external wiki does better

- It gives human readers more scientific context. Entries such as PFSS, NF2, DEM tools, solar wind models, and Predictive Science tools explain purpose, methods, inputs, outputs, limitations, and use cases.
- It consistently distinguishes capabilities from caveats. All inspected external software pages include strengths, limitations, recommended use cases, and uncertainties.
- It includes a useful `uncertainty-log.md`, which turns vague weak spots into concrete follow-up questions.
- It includes a compact `glossary.md`, which improves onboarding for LLM agents and humans who do not already know terms like PFSS, NLFFF, QSL, DEM, PINN, NeRF, MAS, SHARP, and HUX.
- Its taxonomy and workflow pages are more explanatory, while the current versions are more like index maps.

## High-value imports

Do not replace current pages wholesale. Instead, import patterns and selected content after converting citations to explicit URLs.

1. Current-wiki-native [[glossary]] and [[uncertainty-log]] pages were seeded during this comparison pass.
2. Add a richer software-page template to [[SCHEMA]] with these sections:
   - Identification
   - Scientific purpose
   - Methods and algorithms
   - Inputs and outputs
   - Installation and usage
   - Strengths
   - Limitations
   - Recommended use cases
   - Uncertainties
   - Related wiki pages
3. Enrich priority software pages first: [[pfss]], [[pfsspy]], [[sunkit-magex]], [[nf2]], [[pinn-me]], [[sunerf]], [[mas]], [[hux]], [[huxt]], [[dbm]], [[demreg]], [[demregpy]], [[fastqsl]], [[fastqsl2]], [[ufit]], [[oft]], [[swig]], [[mapflpy]], [[chmap]], [[psi-io]], [[pyvisual]].
4. Merge the external grouped pages into current comparison/concept pages:
   - `software/solar_wind_models.md` -> [[solar-wind-tools]], [[ambient-solar-wind-modeling]], [[cme-propagation-models]]
   - `software/dem_tools.md` -> [[dem-tools]], [[differential-emission-measure]]
   - `software/predictive_science.md` -> [[solar-wind-tools]] and individual PSI software pages
   - `software/active_region_tools.md` -> [[active-region-parameters]]
   - `software/qsl-tools.md` -> [[qsl-tools]], [[qsl-and-field-line-topology]]
5. Expand [[overview]], [[taxonomy]], and [[workflow-map]] with short explanatory paragraphs from the external wiki, but keep the current source-backed navigation links.

## Risks to manage

- The external wiki contains likely hallucinated or stale details. Examples include repository URL variants, maintainer claims, development status, license claims, and inferred institutional affiliations. Verify all such details against primary sources before merging.
- Its citation format is not portable. Do not import cursor citations directly; replace each with explicit URL citations already used in the current wiki or newly verified primary sources.
- Some external pages group multiple tools into one page. The current wiki should keep individual software pages as canonical records and use grouped prose in comparison or concept pages.
- The external wiki has empty planned directories (`algorithms/`, `comparisons/`) in the zip listing. Treat those as intent, not content.

## Suggested improvement plan

### Phase 1: Navigation and governance

- Keep expanding [[glossary]] as pages are enriched.
- Keep expanding [[uncertainty-log]] as source-verification questions are found.
- Update [[SCHEMA]] to require `Strengths`, `Limitations`, `Recommended use cases`, and `Uncertainties` for enriched software pages.

### Phase 2: Enrich the highest-traffic pages

- Rewrite the 10 overlapping external/current software pages into the current schema while preserving explicit URLs and frontmatter.
- Start with [[pfss]], [[nf2]], [[pinn-me]], [[sunerf]], and [[mas]] because they already overlap exactly and therefore have the clearest merge path.
- Add compact input/output and limitation tables where they improve scanning.

### Phase 3: Upgrade comparison and concept pages

- Add reader-oriented explanations to [[pfss-tools]], [[nlfff-tools]], [[qsl-tools]], [[dem-tools]], [[solar-wind-tools]], and [[cme-tools]].
- Add workflow paragraphs explaining why tools connect, not only that they are related.
- Keep each comparison page grounded in explicit source URLs and internal links to canonical software pages.

### Phase 4: Source verification pass

- Review all imported scientific claims against primary repositories, papers, or official documentation.
- Mark unresolved claims with `confidence: low` or explicit **Uncertain** notes.
- Append updates to [[log]] after each merge batch.

## Bottom line

The current wiki should remain the canonical base because it has better coverage, provenance, and maintainability. The external wiki is best used as a readability and curation guide: import its section structure, uncertainty discipline, glossary, and explanatory prose after citation conversion and primary-source verification.
