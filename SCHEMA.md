# Wiki Schema

## Domain
Solar physics and space weather software: magnetic-field modeling, coronal/heliospheric modeling, solar-wind and CME forecasting, differential emission measure analysis, active-region parameters, data access, and supporting visualization/analysis tools.

## Conventions
- File names: lowercase, hyphenated slugs.
- Human/LLM-facing pages live in `software/`, `entities/`, `concepts/`, `comparisons/`, and `queries/`.
- Raw source lists are immutable under `raw/transcripts/` with sha256 frontmatter.
- Every wiki page has YAML frontmatter with title, dates, type, tags, and sources.
- Every claim should cite a source URL inline; unresolved ambiguity is marked **Uncertain**.
- Use Obsidian-style double-bracket internal cross-references between pages (for example, link to a page by its slug).
- Update `index.md` and append `log.md` for every ingest.

## Frontmatter
```yaml
---
title: Page Title
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: software | entity | concept | comparison | query | summary
tags: [solar-physics, space-weather]
sources: [https://example.com]
confidence: high | medium | low
---
```

## Tag Taxonomy
- Domain: solar-physics, space-weather, heliophysics, solar-wind, cme, corona, heliosphere, active-region, magnetic-field, dem
- Methods: pfss, mhd, nlfff, neural-field, pinn, nerf, qsl, field-line-tracing, flux-transport, drag-based-model, gcs, cone-model, flux-rope, forecasting, validation, visualization
- Data: jsoc, gong, hmi, mdi, magnetogram, in-situ, remote-sensing, hapi
- Software: python, fortran, idl, matlab, c-plus-plus, package, library, simulation, data-access, documentation, repository
- Quality: uncertain, inactive, maintained, research-code

## Page Thresholds
- Create a `software/` page for every inspected URL that is software, a repository, a data portal, or a model/tool page.
- Create concept pages for model families and scientific workflows recurring across sources.
- Prefer concise pages with source-backed bullets over long prose.

## Update Policy
When a source conflicts with an existing page, preserve both statements with dates/source URLs and mark the page `contested: true` or `confidence: low`.
