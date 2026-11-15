# Todoist

Bundles Todoist's official remote MCP server (`https://ai.todoist.net/mcp`, HTTP + OAuth) plus a small skill. No tokens or secrets are stored here.

## Install

```bash
claude plugin marketplace add seansmoove49/agent-nook
claude plugin install todoist@agent-nook
```

## Codex

The same plugin ships a Codex/Agent Plugins manifest (`plugin.json`, `mcp.json`). Add this repo as a marketplace in Codex and install `todoist`; Codex handles the Todoist sign-in.

## First use

Start Claude Code, run `/mcp`, choose `todoist`, and sign in via the browser. Then try:

- "Add a task to call the dentist tomorrow at 9am"
- "List my tasks for today"
- "Complete the 'send invoice' task"
