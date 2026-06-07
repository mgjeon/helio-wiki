---
title: Wiki Log
created: 2026-06-07
updated: 2026-06-07
type: summary
tags: [solar-physics, space-weather, log]
sources: []
confidence: high
---

# Wiki Log

> Chronological record of all wiki actions. Append-only.
> Format: `## [YYYY-MM-DD] action | subject`

## [2026-06-07] create | Solar physics and space weather software wiki initialized
- Ingested source lists from user-provided text documents.
- Inspected 76 unique URLs/repositories using git tree/README sampling for GitHub repositories and HTML retrieval for web pages.
- Created 76 software pages and 10 concept pages.
- Raw source lists saved under `raw/transcripts/` with sha256 frontmatter.
- Inspection metadata saved to `_meta/source-inspection.json`.

## [2026-06-07] update | Add repository README landing page
- Created `README.md` as the git/Obsidian landing page.
- Updated `index.md` page count to include README.
- Patched `SCHEMA.md` wording to avoid a non-page example being parsed as a broken wikilink.

## [2026-06-07] update | Resolve partial web retrieval issues
- Rechecked NOAA SWPC real-time solar wind and WSA-ENLIL pages with `curl --tlsv1.2` and updated their software pages from low to medium confidence.
- Rechecked DeepWiki JSOC-SDP/proj with `curl -L` and updated the page with canonical retrieval details.
- Added arXiv and CentAUR fallback sources for the ScienceDirect CME propagation review, which remained blocked by HTTP 403.

## [2026-06-07] verify | Heliosphere wiki polish pass
- Confirmed that the two heliosphere source lists contain 89 URL mentions and 76 unique URLs, all represented in `_meta/source-inspection.json` and Markdown pages.
- Confirmed zero missing Obsidian wikilink targets after audit.
- Added ecosystem overview, taxonomy, workflow map, and comparison pages for PFSS/NLFFF/QSL/DEM/CME/solar-wind groupings.
- Added frontmatter to root summary pages so the wiki conforms to `SCHEMA.md`.

## [2026-06-07] update | Obsidian graph polish
- Set the default graph filter to hide `raw/` transcript files so concept and software pages dominate the initial graph view.
- Removed a local Markdown link to `pyproject.toml` that created a non-knowledge unresolved node in Obsidian.
- Corrected a malformed POT3D URL in the SWiG page and linked the index back to the README landing page.
