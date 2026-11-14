---
name: agent-research
description: Research AI agents, harnesses, memory, skills, and related tooling, then preserve the findings as retrieval-friendly Markdown in the repository's research directory. Use when asked to investigate or save agent research.
---

# Agent Research

Create evidence-backed research that future agents can find and reuse.

## Store the research

- Use the repository-root `research/` directory.
- Search existing research first. Update the relevant living document instead of creating a duplicate.
- Name living documents `<subject>-<scope>.md` using lowercase words and single hyphens, such as `hermes-agent-evaluation.md`.
- Use a leading `YYYY-MM-DD-` only for immutable experiments or snapshots.
- Avoid vague names such as `notes.md`, `findings.md`, or numbered research files.

Start each document with:

```yaml
---
title: Natural-language title
description: One sentence explaining when this research is relevant.
keywords: [useful, search, terms]
status: active
last_verified: YYYY-MM-DD
---
```

Lead with the conclusion, distinguish evidence from inference, cite primary sources near the claims they support, and record unresolved questions. Update `research/README.md` with a link and one-line retrieval description.

Keep raw research here. Move only stable, reusable procedures into a skill.
