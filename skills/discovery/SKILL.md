---
description: Cornerstone Phase 1 — interview across the 6 dimensions and save DISCOVERY.md
argument-hint: "[your idea in 1-2 sentences]"
disable-model-invocation: true
---

Run Cornerstone Discovery for this idea: $ARGUMENTS

Follow the "Phase 1: Discovery" prompt in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md. If no idea was given, ask for it first.

Use ${CLAUDE_PLUGIN_ROOT}/templates/DISCOVERY.template.md as the checklist, including its Discovery Guardrails. Ask one group of questions at a time — never the whole template at once.

When every item in the Discovery Checklist is covered and the user agrees, save the result as `DISCOVERY.md` in the project root. Never overwrite an existing file without asking. Then suggest `/cornerstone:spec` as the next step.
