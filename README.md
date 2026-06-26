# nrg — Research Repository

A shared research workspace. The structure here is deliberately optimized so that
**both humans and AI agents** can navigate it quickly and contribute consistently.

> New here? If you're an AI agent, read **[`AGENTS.md`](AGENTS.md)** first.
> If you're a human, skim this README, then the same `AGENTS.md` for conventions.

## What this repo is for

Capturing, organizing, and developing research — sources, notes, experiments,
and write-ups — in a way that stays legible as it grows.

## Layout

```
nrg/
├── README.md          ← you are here (human entry point)
├── AGENTS.md          ← machine entry point: rules + map for AI agents
├── INDEX.md           ← live table of contents, updated as topics are added
├── topics/            ← one folder per research topic (the heart of the repo)
│   └── _TEMPLATE/     ← copy this to start a new topic
├── sources/           ← shared reference material (papers, PDFs, links, datasets)
├── notes/             ← cross-topic notes, ideas, and a running log
├── experiments/       ← code, notebooks, and reproducible runs
└── meta/              ← conventions, decisions, and repo-keeping docs
```

## Quick start

- **Start a new topic:** copy `topics/_TEMPLATE/` to `topics/<short-slug>/`, fill in its `README.md`, and add a line to `INDEX.md`.
- **Drop a source:** put the file (or a link stub) in `sources/` and reference it from the relevant topic.
- **Jot something quick:** add to `notes/log.md` with a date.

## Conventions in one breath

Folder + file names are `lowercase-with-hyphens`. Every folder has a `README.md`
explaining what's inside. Markdown for prose. Dates are `YYYY-MM-DD`. See
[`meta/conventions.md`](meta/conventions.md) for the full list.

## Contributors

- **Spencer** (junovhs@gmail.com)
- **Tim**
