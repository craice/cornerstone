# [Project Name] — Prototype / Proof of Concept

> Lightweight validation of key ideas before planning execution

*Architecture analogy: This is the study model — a rough maquette to test proportions and concepts. It's not the building; it's a tool for thinking.*

---

## When to Use This Phase

Use prototyping / PoC when:
- You're unsure if a technical or visual approach will work
- You want to test a layout, interaction, flow, or integration before committing
- You need to prove feasibility of a critical path
- You want early feedback on any risky assumption

Skip this phase when:
- Requirements are very clear and well-understood
- The project is too small to justify the extra step
- There's no significant uncertainty to resolve

---

## What It Looks Like

The shape of a prototype depends on the type of project. Pick the approach that matches yours:

| Project Type | What to Build | What to Validate | Example |
|-------------|--------------|-----------------|---------|
| **UI / Website** | Single HTML/CSS file, no JS | Layout, visual direction, content hierarchy, responsive behavior | `prototype/index.html` |
| **API / Backend** | Minimal endpoint + request/response | Data model, auth flow, integration with external services | `prototype/api-test.py` |
| **CLI** | Single script with hardcoded inputs | Command structure, output format, core algorithm | `prototype/cli-test.sh` |
| **Data Pipeline** | Small script with sample data | Data transformations, input/output format, edge cases | `prototype/pipeline-test.py` |

---

## Philosophy

Prototypes and proofs of concept are **sketches in code.** Follow these rules regardless of project type:

- **Minimal tooling** — the simplest possible approach (for UI: pure HTML/CSS; for APIs: a single file; for CLIs: a script)
- **Single file when possible** — keep it contained
- **Static or hardcoded** — don't build real infrastructure; fake what you can
- **Disposable** — meant to be thrown away or heavily rewritten
- **Fast** — should take minutes to an hour, not days
- **Real content** — use actual text and data, not placeholders

For UI projects, this aligns with the [Purissimo](https://craice.github.io/purissimo/) philosophy: pure HTML and CSS, zero JavaScript, maximum clarity.

---

## What to Test

Pick the riskiest or most uncertain parts of SPECIFICATION.md. Don't prototype everything — focus.

### Possible Focus Areas

- [ ] **Layout and structure** — Does the page flow make sense? *(UI)*
- [ ] **Visual direction** — Do the colors, typography, and spacing feel right? *(UI)*
- [ ] **Component design** — Does this card/form/nav work as imagined? *(UI)*
- [ ] **Content hierarchy** — Is the most important information prominent? *(UI)*
- [ ] **Responsive behavior** — Does this work on different screen sizes? *(UI)*
- [ ] **Data model** — Does the structure support the operations needed? *(API/Data)*
- [ ] **Integration** — Does the external service/API work as expected? *(API)*
- [ ] **Command UX** — Is the CLI intuitive? Does the output make sense? *(CLI)*
- [ ] **Data transformation** — Does the pipeline produce correct output? *(Data)*

### What I'm Testing

[Describe the specific question(s) you want this prototype to answer]

1. ...
2. ...

---

## Creating the Prototype

### Prompt

Use the Prototype prompt in [PROMPTS.md](https://github.com/craice/cornerstone/blob/main/PROMPTS.md) (Phase 3: Prototype / PoC).

### Prototype Files

```
prototype/
├── index.html          # Main prototype (UI projects)
├── api-test.[ext]      # API proof of concept (backend projects)
├── cli-test.[ext]      # CLI proof of concept (CLI projects)
├── [variant].[ext]     # Alternative approaches (optional)
└── assets/             # Sample data or static files (if needed)
```

---

## Evaluation

After reviewing the prototype, answer these questions:

### Does It Match the Vision?

- [ ] This looks like what I imagined during Discovery
- [ ] The overall direction feels right
- [ ] I'd be comfortable building on this foundation

### What Needs to Change?

[List anything that feels wrong, surprising, or incomplete]

- ...
- ...

### Specification Updates Needed?

[Does the prototype reveal any changes needed in SPECIFICATION.md?]

- [ ] No changes needed — prototype confirms the spec
- [ ] Yes — the following sections need updating:
  - ...

### Decision

- [ ] **Proceed to Roadmap** — the prototype confirms the vision
- [ ] **Iterate** — create another prototype with adjustments
- [ ] **Loop back to Specification** — significant changes are needed

---

## Notes

[Any observations, insights, or patterns worth saving from the prototyping process]

---

*This file follows the Cornerstone process. For more information, see CORNERSTONE.md. Prompts: [PROMPTS.md](https://github.com/craice/cornerstone/blob/main/PROMPTS.md)*
