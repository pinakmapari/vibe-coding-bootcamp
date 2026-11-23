# Schema: Vibe Coding Bootcamp team wiki

Team wiki for the Imperial Enterprise Lab Vibe Coding Bootcamp (Mon 23, Tue 24, Thu 26 Nov 2026). Pattern: Karpathy's LLM Wiki. The LLM maintains the wiki; the team curates sources and asks questions.

## Layers
- `raw/`: immutable sources (Reddit threads, test notes, screenshots). Never edit these, only add. The handbook PDF is not committed; it lives in the team Drive folder.
- `wiki/`: LLM-owned markdown. `wiki/index.md` is the catalogue, `wiki/log.md` is the append-only history.
- This file: the schema. Update it when a workflow changes.

## Rules for this project
- The handbook is the source of truth for process, schedule and judging.
- Separate **Evidence** (sourced, with link or file in `raw/`) from **Assumptions** (unverified). Label both on every page that makes claims.
- Never invent quotes, research or test results. If it isn't in a source, write "Not stated".
- A quote is only valid if checked word for word against its thread. Record the thread link next to it.
- Scope for v1: one user, one task, one outcome.
- Public repo: no passwords, discount codes, Strategyzer logins, emails or phone numbers. Team members are first names only.

## Page conventions
- Filenames: lowercase-kebab-case.md. Link pages with relative links.
- Start each page with frontmatter: `type` (source | problem | concept | decision | test | admin), `updated` (YYYY-MM-DD), `status` (draft | checked).
- Source pages summarise one raw file and link to it.

## Operations
- **Ingest**: read the source, discuss takeaways with the team, write or update a source page, update affected pages, update `wiki/index.md`, append to `wiki/log.md`.
- **Query**: read `wiki/index.md` first, then the relevant pages. File useful answers back as pages.
- **Lint**: check for contradictions, stale claims, orphan pages, unsourced quotes, and assumptions presented as evidence.

## Log format
`## [YYYY-MM-DD] ingest | query | lint | decision | setup | Title`, then one or two lines.

## Two Lovable projects, two repos
1. Team WIP website (Day 1). This repo holds the wiki only, not the site code.
2. Prototype (Day 2): separate Lovable project and its own repo, to be created after the problem is chosen.
