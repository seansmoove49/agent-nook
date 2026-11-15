---
name: new-session
description: Start a new agent session for a task in a specific project so it appears under that project in the sidebar. Use only when the user explicitly asks to create, start, or spin off a new session.
---

# New Session

Start a separate session for a task and make sure it is filed under the right project.

## Steps

1. Identify the project folder as an absolute path. If it is unclear, ask.
2. Write a self-contained brief: the task, the files or area, and what done looks like. The new session does not see this conversation.
3. Start the session in that folder.
4. Confirm it shows under the project in the sidebar. Fix it if not.

## Claude-specific (Claude desktop app)

This workflow depends on Claude's session tools and does not apply to other harnesses.

- Start it with `start_session`: `initiation: "user_asked"`, `context: "fresh"`, `cwd` set to the project folder, plus `title`, `prompt`, and `background`.
- A session started this way nests under the session that started it, so it does not appear under the project. Call `detach_session` with its id to move it to top level. Detaching cannot be undone and stops the parent from being notified when it finishes.
- Verify with `get_session`: `cwd` should be the project folder and `parentSessionId` should be gone or `detached` true.
- Link the session in your reply by its title and id.

If the harness has no session tools, say so and tell the user how to start the session manually.
