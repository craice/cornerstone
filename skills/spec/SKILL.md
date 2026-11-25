---
description: Cornerstone Phase 2 — generate SPECIFICATION.md from Discovery (add "lite" for the one-page version)
argument-hint: "[lite]"
disable-model-invocation: true
---

Generate the Cornerstone specification. Arguments: $ARGUMENTS

Follow the "Phase 2: Specification" prompt in ${CLAUDE_PLUGIN_ROOT}/PROMPTS.md.

- If the arguments say `lite`, use ${CLAUDE_PLUGIN_ROOT}/templates/SPECIFICATION.lite.template.md. Otherwise use ${CLAUDE_PLUGIN_ROOT}/templates/SPECIFICATION.template.md.
- Base it on `DISCOVERY.md` in the project root if it exists, otherwise on this conversation. If neither covers the 6 Discovery dimensions, say what is missing and suggest `/cornerstone:discovery` first.
- Keep the template's section numbering. List anything undecided under Open Questions instead of inventing an answer.

Save it as `SPECIFICATION.md` in the project root. Never overwrite an existing file without asking. Then ask the user to review it against the Review Checklist in ${CLAUDE_PLUGIN_ROOT}/CORNERSTONE.md (Phase 2).
