# [Project Name] — AI Instructions

*Architecture analogy: This is the site preparation — the briefing document the builder receives before breaking ground.*

**Last synced with:** SPECIFICATION.md v1.0 | ROADMAP.md v1.0

> **Sync rule:** This file must be reviewed every time SPECIFICATION.md or ROADMAP.md changes version. Check if principles, references, or key values have shifted. Update the version numbers above after each sync.

> **Why AGENTS.md:** It is the shared convention that AI coding tools read automatically at the start of every session, so the instructions apply without being asked. For tools that read their own file, add a one-line pointer instead of a copy — see [Tool Compatibility](#tool-compatibility) at the end.

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
| `ROADMAP.md` | Current state, phased tasks, execution and decision logs |
| `AGENTS.md` | This file — how to work on this project |

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

### Starting a Session

1. Read SPECIFICATION.md (or relevant sections) and ROADMAP.md
2. Read **Current State** in ROADMAP.md — it says where the last session stopped
3. Confirm the next step before proceeding

### Before Starting a Phase

1. Review all tasks for the phase in ROADMAP.md
2. Identify any dependencies or prerequisites
3. Confirm understanding before proceeding

### During Development

1. Follow the specification exactly
2. Complete tasks in order when possible
3. Mark tasks as complete: `- [x] Task description`
4. **Stop and ask** if something is ambiguous — don't guess
5. **Never mark a `[human]` task as complete.** Prepare what you can, then list it in Current State as waiting on the human

### After Completing a Phase

1. Run validation checks
2. Update the Execution Log with date and summary
3. Log any decisions (see [Logging Requirements](#logging-requirements))
4. Verify all deliverables exist

### Ending a Session

Update **Current State** in ROADMAP.md: where you stopped, the next step, what is waiting on the human, and anything tried and discarded.

### When Something's Wrong

1. Stop and flag the issue
2. Suggest a fix or ask for direction
3. If the spec needs updating, say so explicitly — the human approves spec changes
4. Log the change in the right Decision Log
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

### Where Decisions Go

There are two decision logs. Each has one job:

| Log | Lives in | What goes there | Who decides |
|-----|----------|-----------------|-------------|
| **Decision Log** | SPECIFICATION.md (Appendix) | Product and scope decisions — what the project is, what's in or out | The human |
| **AI Decision Log** | ROADMAP.md | Implementation decisions made during execution | The AI, reviewed by the human |

If an implementation decision changes scope or contradicts the spec, it is no longer an implementation decision: stop, ask, and record it in the spec's Decision Log once approved.

### AI Decision Log Format

```markdown
| Date | Phase/Task | Decision | Rationale |
|------|------------|----------|-----------|
| YYYY-MM-DD | [Task ID] | [What was decided] | [Why] |
```

### When to Log in the AI Decision Log

- Choosing between multiple valid approaches
- Resolving an ambiguity in the spec
- Adding something not explicitly defined
- Making performance or compatibility tradeoffs
- Naming something not named in specs

---

## Validation Checklist

Before considering any phase complete:

- [ ] All tasks for the phase are marked complete (except `[human]` tasks)
- [ ] [Project-specific validation check 1]
- [ ] [Project-specific validation check 2]
- [ ] [Project-specific validation check 3]
- [ ] Execution Log is updated
- [ ] Decisions are logged (if any were made)
- [ ] Current State is updated

---

## Do's

- ✓ Follow the specification exactly
- ✓ Start every session from Current State
- ✓ Stop and ask when something is unclear
- ✓ Log decisions in the right log
- ✓ Validate work before marking complete
- ✓ Flag spec issues instead of guessing

## Don'ts

- ✗ Don't assume — ask
- ✗ Don't skip logging requirements
- ✗ Don't add features not in the specification
- ✗ Don't mark `[human]` tasks as done
- ✗ Don't deviate from naming conventions (see SPECIFICATION.md §4)
- ✗ [Project-specific don't]
- ✗ [Project-specific don't]

---

## Key Values *(if applicable)*

```
[Include frequently referenced values here for quick access]
[e.g., primary color, main font, base spacing unit]
```

---

## Notes

[Any additional context that helps AI understand the project — things that don't fit elsewhere]

---

## Tool Compatibility

Most AI coding tools read `AGENTS.md` automatically. When a tool reads its own file instead, create a pointer — never a copy, or the two will drift apart:

| Tool | File | Content |
|------|------|---------|
| Claude Code | `CLAUDE.md` | `@AGENTS.md` — only needed if the project already has a `CLAUDE.md` (it takes precedence over AGENTS.md) or on older Claude Code versions |
| Other tools | Check the tool's docs | A one-line pointer to `AGENTS.md` |

*Delete this section from your project's AGENTS.md once the pointers are in place.*

---

*This file follows the Cornerstone process. For more information, see CORNERSTONE.md. Prompts: [PROMPTS.md](https://github.com/craice/cornerstone/blob/main/PROMPTS.md)*
