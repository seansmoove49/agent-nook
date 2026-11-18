# FantasyPros

Bundles FantasyPros' official remote MCP server (`https://api.fantasypros.com/mcp`, HTTP + OAuth) plus a small skill. No API key is needed and no tokens or secrets are stored here.

## Install

```bash
claude plugin marketplace add seansmoove49/agent-nook
claude plugin install fantasypros@agent-nook
```

## Codex

The same plugin ships a Codex/Agent Plugins manifest (`plugin.json`, `mcp.json`). Add this repo as a marketplace in Codex and install `fantasypros`, then sign in with `codex mcp login fantasypros`.

## First use

Start Claude Code, run `/mcp`, choose `fantasypros`, and sign in with your FantasyPros account in the browser. A free account covers rankings, projections and research. Sync your leagues at fantasypros.com/myleagues/league-sync for roster questions; start/sit, trade and waiver advice tools need a premium subscription.

- "Who should I start at flex this week?"
- "Best waiver pickups in my league, with FAAB bids"
- "Rest-of-season WR rankings"

The icon recreates FantasyPros' app icon (`https://www.fantasypros.com/apple-touch-icon.png`) in vector form, using the `f` and `p` glyph paths unmodified from FantasyPros' official logo SVG (`https://images.fantasypros.com/images/branding/fantasypros-fullcolor-light-bg.svg`).
