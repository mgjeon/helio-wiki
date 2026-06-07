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

## [2026-06-07] update | Tune Obsidian graph display
- Adjusted global graph defaults for a cleaner visual overview: hide raw/meta paths and unresolved/orphan nodes by default.
- Added folder-based color groups for ecosystem, concepts, comparisons, and software pages.
- Tuned graph force, node, label, and line settings to reduce visual clutter in the default graph view.

## [2026-06-07] compare | External independently generated wiki archive
- Compared `/Users/mausr/Downloads/wiki.zip` against the current wiki.
- Added [[external-wiki-comparison]] with structural, coverage, citation, and readability findings.
- Identified high-value imports: glossary, uncertainty log, richer software-page sections, and reader-oriented expansions for ecosystem/comparison pages.

## [2026-06-07] update | Seed glossary and uncertainty log
- Added [[glossary]] from the external wiki's onboarding pattern, rewritten with current-wiki internal links.
- Added [[uncertainty-log]] from the external wiki's open-question pattern, rewritten as source-verification tasks.
- Linked both pages from [[README]] and [[index]].

## [2026-06-07] update | Add enriched software-page section guidance
- Updated [[SCHEMA]] with recommended sections for priority software-page enrichment based on the external wiki comparison.

## [2026-06-07] update | Add future agent update guidelines
- Added [[agent-update-guidelines]] based on `/Users/mausr/Downloads/llm-wiki.txt`, [[external-wiki-comparison]], and current [[SCHEMA]] conventions.
- Documented source handling, update workflow, software-page enrichment, uncertainty discipline, lint checks, and completion checklist for future LLM agents.
- Linked the guidelines from [[README]] and [[index]].

## [2026-06-07] update | Create LLM Collaboration and Improvements Hub
- Created [[llm-collaboration-hub]] to coordinate future LLM discussion items, track completed improvements, and define collaboration protocols.
- Linked the new hub page from [[README]] and [[index]].
- Updated total page count catalog in [[index]] to 106.

## [2026-06-07] query | JSOC SHARP pipeline structure and algorithms
- Filed the JSOC SHARP/HARP/HMI vector-field pipeline explanation as [[jsoc-sharp-pipeline-structure]].
- Updated [[index]] with a Queries section and total page count 107.
- Updated [[active-region-parameters]] to link the SHARP pipeline deep dive.
- Recorded the user's standing preference that useful Q&A should update the wiki, all wiki changes should be logged, and completed changes should be committed and pushed.

