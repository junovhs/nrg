# Findings — MCP Distribution for AI Coding Agents

Source report (verbatim): [`working/mcp-distribution-research-2026-06-13.md`](working/mcp-distribution-research-2026-06-13.md), mined from the `ishoo` repo.

## Install once locally, consume through each host's native packaging surface
- **What:** The lowest-friction strategy is neither "teach users to edit MCP config" nor "make Ishoo where work starts." Install Ishoo once as a per-user local executable, then let each host consume it via its native surface — plugin, marketplace, deeplink, extension, or user-scope config — so the user stays inside their host.
- **Evidence / source:** [`working/mcp-distribution-research-2026-06-13.md`](working/mcp-distribution-research-2026-06-13.md)
- **Confidence:** high
- **Date:** 2026-06-26

## Cleanest distribution surfaces: Codex and Cursor
- **What:** Codex and Cursor have the cleanest current third-party distribution surfaces. Claude Code is very workable via plugins or skills-directory discovery (instead of project `.mcp.json`). Google Antigravity supports one-click install + plugin packaging, but its public third-party story is less explicit.
- **Evidence / source:** [`working/mcp-distribution-research-2026-06-13.md`](working/mcp-distribution-research-2026-06-13.md)
- **Confidence:** medium
- **Date:** 2026-06-26

## Ship a stable local stdio binary; avoid a manual daemon / open HTTP port
- **What:** Prefer host-managed plugin/extension launch of a local stdio server. Ship a stable `ishoo-mcp` binary and point every host adapter at it, rather than asking users to run a daemon or opening a long-lived local HTTP port unless a host specifically benefits from HTTP.
- **Evidence / source:** [`working/mcp-distribution-research-2026-06-13.md`](working/mcp-distribution-research-2026-06-13.md)
- **Confidence:** high
- **Date:** 2026-06-26
