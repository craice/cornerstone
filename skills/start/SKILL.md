---
description: Run the whole Cornerstone kick-off — Discovery, then SPECIFICATION.md, ROADMAP.md and AGENTS.md
argument-hint: "[your idea in 1-2 sentences]"
disable-model-invocation: true
---

Run the Cornerstone process for this idea: $ARGUMENTS

Follow the "One-Prompt Kick-off" in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md. If no idea was given, ask for it first.

Use the templates in ${CLAUDE_PLUGIN_ROOT}/templates/ for each document and save them in the project root without the `.template` suffix (`DISCOVERY.md`, `SPECIFICATION.md`, `ROADMAP.md`, `AGENTS.md`). Never overwrite an existing file without asking.

Move to the next document only after the user approves the current one. The process is described in ${CLAUDE_PLUGIN_ROOT}/CORNERSTONE.md.
