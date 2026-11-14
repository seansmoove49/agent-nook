---
name: rename-session
description: Rename the current chat, conversation, thread, or agent session with a concise, searchable title. Use only when the user explicitly asks to name or rename the current session.
---

# Rename Session

Name the session for future recognition and retrieval.

## Choose the title

Use this structure when practical:

`Specific topic: Outcome or task`

- Prefer four to eight words.
- Put the most distinctive project, person, product, file, feature, or error first.
- After the colon, capitalize the first word and use lowercase for the remaining words except proper nouns and established acronyms.
- Reflect the session's actual outcome, especially when it changed direction after the opening request.
- Preserve useful retrieval terms such as project names, filenames, feature names, and error codes.
- Omit filler such as `help`, `question`, `discussion`, `request`, and `session` unless it is part of the specific subject.
- Include a date only when it distinguishes recurring work.
- Do not include secrets or unnecessarily sensitive information.

Examples:

- `Agent Skills: Portable session renaming`
- `Agent Research: Compare storage and Hermes`
- `VPN Services: Choose best overall`

## Apply the title

Use the safest native mechanism available in the current harness:

1. If the harness exposes a callable tool for renaming the current session, use it.
2. If renaming is available only through a user-entered command, provide the exact command for the user to run.
3. If no rename mechanism is available, provide the proposed title and concise manual instructions.

Never edit internal session databases, metadata files, or application state directly. Do not claim the rename succeeded unless the harness confirms it.

Report `Renamed to: <title>` after confirmed success. Otherwise report `Suggested title: <title>` and the required user action.
