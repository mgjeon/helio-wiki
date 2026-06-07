---
title: LLM Collaboration and Improvements Hub
created: 2026-06-07
updated: 2026-06-07
type: summary
tags: [wiki, agent-guidelines, meta, llm-collaboration, improvements]
sources: [/Users/mausr/wiki/agent-update-guidelines.md, /Users/mausr/wiki/comparisons/external-wiki-comparison.md, /Users/mausr/wiki/SCHEMA.md]
confidence: high
---

# LLM Collaboration and Improvements Hub

This hub serves as a central registry and communication center for LLM agents updating the Solar Physics and Space Weather Software Wiki. Since different agents operate across independent sessions with no shared runtime memory, this page is the **canonical record** for tracking planned improvements, discussing wiki structure, and coordinating efforts to build a mature, compounding knowledge base.

---

## 1. LLM Collaboration Protocol

To prevent agents from duplicating work, introducing inconsistencies, or overwriting valuable context, all future LLM sessions must adhere to these rules:

1. **Read First**: At the start of a session, always read this hub alongside [[agent-update-guidelines]], [[SCHEMA]], and [[log]].
2. **Consult Active Discussions**: Check the **Active Improvement Proposals** section below before initiating any major restructurings, file creations, or script/concept migrations.
3. **Contribute to Threads**: If you have insights or want to propose a change, append a comment to the appropriate proposal thread. Use the standard signature format:
   ```markdown
   - **[YYYY-MM-DD] Agent (e.g., Antigravity)**: Proposed comment/rationale.
   ```
4. **Log Completed Changes**: When you resolve a proposal or implement a major improvement, move it (or summarize it) in the **Completed Improvements & Change History** section, and update [[log]].
5. **No Placeholders**: Never introduce empty pages or placeholder text. If a page or section is added, populate it with verified facts and links to primary sources.

---

## 2. Active Improvement Proposals

Future LLM agents should review, update, or resolve the following active discussions:

### `[PROPOSAL-001]` Scientific Context Enrichment over Raw Inspection

* **Status**: Open
* **Context**: Most current `software/` pages contain raw git tree layouts and configuration file names, which serve as proof of inspection but offer little help to heliophysics researchers.
* **Proposed Action**:
  - Transition software pages from raw provenance logs to scientific guides using the enriched schema sections defined in [[SCHEMA]] (Scientific purpose, Methods and algorithms, Inputs/outputs, Strengths, Limitations, Recommended use cases, and Uncertainties).
  - Target priority pages first, such as [[pfsspy]], [[nf2]], [[sunerf]], and [[mas]].
* **Discussion**:
  - **[2026-06-07] Antigravity**: Seeding this proposal. High-traffic pages should prioritize explaining *how* and *why* a tool is used rather than listing `.github/workflows` files.

---

### `[PROPOSAL-002]` Citation Standardization & Verification

* **Status**: Open
* **Context**: The external wiki comparisons show that while the current wiki has strong URL-level citations, some imported content has unresolvable citations. Conversely, maintainer details, Python versions, and licenses might be out of date or inferred.
* **Proposed Action**:
  - Standardize all citations to explicit primary source URLs (repositories, official docs, papers).
  - Perform live verification of repository metadata (license, supported Python versions, active status) before making claims.
  - Do not copy non-portable LLM session-specific citation tokens.
* **Discussion**:
  - **[2026-06-07] Antigravity**: Proposing that any claim marked **Uncertain** must be resolved via primary-source verification and removed from [[uncertainty-log]] once confirmed.

---

### `[PROPOSAL-003]` Enhancing Grouped Concept & Comparison Pages

* **Status**: Open
* **Context**: Grouped pages like [[solar-wind-tools]] and [[cme-tools]] are currently structured as flat lists. They lack reader-oriented narratives comparing algorithms or explaining observation-to-forecasting pipelines.
* **Proposed Action**:
  - Rewrite comparison pages to act as selection guides (e.g., when to choose potential-field PFSS vs. non-linear force-free field NLFFF).
  - Enrich concept pages (e.g., [[ambient-solar-wind-modeling]]) to detail the physics, inputs/outputs, boundary conditions, and where tools sit in the space weather forecasting pipeline.
* **Discussion**:
  - **[2026-06-07] Antigravity**: Initializing the thread. We should merge findings from comparison archives (like `comparisons/external-wiki-comparison.md`) to write comparison summaries that help researchers make decisions.

---

## 3. Completed Improvements & Change History

Track historical changes made to the wiki's structure, guidelines, and metadata below. For individual page updates, refer to the global [[log]].

| Date | Agent | Scope of Change | Affected Pages | Description |
| --- | --- | --- | --- | --- |
| 2026-06-07 | Antigravity | Seeding LLM Collaboration Hub | [[llm-collaboration-hub]], [[README]], [[index]], [[log]] | Established this hub page to log LLM discussions, track improvements, and set rules for multi-session coordination. |

---

*To add new proposal threads or update existing ones, follow the conventions in [[SCHEMA]] and update the table above.*
