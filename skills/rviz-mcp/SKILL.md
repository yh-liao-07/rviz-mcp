---
name: rviz-mcp
description: >
  RViz2 displays, fixed frame, views (mock + live). CLI `rviz-mcp` + MCP stdio serve. Use when the user mentions
  rviz-mcp, /rviz-mcp, or related domain work. One-command Grok install from GitHub.
metadata:
  short-description: "RViz2 displays, fixed frame, views (mock + live)."
---

# rviz-mcp

## One-command install (Grok)

```bash
pip install "git+https://github.com/mergeos-bounties/rviz-mcp.git" && grok plugin install mergeos-bounties/rviz-mcp --trust
```

Or plugin first, then package:

```bash
grok plugin install mergeos-bounties/rviz-mcp --trust
pip install "git+https://github.com/mergeos-bounties/rviz-mcp.git"
```

Verify:

```bash
rviz-mcp version
rviz-mcp doctor
rviz-mcp demo
rviz-mcp serve   # MCP stdio for hosts
```

## Modes

| Env | Values |
| --- | --- |
| `RVIZ_MCP_MODE` | `mock` (default) · `live` |

## MCP

```bash
rviz-mcp serve
```

Config ships in plugin `.mcp.json`. Manual: see repo `examples/`.
