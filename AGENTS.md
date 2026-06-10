@C:\Users\mgjeon\.codex\RTK.md

# Helio Wiki Agent Instructions

This repository is a persistent solar physics and space weather wiki. Treat user questions and answers in this workspace as part of the wiki maintenance workflow, not as throwaway chat.

## First Principles

- Answer from the wiki first. Before giving a substantive answer, search the existing Markdown pages for relevant concepts, software, prior Q&A, and uncertainty notes.
- If the wiki is missing important context that emerges during the conversation, update the appropriate wiki page before finishing.
- If no existing page fits, create or update a page under the closest folder: `concepts/`, `software/`, `comparisons/`, `queries/`, or `ecosystem/`.
- Preserve source material under `raw/`; do not rewrite transcripts or original source captures.
- Follow `SCHEMA.md`, `agent-update-guidelines.md`, and `llm-collaboration-hub.md` for page structure, confidence, citations, and update style.

## Question Answering Workflow

1. Search the wiki for relevant pages and prior notes.
2. Use the stored wiki content as the baseline for the answer.
3. If a claim is current, high-stakes, stale, or not covered by the wiki, verify it from primary sources when needed.
4. Answer the user clearly, including uncertainty where appropriate.
5. Update the wiki when the answer adds reusable knowledge, resolves uncertainty, clarifies a recurring distinction, or records a user preference.
6. Append `log.md` for every wiki update, including Q&A-derived updates.
7. Commit and push completed wiki changes.

## Wiki Update Rules

- Prefer improving existing canonical pages over creating isolated notes.
- Add internal links so new knowledge is discoverable from `index.md`, related concept pages, comparison pages, and query pages.
- Update `index.md` when adding pages or materially changing page roles.
- Update `uncertainty-log.md` when a useful claim remains unresolved.
- Keep entries concise but durable: future agents should understand what changed and why without rereading the whole chat.

## Log Requirement

Every meaningful wiki action must append `log.md` using this format:

```markdown
## [YYYY-MM-DD] action | subject
- What changed.
- Why it changed.
- Related pages updated.
```

Use the local current date. The log is append-only.

## Git Requirement

After completing wiki updates:

1. Inspect `git status`.
2. Stage only files changed for the current task.
3. Commit with a concise message.
4. Push the branch to the configured remote.

Do not stage or revert unrelated user changes. If unrelated local modifications are present, leave them untouched.

## Command Requirement

Follow the repository's RTK instruction: prefix shell commands with `rtk`.
