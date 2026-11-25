# Cornerstone

> From idea to implementation through human-AI collaboration

---

## What is Cornerstone?

Cornerstone is a structured process for building projects in collaboration with AI. It transforms a rough idea into a well-defined specification, validates it through lightweight prototyping, then breaks it into an actionable roadmap and a finished product.

The name comes from architecture: the cornerstone is the first stone laid, determining the position and alignment of the entire structure. In the same way, this process establishes the foundation before building begins.

### The Architecture Analogy

Building software with AI is remarkably similar to building a house. No architect starts construction without a plan — and yet, most people start coding with AI by typing "build me an app." Cornerstone brings the discipline of architectural practice to AI-assisted development:

| Architecture | Cornerstone | Purpose |
|-------------|-------------|---------|
| Programming Brief | Discovery | Understand what's needed and why |
| Schematic Design | Specification | Define the complete vision |
| Study Model | Prototype | Test ideas cheaply before committing |
| Construction Documents | Roadmap | Detail exactly how to build it |
| Site Preparation | Setup | Prepare the environment |
| Construction | Execution | Build it, phase by phase |

Just as an architect wouldn't skip from a client conversation to pouring concrete, Cornerstone ensures you don't skip from an idea to writing code.

### Core Philosophy

1. **Clarity before code** — Define what you're building before you build it
2. **Questions before answers** — Discovery through dialogue leads to better outcomes
3. **Test before you invest** — Validate ideas with lightweight prototypes before planning execution
4. **Incremental progress** — Break work into phases that can be validated independently
5. **Documented decisions** — Track what was decided and why for future reference
6. **Human direction, AI execution** — You set the vision, AI helps realize it

### Sizing

Not every project needs the full process. Before starting, ask yourself honestly: **how much energy do I want to put into this?** The answer determines how much structure you need.

| Level | Energy | What to do | What to simplify or skip |
|-------|--------|-----------|--------------------------|
| **Low** | "I want this done with minimal effort" | Discovery (quick), Specification (essentials only), Roadmap (flat task list), AI.md (minimal) | Skip Prototype. Combine Discovery + Spec into one conversation. Roadmap can be a single phase. |
| **Medium** | "I want this done well" | All phases. Discovery, Specification, Roadmap, Setup — each as its own step. | Prototype is optional. Documents can be concise but should be complete. |
| **High** | "I want this done right — no shortcuts" | Full process, all phases, thorough documentation. Prototype when there's uncertainty. | Nothing skipped. Take time with Discovery. Spec should be comprehensive. |

**The key insight:** Even at Low energy, you still produce the minimum viable documentation — a specification and a roadmap. The difference is depth, not presence. A Low-energy spec might be one page; a High-energy spec might be ten. Both are valid.

Choose honestly. A Low-energy project done consistently beats a High-energy project abandoned halfway.

---

## The Process

Cornerstone has 6 phases:

```
┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
│DISCOVERY │───>│   SPEC   │───>│PROTOTYPE │───>│ ROADMAP  │───>│  SETUP   │───>│EXECUTION │
│          │    │          │    │          │    │          │    │          │    │          │
│Understand│    │Define the│    │Test the  │    │Plan the  │    │Prepare   │    │Build it  │
│the need  │    │vision    │    │idea      │    │build     │    │AI context│    │phase by  │
│          │    │          │    │(optional)│    │          │    │          │    │phase     │
└──────────┘    └──────────┘    └──────────┘    └──────────┘    └──────────┘    └──────────┘
```

### It's Not Always a Straight Line

The diagram above shows the ideal flow, but real projects loop back. Like an architect who revises the schematic after a study model reveals a problem, you should expect — and welcome — iteration:

```
DISCOVERY ──> SPEC ──> PROTOTYPE ──> ROADMAP ──> SETUP ──> EXECUTION
                 ▲         │                                   │
                 │         │ prototype reveals                 │
                 └─────────┘ spec needs fixing                 │
                 ▲                                             │
                 │         execution reveals                   │
                 └─────────────────────────────────────────────┘
                           spec was incomplete
```

**Common loops:**
- **Prototype → Specification:** The prototype reveals that a feature doesn't work as imagined. Go back and fix the spec.
- **Execution → Specification:** During development, you discover a requirement was missing or wrong. Update the spec, adjust the roadmap, continue.
- **Discovery → Discovery:** The first round of questions reveals the idea is bigger than expected. Keep going until it's clear.

**When to loop back:**
- Something feels wrong or unclear
- The AI is making assumptions you didn't intend
- A decision in a later phase contradicts an earlier one
- You changed your mind (this is normal and healthy)

**When looping, always:**
1. Update the relevant document (SPECIFICATION.md, ROADMAP.md)
2. **Review AI.md** — every time SPECIFICATION.md or ROADMAP.md changes, check if AI.md needs updating (principles, references, or key values may have shifted)
3. Log the change in the Decision Log
4. Continue from where the change matters

---

## Phase 1: Discovery

**Goal:** Transform a vague idea into a clear vision through structured dialogue.

*Architecture analogy: The programming brief — where the architect interviews the client to understand their needs, constraints, lifestyle, and aspirations before drawing a single line.*

### How It Works

You start with an idea — it can be rough, incomplete, even just a feeling. Through a structured conversation, the AI helps you explore and define the idea from multiple angles. Think of it as an architectural brief: the AI interviews you, challenges your assumptions, and helps you articulate what you might not have words for yet.

### The Discovery Protocol

Discovery covers 6 dimensions. The AI should guide you through each one, but you don't need to address them in order. Conversations are organic — the important thing is that all dimensions are covered before moving on.

#### 1. Purpose — *Why does this exist?*
- What problem does this solve?
- Who has this problem today?
- What happens if this project doesn't exist?
- What's the motivation behind it (personal, commercial, learning)?

#### 2. Audience — *Who is it for?*
- Who is the primary user?
- Who is the secondary user (if any)?
- What do they already use today?
- What's their technical level?

#### 3. Scope — *What's in and what's out?*
- What are the core features (the must-haves)?
- What is explicitly NOT part of this project?
- What might be added later but not now?
- What's the smallest version that would be valuable?

#### 4. Constraints — *What limits exist?*
- Technical: languages, platforms, dependencies, hosting
- Time: deadline, available hours per week
- Resources: solo or team, budget, existing assets
- Knowledge: what you know vs. what you'd need to learn

#### 5. Quality — *What standards matter?*
- Performance expectations
- Accessibility requirements
- Browser/device support
- Visual quality bar (rough, polished, pixel-perfect)

#### 6. Identity — *What makes this unique?*
- What's the personality or tone?
- Are there references or inspirations?
- What should this NOT look or feel like?
- If this project were a building, what kind would it be?

### How to Start

Use this prompt to kick off Discovery:

```
I want to create [brief description of your idea].

Help me define this project using the Cornerstone Discovery process.
Interview me across these 6 dimensions: Purpose, Audience, Scope,
Constraints, Quality, and Identity. Ask questions one group at a time.
Challenge my assumptions when needed.
```

### Discovery Checklist

Before moving to Specification, verify all dimensions are covered:

- [ ] **Purpose** is clear — you can explain why this exists in one sentence
- [ ] **Audience** is defined — you know who it's for and who it's not for
- [ ] **Scope** has boundaries — you know what's in, what's out, and what's for later
- [ ] **Constraints** are documented — technical, time, and resource limits are known
- [ ] **Quality** standards are set — you know how good is good enough
- [ ] **Identity** has direction — you have a sense of personality and style

### Tips for Discovery

- Answer honestly, including "I don't know" — the AI can suggest options
- Share constraints early — they shape every decision downstream
- Provide references when you have them (links, screenshots, descriptions)
- Think out loud — partial thoughts help the AI understand your direction
- Don't rush. Good discovery takes 15-30 minutes. It saves hours later.
- If the AI stops asking questions too early, say: *"Keep going. What else should we define?"*

---

## Phase 2: Specification

**Goal:** Create a comprehensive document that defines everything about the project.

*Architecture analogy: The schematic design — a complete drawing that captures the architect's vision, including floor plans, elevations, materials, and systems. Detailed enough that anyone could understand what will be built.*

### How It Works

Based on the Discovery phase, the AI generates a detailed specification document (SPECIFICATION.md) that captures all decisions, requirements, and guidelines. This is your single source of truth.

### What the Specification Includes

1. **Overview** — Project summary, key facts, what makes it unique
2. **Purpose & Goals** — Problem, audience, success criteria, out of scope
3. **Philosophy** — Core principles, decision framework for tradeoffs
4. **Technical Details** — Stack, structure, conventions, dependencies
5. **Design Tokens** — Colors, typography, spacing (if visual project)
6. **Features/Components** — Detailed description of each part
7. **Quality Requirements** — Performance, accessibility, compatibility
8. **Constraints** — Technical, resource, and external limitations

### How to Generate

After Discovery is complete:

```
Based on our Discovery conversation, create a complete SPECIFICATION.md
using the Cornerstone Specification template. Capture every decision we made.
Be comprehensive — this document should be the single source of truth
for the entire project.
```

### Review Checklist

Before moving on, verify:

- [ ] All decisions from Discovery are captured
- [ ] Nothing is ambiguous or left undefined
- [ ] Technical constraints are documented
- [ ] Success criteria are measurable
- [ ] Out of scope is explicitly listed
- [ ] You could hand this to someone else and they'd understand the project
- [ ] Open questions are listed (if any remain)

---

## Phase 3: Prototype / Proof of Concept *(Optional)*

**Goal:** Validate key ideas quickly and cheaply before investing in detailed planning.

*Architecture analogy: The study model — a rough maquette made from cardboard and foam, built to test proportions, spatial relationships, and the overall concept. It's not the building; it's a tool for thinking.*

### When to Prototype / PoC

This phase is optional. Use it when:

- You're unsure if a technical approach will work
- You want to test a layout, interaction, flow, or integration before committing
- You need to prove feasibility of a critical path
- You want early feedback on any risky assumption

Skip it when:

- Requirements are very clear and well-understood
- The project is too small to justify the extra step
- There's no significant uncertainty to resolve

### What It Looks Like

The shape of a prototype depends on the type of project. The goal is always the same — **answer your riskiest question with the least effort.**

| Project Type | Prototype / PoC Example | What to Validate |
|-------------|------------------------|-----------------|
| **UI / Website** | Single HTML/CSS file, no JS | Layout, visual direction, content hierarchy, responsive behavior |
| **API / Backend** | Minimal endpoint + request/response example | Data model, auth flow, integration with external services |
| **CLI** | Single script with hardcoded inputs | Command structure, output format, core algorithm |
| **Data Pipeline** | Small script with sample data | Data transformations, input/output format, edge cases |

### Philosophy

Prototypes and proofs of concept follow the same principles regardless of project type:

- **Minimal tooling** — use the simplest possible approach (for UI: pure HTML/CSS; for APIs: a single file; for CLIs: a script)
- **Static or hardcoded** — don't build real infrastructure; fake what you can
- **Disposable** — meant to be thrown away or heavily rewritten
- **Fast** — should take minutes to an hour, not days
- **Real content** — use actual data, not placeholders

For UI projects, this aligns with the [Purissimo](https://craice.github.io/purissimo/) philosophy: pure HTML and CSS, zero JavaScript, maximum clarity.

### How to Create

```
Based on SPECIFICATION.md, create a lightweight prototype / proof of concept
that tests [specific aspect]. Keep it minimal and disposable.
This is a study model, not the final product. Focus on [the riskiest
assumption you need to validate].
```

### Evaluating the Prototype

After reviewing the prototype, ask yourself:

- [ ] Does this match what I imagined during Discovery?
- [ ] Does anything feel wrong or surprising?
- [ ] Are there spec decisions that need to change?
- [ ] Is there anything I hadn't considered that the prototype revealed?

**If the prototype reveals problems:** Loop back to Specification, update the document, and optionally prototype again.

**If it confirms the vision:** Move on to Roadmap with confidence.

### Tips for Prototyping

- Don't polish. Prototypes are disposable.
- Test one thing at a time — a full prototype of everything is just building the project
- Use real content when possible (not "Lorem ipsum")
- Show it to someone else if you can — fresh eyes catch things you miss
- Save the prototype file if it contains useful patterns for Execution

---

## Phase 4: Roadmap

**Goal:** Break the specification into phases and actionable tasks.

*Architecture analogy: The construction documents — detailed blueprints with dimensions, materials, sequences, and specifications that the builder follows to construct the building.*

### How It Works

The specification defines *what* to build. The roadmap defines *how* and *when*. It divides the work into logical phases, each with specific tasks that can be checked off.

### What the Roadmap Includes

1. **Phases** — Logical groupings of related work (as many or few as needed)
2. **Tasks** — Specific, actionable items with unique IDs
3. **Deliverables** — What should exist when the phase is complete
4. **Validation criteria** — How to verify each phase is done
5. **Execution Log** — Space to record what was done (filled during execution)
6. **Decision Log** — Space to record decisions made (filled during execution)

### How to Generate

```
Based on SPECIFICATION.md, create a ROADMAP.md using the Cornerstone
Roadmap template. Break the work into logical phases with numbered tasks,
deliverables, and validation criteria. Include empty Execution Log and
AI Decision Log sections.
```

### Good Phase Design

Each phase should:

- Be completable in one work session (ideally)
- Have a clear, verifiable outcome
- Not depend on unfinished work from later phases
- Build on previous phases naturally

**Number of phases:** Use as many as the project needs. A small project might have 3 phases; a complex one might have 10. Don't force your project into a fixed number.

---

## Phase 5: Setup

**Goal:** Prepare the AI context file for execution.

*Architecture analogy: Site preparation — before construction begins, the site is surveyed, utilities are marked, and the builder receives a clear set of instructions about how to work on this specific project.*

### How It Works

Create an AI.md file that gives any AI tool the context it needs to work on your project. This file stays in the project root and serves as persistent instructions — a briefing document that any AI tool reads before doing any work.

### What AI.md Includes

AI.md is a **behavioral guide**, not a copy of the specification. It tells the AI *how to work*, and points to other documents for *what to build*:

1. **Project Overview** — Brief description (2-3 sentences) and key facts
2. **Key Files** — What to read before starting work (always: SPECIFICATION.md and ROADMAP.md)
3. **Core Principles** — Rules that must never be violated
4. **Working Process** — How to approach tasks, what to do before/during/after each phase
5. **Logging Requirements** — How to document work and decisions
6. **Validation Checklist** — How to verify quality
7. **Do's and Don'ts** — Explicit behavioral guidance

**Important:** Avoid duplicating content from SPECIFICATION.md. Instead, reference it. For example, instead of listing the full tech stack in AI.md, write: *"See SPECIFICATION.md §4 for full technical details."*

### How to Generate

```
Create an AI.md file using the Cornerstone AI template. This should be a
behavioral guide for AI tools working on this project. Reference
SPECIFICATION.md and ROADMAP.md for details — don't duplicate their content.
Focus on principles, process, and rules.
```

### Project Structure

After Setup, your project folder should contain:

```
your-project/
├── AI.md                    # How to work on this project
├── SPECIFICATION.md         # What to build
├── ROADMAP.md               # How to build it (phases + tasks)
├── prototype/               # (optional) study model files
└── ... (project files will be added during execution)
```

---

## Phase 6: Execution

**Goal:** Build the project phase by phase, with documentation.

*Architecture analogy: Construction — the builder follows the construction documents, works in planned sequences, logs progress, and flags issues for the architect to resolve.*

### How It Works

With the foundation in place, you execute one phase at a time. The AI reads the context files and follows the roadmap, checking off tasks and logging progress.

### Starting a Phase

```
Read AI.md, SPECIFICATION.md, and ROADMAP.md.
Execute Phase [N]: [Phase Name].
Mark tasks as complete, update Execution Log, and log any decisions.
```

### During Execution

The AI should:

- Follow the specification exactly
- Check off tasks as completed: `- [x] Task`
- Log a summary in the Execution Log
- Document any decisions in the AI Decision Log

### Validating a Phase

Before moving to the next phase, validate across all applicable categories:

- **Functional** — Does it work? Do features behave as specified?
- **Visual** — Does it look right? (if applicable)
- **Technical** — Is code quality acceptable? No regressions?
- **Documentation** — Are logs updated? Are decisions recorded?

See `ROADMAP.template.md` for detailed validation checklists per category.

```
Run validation checks for Phase [N] as defined in the roadmap.
```

### Handling Problems

If something doesn't work or needs clarification:

1. **Stop and discuss** before proceeding
2. **Update the specification** if requirements change (loop back)
3. **Document the decision** in the AI Decision Log
4. **Continue execution** from where the change matters

### When to Loop Back

During Execution, you might discover that:
- A spec requirement is ambiguous or contradictory → Update SPECIFICATION.md
- A better approach exists than what was planned → Update ROADMAP.md
- The scope needs to change → Go back to relevant sections

This is normal. The key is to update the documents so they remain the source of truth.

---

## Templates

Cornerstone includes templates to start your projects:

| Template | Purpose | Phase |
|----------|---------|-------|
| `DISCOVERY.template.md` | Structured discovery checklist | Discovery |
| `SPECIFICATION.template.md` | Complete project definition | Specification |
| `PROTOTYPE.template.md` | Lightweight prototyping guide | Prototype |
| `ROADMAP.template.md` | Phases, tasks, and logs | Roadmap |
| `AI.template.md` | AI behavioral instructions | Setup |

Copy these templates into your project and fill them in through the Cornerstone process.

---

## Quick Start

### Option A: Full Process (Recommended)

1. Start a conversation with an AI assistant
2. Share your idea and start the Discovery Protocol
3. Answer questions until all 6 dimensions are covered
4. Ask AI to generate SPECIFICATION.md
5. Review and adjust the specification
6. *(Optional)* Create a lightweight prototype to test key ideas
7. Ask AI to generate ROADMAP.md
8. Review and adjust the roadmap
9. Ask AI to generate AI.md
10. Create project folder with all files
11. Execute phase by phase using an AI coding tool

### Option B: Quick Start (For Simpler Projects)

1. Copy the templates to your project folder
2. Fill in SPECIFICATION.md manually or with AI help
3. Fill in ROADMAP.md with your planned phases
4. Fill in AI.md with project-specific instructions
5. Execute with an AI coding tool

### Option C: One-Prompt Kick-off

Paste this to start a new project in a single prompt:

```
I want to build [your idea in 1-2 sentences].

Let's use the Cornerstone process:
1. Start with Discovery — interview me across the 6 dimensions
   (Purpose, Audience, Scope, Constraints, Quality, Identity)
2. Then generate SPECIFICATION.md
3. Then generate ROADMAP.md
4. Then generate AI.md

Begin with Discovery. Ask me questions one group at a time.
```

---

## Best Practices

### For Discovery
- Let the AI ask at least 3 rounds of questions
- Don't skip details — they matter later
- Share your "why" not just your "what"
- Include constraints early — they shape everything
- If something is unclear, say so. "I don't know" is a valid answer.

### For Specification
- Be specific, not vague
- Include examples where helpful
- Define what's out of scope (this prevents more problems than anything else)
- Make success criteria measurable

### For Prototyping / PoC
- Keep it simple — minimal tooling, single file when possible
- Test the riskiest assumption first
- Don't polish; it's disposable
- Use real content, not placeholder text

### For Roadmap
- Use as many phases as the project needs (no fixed number)
- Keep phases focused (5-15 tasks each)
- Include validation criteria for each phase
- Don't over-plan — you can adjust

### For Execution
- Do one phase at a time
- Validate before moving on
- Keep logs updated
- Review AI decisions regularly
- Loop back when something's wrong — don't push through

---

## When to Use Cornerstone

**Good fit:**
- Websites and web apps
- Design systems
- Documentation projects
- Content systems
- APIs and backends
- Any project that benefits from upfront planning

**Maybe not ideal for:**
- Quick experiments or prototypes (< 1 hour of work)
- Highly uncertain/exploratory research
- Projects where requirements will change radically every day
- Learning exercises where the process IS the point

---

## Case Study: Purissimo

TO DO

### How Cornerstone Was Used

1. **Discovery:** Defined the vision through conversation — a pure CSS design system inspired by Antarctic ice, with accessibility as a core constraint.
2. **Specification:** Generated a comprehensive SPECIFICATION.md covering every component, design token, naming convention, and quality requirement.
3. **Roadmap:** Broke the work into phases — foundation first, then components, then interactive elements, then documentation.
4. **Setup:** Created AI.md with strict rules (no JavaScript, BEM naming, accessibility requirements) that kept the AI aligned across multiple sessions.
5. **Execution:** Built phase by phase, with each session starting by reading the context files. The AI Decision Log captured choices like "why Outfit typeface" and "why base-4 spacing."

### What It Proved

- Clear specification dramatically reduces AI hallucination and drift
- The AI.md file is essential for maintaining consistency across sessions
- Logging decisions creates a valuable record that's useful long after the project is done
- The process works end-to-end for real, published projects

---

## FAQ

**Q: How long does Discovery take?**
A: Usually 15-30 minutes of back-and-forth. Don't rush it — the time invested here saves hours later.

**Q: Can I modify the specification later?**
A: Yes. The specification is a living document. Update it when requirements change, and log the change.

**Q: Do I need all the files?**
A: For best results, yes. Each serves a different purpose. For small projects, you can simplify them.

**Q: Is the Prototype phase required?**
A: No. It's optional and useful for any project type — UI, API, CLI, data pipeline — when you need to validate a risky assumption. Skip it when requirements are very clear and there's no significant uncertainty.

**Q: Which AI tools work with Cornerstone?**
A: Any AI assistant for Discovery/Specification. AI coding tools (Claude Code, Cursor, GitHub Copilot, etc.) for Execution. The process is tool-agnostic.

**Q: Can I use this for non-technical projects?**
A: Yes. The process works for any project that benefits from structured planning — writing, research, events, etc. Adapt the templates as needed.

**Q: What if I'm mid-project and want to adopt Cornerstone?**
A: Start by writing a SPECIFICATION.md that captures the current state. Then create a ROADMAP.md for the remaining work. Then create AI.md. You don't need to start over.

---

## Credits

Cornerstone was developed by Rafael Craice through practical application on real projects — most notably [Purissimo](https://craice.github.io/purissimo/) — refining the process through iteration.

The framework draws on principles from architectural practice, product design, and the lived experience of building things with AI.

---

## License

MIT — Use freely, adapt as needed, share with others.

---

*"No architect starts construction without a plan. Neither should you."*
