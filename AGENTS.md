# AGENTS.md — Guide for AI Agents

You are working in a **research repository**. This file is your contract: read it
fully before acting. It tells you where things live, how to add to the repo, and
what *not* to do. (`CLAUDE.md` is a thin pointer to this file.)

## 1. Orient yourself first

Before doing anything, read in this order:

1. This file (`AGENTS.md`) — rules and map.
2. [`INDEX.md`](INDEX.md) — the live table of contents of all topics.
3. The `README.md` of whatever folder you're about to touch. **Every folder has one.**

Never guess where something lives — `INDEX.md` and per-folder `README.md`s are the
source of truth. If they disagree with reality, fixing them is part of the task.

## 2. The map

| Path | What's there | When to touch it |
|------|--------------|------------------|
| `topics/` | One folder per research topic. The core of the repo. | Adding/expanding a research thread |
| `topics/_TEMPLATE/` | Skeleton to copy for a new topic. | Never edit; only copy |
| `sources/` | Shared reference material: papers, PDFs, link stubs, data pointers | Citing or storing source material |
| `notes/` | Cross-topic notes + `log.md` running journal | Quick captures, ideas spanning topics |
| `experiments/` | Code, notebooks, reproducible runs | Anything executable |
| `meta/` | Conventions, decision records | Changing how the repo itself works |

## 3. How to add a research topic

1. Copy `topics/_TEMPLATE/` → `topics/<short-slug>/` (slug is `lowercase-with-hyphens`).
2. Fill in the new topic's `README.md` (it has a fixed front-matter + section layout).
3. Add one row to [`INDEX.md`](INDEX.md) pointing at it.
4. Keep findings in that topic's `findings.md`; raw working material in `working/`.

## 4. Rules (do / don't)

**Do**
- Keep every new folder self-documenting: add a `README.md` saying what it holds.
- Update `INDEX.md` in the same change that adds a topic. A topic not in the index doesn't exist.
- Use `lowercase-with-hyphens` for files and folders; `YYYY-MM-DD` for dates.
- Cite sources by linking to the file/stub in `sources/`, not by pasting raw URLs inline.
- Prefer Markdown for prose. Keep one idea per file; link liberally between files.
- Leave a dated line in `notes/log.md` when you do meaningful work, so the next agent has a trail.

**Don't**
- Don't dump files in the repo root. Everything belongs under a topic or a top-level folder.
- Don't edit `_TEMPLATE/` — copy it.
- Don't delete or rewrite another contributor's findings; append, annotate, or open a note instead.
- Don't invent structure ad hoc. If a new pattern is needed, record it in `meta/conventions.md` first.

## 5. Conventions

Full list in [`meta/conventions.md`](meta/conventions.md). The essentials are in §4 above.

## 6. When you finish a task

- Confirm `INDEX.md` and the relevant `README.md`s reflect what you changed.
- Add a one-line dated entry to `notes/log.md`.
- Leave the repo in the state these rules describe — the next agent relies on it.
