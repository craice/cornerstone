---
description: Cornerstone Phase 5 — create AGENTS.md, the behavioral guide AI tools read automatically
disable-model-invocation: true
---

Generate the Cornerstone AI instructions.

Follow the "Phase 5: Setup" prompt in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md, using ${CLAUDE_PLUGIN_ROOT}/templates/AGENTS.template.md. Read `SPECIFICATION.md` and `ROADMAP.md` first.

- Reference the spec by section number instead of copying its content.
- Set "Last synced with" to the current versions of SPECIFICATION.md and ROADMAP.md.
- Remove the Tool Compatibility section from the result.

Save it as `AGENTS.md` in the project root. Never overwrite an existing file without asking.

Then check for a `CLAUDE.md`, `.claude/CLAUDE.md` or `CLAUDE.local.md` in the project. If one exists, Claude Code reads it instead of AGENTS.md: offer to add the line `@AGENTS.md` to it. If none exists, nothing else is needed.
