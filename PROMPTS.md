# Cornerstone — Prompts

> The single source for every Cornerstone prompt. Other documents link here instead of repeating them.

Copy a prompt, replace the `[brackets]`, and paste it into your AI tool.

---

## Kick-off

### One-Prompt Kick-off

Runs Discovery through Setup in a single conversation.

```
I want to build [your idea in 1-2 sentences].

Let's use the Cornerstone process:
1. Start with Discovery — interview me across the 6 dimensions
   (Purpose, Audience, Scope, Constraints, Quality, Identity)
2. Then generate SPECIFICATION.md
3. Then generate ROADMAP.md
4. Then generate AGENTS.md

Begin with Discovery. Ask me questions one group at a time.
```

---

## Phase 1: Discovery

```
I want to create [brief description of your idea].

Help me define this project using the Cornerstone Discovery process.
Interview me across these 6 dimensions: Purpose, Audience, Scope,
Constraints, Quality, and Identity. Ask questions one group at a time.
Challenge my assumptions when needed.
```

If the AI stops asking too early:

```
Keep going. What else should we define?
```

---

## Phase 2: Specification

```
Based on our Discovery conversation, create a complete SPECIFICATION.md
using the Cornerstone Specification template. Capture every decision we made.
Be comprehensive — this document should be the single source of truth
for the entire project.
```

For Low-energy projects, ask for the lite template instead:

```
Based on our Discovery conversation, create a SPECIFICATION.md using the
Cornerstone Specification Lite template. Keep it to essentials — one page.
```

---

## Phase 3: Prototype / PoC

```
Based on SPECIFICATION.md, create a lightweight prototype / proof of concept
that tests [specific aspect]. Keep it minimal and disposable — this is a
study model, not the final product. Focus on [the riskiest assumption you
need to validate].

Use real content where possible. Keep it in a single file if you can.
```

---

## Phase 4: Roadmap

```
Based on SPECIFICATION.md, create a ROADMAP.md using the Cornerstone
Roadmap template. Break the work into logical phases with numbered tasks,
deliverables, and validation criteria. Mark tasks only a human can do
(deploys, accounts, publishing) with [human]. Fill in Current State and
leave the Execution Log and AI Decision Log empty.
```

---

## Phase 5: Setup

```
Create an AGENTS.md file using the Cornerstone AGENTS template. This should
be a behavioral guide for AI tools working on this project. Reference
SPECIFICATION.md and ROADMAP.md for details — don't duplicate their content.
Focus on principles, process, and rules.
```

---

## Phase 6: Execution

### Start a session

```
Read AGENTS.md, SPECIFICATION.md, and ROADMAP.md.
Start from Current State in ROADMAP.md and confirm the next step before proceeding.
```

### Execute a phase

```
Execute Phase [N]: [Phase Name] from ROADMAP.md.
Follow SPECIFICATION.md. Mark tasks complete, update the Execution Log,
and log any decisions.
```

### Complete specific tasks

```
Complete tasks [X.X] through [X.X] from ROADMAP.md.
```

### Validate a phase

```
Run validation checks for Phase [N] as defined in ROADMAP.md.
```

### When something's wrong

```
Task [X.X] revealed that [describe problem].
Update SPECIFICATION.md and ROADMAP.md accordingly, review AGENTS.md,
then continue. Log the change in the right Decision Log.
```

### End a session

```
Before we stop: update Current State in ROADMAP.md — where we stopped,
the next step, and anything we tried and discarded.
```

---

## Adopting Cornerstone Mid-Project

```
This project is already in progress. Read the codebase and create a
SPECIFICATION.md that captures its current state using the Cornerstone
Specification template. Mark anything you had to infer as an open question.
Then create a ROADMAP.md for the remaining work and an AGENTS.md.
```

---

*This file is part of the Cornerstone process. For more information, see CORNERSTONE.md*
