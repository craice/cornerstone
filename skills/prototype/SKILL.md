---
description: Cornerstone Phase 3 (optional) — build a minimal, disposable prototype to test the riskiest assumption
argument-hint: "[what to test]"
disable-model-invocation: true
---

Build a Cornerstone prototype to test: $ARGUMENTS

Follow the "Phase 3: Prototype / PoC" prompt in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md and the philosophy in ${CLAUDE_PLUGIN_ROOT}/templates/PROTOTYPE.template.md. Read `SPECIFICATION.md` first.

If nothing to test was given, read the spec and propose the 2-3 riskiest assumptions, then ask which one to test.

Put the files in `prototype/`. Keep it minimal, single-file when possible, with real content. When done, walk the user through the template's Evaluation section and its three possible decisions.
