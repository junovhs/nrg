# MCP Distribution for AI Coding Agents

- **Slug:** `mcp-distribution-for-coding-agents`
- **Status:** done
- **Owner(s):** Spencer
- **Started:** 2026-06-26
- **Last updated:** 2026-06-26

## Question
What is the lowest-friction way to distribute Ishoo as an MCP server so users
"enable once, then forget it" across Claude Code, Cursor, Codex, and Google's stack?

## Why it matters
Distribution strategy directly determines Ishoo adoption and the install/onboarding
experience across the major AI coding hosts.

## Key questions / sub-threads
- [x] Which hosts have the cleanest third-party distribution surfaces?
- [x] stdio local binary vs. long-lived HTTP daemon?
- [x] How to package per host (plugin / marketplace / deeplink / user-scope config)?

## Current state
Full distribution research report mined from the `ishoo` repo. Recommendation:
install Ishoo once as a per-user local executable, then consume it through each host's
native packaging surface (host-managed plugin/extension launch of a local stdio
server). Cleanest surfaces today: Codex and Cursor. See findings.

## Links
- Findings: [`findings.md`](findings.md)
- Working material: [`working/`](working/) — verbatim source report (dated 2026-06-13)
- Source repo: `../ishoo/docs/archive/research/mcp-research-6-13-26.md`
