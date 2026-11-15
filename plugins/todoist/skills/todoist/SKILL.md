---
name: todoist
description: Manage the user's Todoist tasks, projects, and labels through the Todoist MCP server. Use when asked to add, list, find, update, reschedule, or complete Todoist tasks.
---

# Todoist

Use the `todoist` MCP server tools for all Todoist work.

## First use

If the Todoist tools report that authentication is needed, tell the user to run `/mcp`, select `todoist`, and sign in with their Todoist account in the browser. Never ask for or store tokens.

## Workflow

- **Add**: create the task with a clear title; pass natural-language due dates (such as "tomorrow 9am") and the project or labels the user named.
- **List today**: filter for `today | overdue` and show title, project, and due time.
- **Complete**: find the task first; if several match, ask which one before completing.
- **Update or reschedule**: confirm the matched task, then change only the requested fields.
- Confirm before deleting anything. Summarize what changed afterwards.

## Example prompts

- "Add a task to call the dentist tomorrow at 9am in Personal."
- "What's on my Todoist today?"
- "Mark 'send invoice' as done."
