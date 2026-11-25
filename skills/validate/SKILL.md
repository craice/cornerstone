---
description: Cornerstone — run the validation checks for a roadmap phase
argument-hint: "[phase number]"
disable-model-invocation: true
---

Validate phase $ARGUMENTS of ROADMAP.md.

Follow "Validate a phase" in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md. If no phase was given, use the most recent phase in Current State.

Run every check in that phase's Validation section, plus the Validation Checklist in `AGENTS.md`. Report each check as pass, fail or N/A, with evidence. Don't mark the phase complete if anything fails — list what needs fixing.
