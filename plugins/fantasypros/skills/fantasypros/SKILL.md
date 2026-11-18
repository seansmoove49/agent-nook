---
name: fantasypros
description: Answer fantasy football and baseball questions with FantasyPros data through the FantasyPros MCP server. Use when asked about rankings, projections, start/sit, waiver pickups, trades, injuries, or the user's synced fantasy leagues.
---

# FantasyPros

Use the `fantasypros` MCP server tools for all FantasyPros work.

## First use

If the FantasyPros tools report that authentication is needed, tell the user to run `/mcp`, select `fantasypros`, and sign in with their FantasyPros account in the browser (in Codex: `codex mcp login fantasypros`). Never ask for or store tokens.

## Workflow

- **Rankings and research**: use rankings, projections, stats, injury, and news tools; these work on a free account and need no league.
- **The user's teams**: call `get_leagues` first, then pass the league to roster, starter, ownership, matchup, and waiver tools. If no leagues come back, tell the user to sync them at fantasypros.com/myleagues/league-sync.
- **Advice** (start/sit, trade analyzer, trade finder, waiver finder): these need a FantasyPros premium subscription. If a tool reports that premium is required, say so instead of guessing.
- Say which tool or data source an answer came from, and include the expert-consensus numbers behind a recommendation.

## Example prompts

- "Who should I start at flex this week?"
- "Who are the best waiver pickups in my ESPN league, with FAAB bids?"
- "Show the rest-of-season RB rankings."
