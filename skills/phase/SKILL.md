---
description: Cornerstone Phase 6 — execute a roadmap phase or a range of tasks
argument-hint: "[phase number, or task range like 2.1-2.4]"
disable-model-invocation: true
---

Execute from ROADMAP.md: $ARGUMENTS

Follow "Execute a phase" (or "Complete specific tasks" for a task range) in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md, and the rules in `AGENTS.md`. If no phase or range was given, use the next step in Current State and confirm it first.

- Mark tasks complete as you go. Never mark a `[human]` task complete — prepare what you can and list it as waiting on the human.
- Record implementation decisions in the AI Decision Log. Stop and ask before any decision that changes scope or contradicts SPECIFICATION.md.
- At the end, update the Execution Log and Current State.
