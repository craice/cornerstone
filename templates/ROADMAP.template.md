# [Project Name] — Development Roadmap

> A phased approach to building [Project Name]

*Architecture analogy: These are the construction documents — detailed blueprints the builder follows.*

---

## Changelog

| Version | Date | What Changed | Why |
|---------|------|-------------|-----|
| 1.0 | [Date] | Initial roadmap | Created from SPECIFICATION.md v1.0 |

*Bump the version when phases or tasks change (not when tasks are checked off). AGENTS.md records which version it was last synced with.*

---

## Current State

*Read this first at the start of every session. Update it at the end of every session.*

| | |
|---|---|
| **Last updated** | [YYYY-MM-DD] |
| **Where we stopped** | [Phase N, task N.N — or "Not started"] |
| **Next step** | [The very next concrete action] |
| **Waiting on the human** | [`[human]` tasks or decisions that block progress — or "Nothing"] |
| **Tried and discarded** | [Approaches that didn't work, so the next session doesn't retry them — or "Nothing"] |

---

## About This Document

This document serves two purposes:

1. **Plan** — A structured list of all tasks required to build [Project Name], organized by phases. Use it to guide AI tools through development.

2. **Record** — A living log of what has been completed. As tasks are finished, mark them with `[x]` and document the work in the [Execution Log](#execution-log).

### How to Use

- **Planning:** Review phases and tasks before starting work
- **Execution:** Reference specific tasks when working with AI (e.g., "Complete task 2.3")
- **Tracking:** Mark tasks as complete and log summaries in the Execution Log
- **Review:** Check the AI Decision Log for decisions made during development
- **Resuming:** Start every session from [Current State](#current-state)

### Task Markers

| Marker | Meaning |
|--------|---------|
| `- [ ] **1.1** ...` | Task for the AI (or anyone) |
| `- [ ] **1.2** [human] ...` | Only a human can do it — deploys, accounts, payments, publishing, real-world actions. The AI prepares what it can but never marks it complete |

---

## Overview

| Attribute | Value |
|-----------|-------|
| **Total Phases** | [N] |
| **Total Tasks** | [N] |
| **Estimated Effort** | [Time estimate or "Flexible"] |

---

## Progress Summary

- [ ] Phase 1: [Phase Name]
- [ ] Phase 2: [Phase Name]
- [ ] Phase 3: [Phase Name]

*Add or remove phases as your project requires. There is no "right" number.*

---

## Phase 1: [Phase Name]

**Goal:** [One sentence describing the objective]

### Tasks

- [ ] **1.1** [Task description]
- [ ] **1.2** [Task description]
- [ ] **1.3** [Task description]
- [ ] **1.4** [Task description]
- [ ] **1.5** [human] [Task only a human can do, if any]

### Deliverables

- [What should exist when this phase is complete]
- ...

### Validation

*Check each applicable category. Not all categories apply to every phase — mark N/A where irrelevant.*

**Functional:**
- [ ] [Features work as specified in SPECIFICATION.md]
- [ ] [Edge cases handled]

**Visual:** *(if applicable)*
- [ ] [UI matches design tokens / spec requirements]
- [ ] [Responsive behavior verified]

**Technical:**
- [ ] [No regressions introduced]
- [ ] [Code follows project conventions]

**Documentation:**
- [ ] Execution Log updated
- [ ] Decisions logged (if any were made)

---

## Phase 2: [Phase Name]

**Goal:** [One sentence describing the objective]

### Tasks

- [ ] **2.1** [Task description]
- [ ] **2.2** [Task description]
- [ ] **2.3** [Task description]
- [ ] **2.4** [Task description]
- [ ] **2.5** [Task description]

### Deliverables

- ...

### Validation

**Functional:**
- [ ] ...

**Visual:** *(if applicable)*
- [ ] ...

**Technical:**
- [ ] ...

**Documentation:**
- [ ] Execution Log updated
- [ ] Decisions logged (if any were made)

---

## Phase 3: [Phase Name]

**Goal:** [One sentence describing the objective]

### Tasks

- [ ] **3.1** [Task description]
- [ ] **3.2** [Task description]
- [ ] **3.3** [Task description]
- [ ] **3.4** [Task description]
- [ ] **3.5** [Task description]

### Deliverables

- ...

### Validation

**Functional:**
- [ ] ...

**Visual:** *(if applicable)*
- [ ] ...

**Technical:**
- [ ] ...

**Documentation:**
- [ ] Execution Log updated
- [ ] Decisions logged (if any were made)

---

*Add more phases as needed. A small project might have 3 phases; a complex one might have 10. Each phase should be completable in roughly one work session and have a clear, verifiable outcome.*

---

## Task Summary

| Phase | Name | Tasks | Focus |
|-------|------|-------|-------|
| 1 | [Name] | [N] | [Brief description] |
| 2 | [Name] | [N] | [Brief description] |
| 3 | [Name] | [N] | [Brief description] |
| **Total** | | **[N]** | |

---

## Using This Roadmap with AI

Prompts for starting, executing, validating, and ending sessions are in [PROMPTS.md](https://github.com/craice/cornerstone/blob/main/PROMPTS.md) (Phase 6: Execution).

---

## Execution Log

A summary of what was accomplished in each phase, recorded as work is completed.

### Phase 1: [Phase Name]

| Date | Summary |
|------|---------|
| | |

### Phase 2: [Phase Name]

| Date | Summary |
|------|---------|
| | |

### Phase 3: [Phase Name]

| Date | Summary |
|------|---------|
| | |

---

## AI Decision Log

Implementation decisions made by AI tools during development. This log documents the AI's reasoning and allows for human review.

> Product and scope decisions don't go here — they go in the Decision Log in SPECIFICATION.md, after the human approves them.

| Date | Phase/Task | Decision | Rationale |
|------|------------|----------|-----------|
| | | | |
| | | | |
| | | | |

### What to Log

- Choices between multiple valid approaches
- Resolutions of ambiguities in the specification
- Additions not explicitly defined in specs
- Performance or compatibility tradeoffs
- Naming decisions for undefined elements

---

*Last updated: [Date]*
*This file follows the Cornerstone process. For more information, see CORNERSTONE.md. Prompts: [PROMPTS.md](https://github.com/craice/cornerstone/blob/main/PROMPTS.md)*
