# [Project Name] — AI Instructions

*Architecture analogy: This is the site preparation — the briefing document the builder receives before breaking ground.*

**Last synced with:** SPECIFICATION.md v1.0 | ROADMAP.md v1.0

> **Sync rule:** This file must be reviewed every time SPECIFICATION.md or ROADMAP.md is updated. Check if principles, references, or key values have shifted. Update the version numbers above after each sync.

---

## Project Overview

[2-3 sentences describing the project. What is it? What's the goal?]

**Key Facts:**
- **Author:** [Name]
- **Type:** [Type of project]
- **Stack:** [Main technologies — brief, see SPECIFICATION.md §4 for details]

## Key Files

| File | Purpose |
|------|---------|
| `SPECIFICATION.md` | Complete project specification — the source of truth |
| `ROADMAP.md` | Phased task list with execution and decision logs |
| `AI.md` | This file — how to work on this project |

**Always read SPECIFICATION.md and ROADMAP.md before starting any work.**

---

## Core Principles

Rules that must never be violated, regardless of context:

1. **[Principle 1]** — [Description]
2. **[Principle 2]** — [Description]
3. **[Principle 3]** — [Description]
4. **[Principle 4]** — [Description]
5. **[Principle 5]** — [Description]

---

## Working Process

### Before Starting a Phase

1. Read SPECIFICATION.md (or relevant sections)
2. Review all tasks for the phase in ROADMAP.md
3. Identify any dependencies or prerequisites
4. Confirm understanding before proceeding

### During Development

1. Follow the specification exactly
2. Complete tasks in order when possible
3. Mark tasks as complete: `- [x] Task description`
4. **Stop and ask** if something is ambiguous — don't guess

### After Completing a Phase

1. Run validation checks
2. Update the Execution Log with date and summary
3. Log any decisions in the AI Decision Log
4. Verify all deliverables exist

### When Something's Wrong

1. Stop and flag the issue
2. Suggest a fix or ask for direction
3. If the spec needs updating, say so explicitly
4. Log the change in the AI Decision Log
5. Continue from where the change matters

---

## Logging Requirements

### Execution Log Format

After completing a phase, add an entry to ROADMAP.md:

```markdown
| Date | Summary |
|------|---------|
| YYYY-MM-DD | Brief description of what was accomplished |
```

### AI Decision Log Format

When making a decision not explicitly defined in specs:

```markdown
| Date | Phase/Task | Decision | Rationale |
|------|------------|----------|-----------|
| YYYY-MM-DD | [Task ID] | [What was decided] | [Why] |
```

### When to Log Decisions

- Choosing between multiple valid approaches
- Specs are ambiguous or incomplete
- Adding something not explicitly defined
- Making performance or compatibility tradeoffs
- Naming something not named in specs
- Changing or deviating from the spec

---

## Validation Checklist

Before considering any phase complete:

- [ ] All tasks for the phase are marked complete
- [ ] [Project-specific validation check 1]
- [ ] [Project-specific validation check 2]
- [ ] [Project-specific validation check 3]
- [ ] Execution Log is updated
- [ ] Decisions are logged (if any were made)

---

## Do's

- ✓ Follow the specification exactly
- ✓ Read context files before every work session
- ✓ Stop and ask when something is unclear
- ✓ Document decisions in the AI Decision Log
- ✓ Validate work before marking complete
- ✓ Flag spec issues instead of guessing

## Don'ts

- ✗ Don't assume — ask
- ✗ Don't skip logging requirements
- ✗ Don't add features not in the specification
- ✗ Don't deviate from naming conventions (see SPECIFICATION.md §4)
- ✗ [Project-specific don't]
- ✗ [Project-specific don't]

---

## Quick Reference

### Commands

**Start work:**
```
Read AI.md, SPECIFICATION.md, and ROADMAP.md.
Confirm you understand the project before proceeding.
```

**Execute a phase:**
```
Execute Phase [N]: [Phase Name] from ROADMAP.md.
Follow SPECIFICATION.md. Mark tasks complete. Update logs.
```

**Specific tasks:**
```
Complete tasks [X.X] through [X.X] from ROADMAP.md.
```

**Validate:**
```
Run validation checks for Phase [N] as defined in the roadmap.
```

### Key Values *(if applicable)*

```
[Include frequently referenced values here for quick access]
[e.g., primary color, main font, base spacing unit]
```

---

## Notes

[Any additional context that helps AI understand the project — things that don't fit elsewhere]

---

*This file follows the Cornerstone process. For more information, see CORNERSTONE.md*
