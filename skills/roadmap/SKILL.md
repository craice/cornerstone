---
description: Cornerstone Phase 4 — break SPECIFICATION.md into ROADMAP.md with phases, tasks and Current State
disable-model-invocation: true
---

Generate the Cornerstone roadmap.

Follow the "Phase 4: Roadmap" prompt in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md, using ${CLAUDE_PLUGIN_ROOT}/templates/ROADMAP.template.md. Read `SPECIFICATION.md` first; if it doesn't exist, suggest `/cornerstone:spec`.

- Mark every task only a human can do (deploys, accounts, payments, publishing) with `[human]`.
- Fill in the Changelog (v1.0) and Current State. Leave the Execution Log and AI Decision Log empty.
- Follow "Good Phase Design" in ${CLAUDE_PLUGIN_ROOT}/CORNERSTONE.md (Phase 4).

Save it as `ROADMAP.md` in the project root. Never overwrite an existing file without asking.
