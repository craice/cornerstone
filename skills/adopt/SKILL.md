---
description: Adopt Cornerstone in a project already in progress — write spec, roadmap and AGENTS.md from the current code
disable-model-invocation: true
---

Adopt Cornerstone in this existing project.

Follow "Adopting Cornerstone Mid-Project" in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md, using the templates in ${CLAUDE_PLUGIN_ROOT}/templates/.

- Read the codebase and any existing docs or AI instruction files (README, CLAUDE.md, AGENTS.md, .cursor/rules) first.
- In SPECIFICATION.md, mark everything you inferred rather than read as an Open Question for the user to confirm.
- Create one document at a time — SPECIFICATION.md, then ROADMAP.md, then AGENTS.md — and wait for approval before the next.

Never overwrite an existing file without asking. If the project already has a CLAUDE.md, offer to add `@AGENTS.md` to it.
