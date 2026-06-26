# Conventions

The rules that keep this repo navigable. If you need a pattern that isn't here,
add it here first, then use it.

## Naming
- Folders and files: `lowercase-with-hyphens` (e.g. `solar-storage-costs/`).
- Dates: `YYYY-MM-DD`, always.
- Slugs are short — a few words at most.

## Structure
- **Every folder has a `README.md`** stating what it contains and how it's organized.
- Research lives under `topics/<slug>/`. Nothing topic-specific goes in the repo root.
- One idea per file. Prefer many small linked Markdown files over one giant document.
- Use relative Markdown links between files so navigation works on GitHub and locally.

## Topics
- Start one by copying `topics/_TEMPLATE/`.
- Each topic has: `README.md` (overview + status), `findings.md` (what we've learned),
  and `working/` (raw notes, drafts, scratch).
- Register every topic in `INDEX.md`. Keep its `Status` column current.

## Sources
- Store reference material in `sources/`. For web sources that can't be saved,
  create a small `.md` stub with title, URL, date accessed, and a one-line summary.
- Reference sources by linking to them, not by pasting raw URLs into prose.

## Logging
- `notes/log.md` is a reverse-chronological journal. Add a dated bullet after
  meaningful work so the next person (or agent) can pick up the thread.

## Decisions
- Non-obvious choices about the repo or research direction go in `meta/decisions.md`
  as short dated entries.
