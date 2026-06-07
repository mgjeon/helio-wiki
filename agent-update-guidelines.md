---
title: Agent Update Guidelines
created: 2026-06-07
updated: 2026-06-07
type: summary
tags: [solar-physics, space-weather, wiki, agent-guidelines, documentation]
sources: [/Users/mausr/Downloads/llm-wiki.txt, comparisons/external-wiki-comparison.md, SCHEMA.md, log.md]
confidence: high
---

# Agent Update Guidelines

These guidelines are for future LLM agents updating this wiki. Treat the wiki as a persistent, compounding knowledge base, not as a temporary answer cache. Each update should make future answers easier, more accurate, and less dependent on rediscovering the same source material.

## Operating model

- Raw sources are the source of truth. Preserve files under `raw/` and do not rewrite source transcripts.
- The wiki is the compiled knowledge layer. Update existing pages when new information changes the synthesis; do not only add isolated summaries.
- [[SCHEMA]] defines page conventions, frontmatter, tags, confidence, source citation, and software-page structure.
- [[index]] is the content catalog. Keep it current so future agents can navigate without reading every file.
- [[log]] is the chronological memory. Append an entry for every ingest, comparison, lint, or substantial update.
- [[uncertainty-log]] is the queue of open verification work. Add to it when a claim is useful but not yet settled.

## First moves in a new update session

1. Read [[README]], [[index]], [[SCHEMA]], and the latest entries in [[log]].
2. Search for existing pages before creating new ones.
3. Check [[external-wiki-comparison]] when enriching software pages; it identifies the readability gap between the current wiki and the independently generated wiki.
4. Use [[glossary]] to normalize recurring terminology.
5. If a claim seems stale, contested, or inferred, verify it from a primary source before presenting it as fact.

## Source handling

- Prefer primary sources: official repositories, official documentation, official project pages, and peer-reviewed papers.
- Keep raw source lists and transcripts immutable.
- Use explicit URLs in citations. Do not import non-portable citation tokens from another LLM session.
- When importing from `/Users/mausr/Downloads/wiki.zip` or similar generated artifacts, treat the artifact as a writing and organization aid, not as authority.
- For repository metadata such as license, maintainer, active status, supported Python versions, or installation method, verify against the current repository before updating the page.

## Page update workflow

When ingesting or improving a source:

1. Identify canonical pages affected by the source: software, concept, comparison, ecosystem, glossary, and uncertainty pages.
2. Update the relevant existing pages before creating new pages.
3. Add or revise internal links so the knowledge is discoverable from multiple routes.
4. Preserve useful older claims if a new source conflicts with them; mark the conflict with source dates and lower confidence where needed.
5. Update [[index]] with new pages or materially changed page roles.
6. Append [[log]] with what changed and why.
7. Run a wikilink check if new links or pages were added.

## Software page enrichment

Many current software pages are strong provenance records but thin as researcher-facing explanations. For priority pages, expand beyond repository inspection notes using the enriched sections in [[SCHEMA]]:

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

Prioritize pages named in [[external-wiki-comparison]]: [[pfss]], [[pfsspy]], [[sunkit-magex]], [[nf2]], [[pinn-me]], [[sunerf]], [[mas]], [[hux]], [[huxt]], [[dbm]], [[demreg]], [[demregpy]], [[fastqsl]], [[fastqsl2]], [[ufit]], [[oft]], [[swig]], [[mapflpy]], [[chmap]], [[psi-io]], and [[pyvisual]].

## Comparison and concept pages

- Comparison pages should help a researcher choose between tools, not merely list them.
- Concept pages should explain the scientific problem, common inputs, outputs, assumptions, and where software fits in the workflow.
- If a generated external wiki has good prose for a grouped topic, merge the useful structure into current concept or comparison pages after replacing citations with explicit primary sources.
- Keep individual software pages as canonical homes for tool-specific facts.

## Uncertainty discipline

- Use **Uncertain** inline when a claim is plausible but not verified.
- Add durable open questions to [[uncertainty-log]] instead of leaving uncertainty only in chat history.
- Record what would resolve the uncertainty: repository file, paper, benchmark, official documentation, or expert confirmation.
- Do not overstate maintenance status, operational readiness, scientific validation, or recommended use cases.

## Lint and health checks

Periodically check for:

- Broken or unresolved Obsidian-style internal links.
- Orphan pages that should be linked from [[index]], concept pages, or comparison pages.
- Software pages with only technical inspection notes and no use-case framing.
- Duplicate pages covering the same tool under different slugs.
- Claims about version, status, license, or installation that may have changed.
- Concepts mentioned repeatedly but lacking a page or glossary entry.
- Open questions in [[uncertainty-log]] that have since been resolved.

## Good update shape

A high-quality update usually touches more than one page:

- A source summary or software page captures local detail.
- A concept page absorbs the broader implication.
- A comparison page updates selection guidance.
- [[glossary]] gains or refines terms if needed.
- [[uncertainty-log]] records unresolved questions.
- [[index]] and [[log]] make the change findable and auditable.

## Anti-patterns

- Creating a new summary page while leaving related canonical pages stale.
- Copying another LLM's prose with unverifiable citations.
- Treating repository file listings as enough for a mature software page.
- Adding broad claims like "active", "maintained", "best", or "production-ready" without current primary-source evidence.
- Letting useful analysis remain only in the chat instead of filing it back into the wiki.
- Adding links without checking that they resolve.

## Completion checklist

Before finishing an update session:

- Relevant pages updated, not just new pages added.
- Explicit source URLs included for factual claims.
- [[index]] updated if page inventory or navigation changed.
- [[log]] appended with the action.
- [[uncertainty-log]] updated for unresolved questions.
- No unresolved wikilinks introduced.
