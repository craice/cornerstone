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
| **Low** | "I want this done with minimal effort" | Discovery (quick), Specification (use the lite template), Roadmap (flat task list), AGENTS.md (minimal) | Skip Prototype. Combine Discovery + Spec into one conversation. Roadmap can be a single phase. |
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
1. Update the relevant document (SPECIFICATION.md, ROADMAP.md) and bump its version
2. **Review AGENTS.md** — every time SPECIFICATION.md or ROADMAP.md changes, check if AGENTS.md needs updating (principles, references, or key values may have shifted)
3. Log the change in the right log (see [Decision Logs](#decision-logs))
4. Continue from where the change matters

### Decision Logs

Cornerstone keeps two decision logs, each with one job:

| Log | Lives in | What goes there | Who decides |
|-----|----------|-----------------|-------------|
| **Decision Log** | SPECIFICATION.md (Appendix) | Product and scope decisions — what the project is, what's in or out | The human |
| **AI Decision Log** | ROADMAP.md | Implementation decisions made during execution | The AI, reviewed by the human |

If an implementation decision changes scope or contradicts the spec, it stops being an implementation decision: the AI stops, asks, and the approved change goes in the spec's Decision Log.

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

Use the Discovery prompt in [PROMPTS.md](PROMPTS.md#phase-1-discovery). The AI interviews you; `DISCOVERY.template.md` is the checklist that makes sure nothing is missed.

### What Discovery Produces

Save the result as `DISCOVERY.md` in your project. It records the *why* behind the spec, but it is not maintained afterwards: once SPECIFICATION.md exists, the spec is the source of truth. If they disagree, the spec wins.

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
3. **Philosophy & Principles** — Core values, decision framework for tradeoffs
4. **Technical Specification** — Stack, structure, conventions, dependencies
5. **Design Tokens** — Colors, typography, spacing *(if visual project)*
6. **Features / Components** — Detailed description of each part
7. **Quality Requirements** — Performance, accessibility, compatibility, security
8. **Content & Copy** — Voice, tone, key messages *(if applicable)*
9. **Constraints & Limitations** — Technical, resource, and external limits
10. **References & Inspiration**
11. **Open Questions** — What's still undecided
- **Appendix: Decision Log** — Product and scope decisions

The numbering matches `SPECIFICATION.template.md`, so AGENTS.md can reference sections by number (e.g., *"see SPECIFICATION.md §4"*). Keep it stable: if you add a section, add it at the end.

For Low-energy projects, `SPECIFICATION.lite.template.md` covers the essentials in one page.

### How to Generate

After Discovery is complete, use the Specification prompt in [PROMPTS.md](PROMPTS.md#phase-2-specification).

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

Use the Prototype prompt in [PROMPTS.md](PROMPTS.md#phase-3-prototype--poc), naming the specific aspect and the riskiest assumption you want to test.

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

1. **Changelog** — Version history, so AGENTS.md can record which version it was synced with
2. **Current State** — Where the last session stopped, the next step, what's waiting on the human, what was tried and discarded
3. **Phases** — Logical groupings of related work (as many or few as needed)
4. **Tasks** — Specific, actionable items with unique IDs. Tasks only a human can do (deploys, accounts, publishing) are marked `[human]`
5. **Deliverables** — What should exist when the phase is complete
6. **Validation criteria** — How to verify each phase is done
7. **Execution Log** — Space to record what was done (filled during execution)
8. **AI Decision Log** — Space to record implementation decisions (filled during execution)

### How to Generate

Use the Roadmap prompt in [PROMPTS.md](PROMPTS.md#phase-4-roadmap).

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

Create an `AGENTS.md` file that gives any AI tool the context it needs to work on your project. This file stays in the project root and serves as persistent instructions — a briefing document that AI tools read before doing any work.

### Why AGENTS.md

`AGENTS.md` is the shared convention that AI coding tools read **automatically** at the start of every session. That matters: if the instructions only apply when you remember to say *"read the instructions file"*, the one session you forget is the one where the AI works without context.

When a tool reads its own file instead, add a one-line pointer — never a copy, or the two will drift apart. Claude Code, for example, reads AGENTS.md on its own unless the project has a `CLAUDE.md`; if it does, add `@AGENTS.md` to that `CLAUDE.md`. The template's Tool Compatibility section lists the pointers.

### What AGENTS.md Includes

AGENTS.md is a **behavioral guide**, not a copy of the specification. It tells the AI *how to work*, and points to other documents for *what to build*:

1. **Project Overview** — Brief description (2-3 sentences) and key facts
2. **Key Files** — What to read before starting work (always: SPECIFICATION.md and ROADMAP.md)
3. **Core Principles** — Rules that must never be violated
4. **Working Process** — How to start and end sessions, what to do before/during/after each phase
5. **Logging Requirements** — How to document work, and which decision log to use
6. **Validation Checklist** — How to verify quality
7. **Do's and Don'ts** — Explicit behavioral guidance

**Important:** Avoid duplicating content from SPECIFICATION.md. Instead, reference it. For example, instead of listing the full tech stack in AGENTS.md, write: *"See SPECIFICATION.md §4 for full technical details."*

### How to Generate

Use the Setup prompt in [PROMPTS.md](PROMPTS.md#phase-5-setup).

### Project Structure

After Setup, your project folder should contain:

```
your-project/
├── AGENTS.md                # How to work on this project (read automatically)
├── CLAUDE.md                # (only if needed) one-line pointer: @AGENTS.md
├── SPECIFICATION.md         # What to build — the source of truth
├── ROADMAP.md               # How to build it (current state + phases + logs)
├── DISCOVERY.md             # (optional) record of the Discovery conversation
├── prototype/               # (optional) study model files
└── ... (project files will be added during execution)
```

---

## Phase 6: Execution

**Goal:** Build the project phase by phase, with documentation.

*Architecture analogy: Construction — the builder follows the construction documents, works in planned sequences, logs progress, and flags issues for the architect to resolve.*

### How It Works

With the foundation in place, you execute one phase at a time. The AI reads the context files and follows the roadmap, checking off tasks and logging progress.

### Sessions

AI tools don't remember previous conversations. **Current State** in ROADMAP.md is the bridge between sessions:

- **Start of a session:** the AI reads AGENTS.md, SPECIFICATION.md, and ROADMAP.md, then picks up from Current State
- **End of a session:** the AI updates Current State — where it stopped, the next step, what's waiting on you, what was tried and discarded

The prompts for both are in [PROMPTS.md](PROMPTS.md#phase-6-execution).

### During Execution

The AI should:

- Follow the specification exactly
- Check off tasks as completed: `- [x] Task`
- Never check off a `[human]` task — prepare what it can, then list it in Current State as waiting on you
- Log a summary in the Execution Log
- Record implementation decisions in the AI Decision Log, and stop to ask before any decision that changes scope

### Validating a Phase

Before moving to the next phase, validate across all applicable categories:

- **Functional** — Does it work? Do features behave as specified?
- **Visual** — Does it look right? (if applicable)
- **Technical** — Is code quality acceptable? No regressions?
- **Documentation** — Are logs updated? Are decisions recorded?

See `ROADMAP.template.md` for detailed validation checklists per category.

### Handling Problems

If something doesn't work or needs clarification:

1. **Stop and discuss** before proceeding
2. **Update the specification** if requirements change (loop back)
3. **Document the decision** in the right log — scope changes in the spec, implementation choices in the roadmap
4. **Continue execution** from where the change matters

### When to Loop Back

During Execution, you might discover that:
- A spec requirement is ambiguous or contradictory → Update SPECIFICATION.md (and bump its version)
- A better approach exists than what was planned → Update ROADMAP.md (and bump its version)
- The scope needs to change → Go back to relevant sections

This is normal. The key is to update the documents so they remain the source of truth.

---

## Templates

Cornerstone includes templates to start your projects:

| Template | Purpose | Phase |
|----------|---------|-------|
| `DISCOVERY.template.md` | Structured discovery checklist | Discovery |
| `SPECIFICATION.template.md` | Complete project definition | Specification |
| `SPECIFICATION.lite.template.md` | One-page definition for Low-energy projects | Specification |
| `PROTOTYPE.template.md` | Lightweight prototyping guide | Prototype |
| `ROADMAP.template.md` | Current state, phases, tasks, and logs | Roadmap |
| `AGENTS.template.md` | AI behavioral instructions | Setup |

Copy these templates into your project and fill them in through the Cornerstone process. Every prompt lives in [PROMPTS.md](PROMPTS.md).

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
9. Ask AI to generate AGENTS.md (add pointers only for tools that need them — see the template)
10. Create project folder with all files
11. Execute phase by phase using an AI coding tool

### Option B: Quick Start (For Simpler Projects)

1. Copy the templates to your project folder
2. Fill in SPECIFICATION.md manually or with AI help
3. Fill in ROADMAP.md with your planned phases
4. Fill in AGENTS.md with project-specific instructions
5. Execute with an AI coding tool

### Option C: One-Prompt Kick-off

Paste the One-Prompt Kick-off from [PROMPTS.md](PROMPTS.md#one-prompt-kick-off) to run Discovery through Setup in a single conversation.

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
- End every session by updating Current State
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

[Purissimo](https://craice.github.io/purissimo/) is a minimalist design system built with pure HTML and CSS — zero JavaScript in components, inspired by Antarctic ice, with WCAG 2.1 AA accessibility as a core constraint. It was the project where Cornerstone was refined.

### How Cornerstone Was Used

1. **Discovery:** Defined the vision through conversation — a pure CSS design system inspired by Antarctic ice, with accessibility as a core constraint.
2. **Specification:** Generated a comprehensive SPECIFICATION.md covering every component, design token, naming convention, and quality requirement. Product decisions such as *why the Outfit typeface* and *why base-4 spacing* were recorded in the spec's Decision Log.
3. **Roadmap:** Broke the work into 8 phases and 134 tasks — foundation, base styles, components, layout and utilities, accessibility, documentation, validation and launch, then a v1.1 phase for icons and examples.
4. **Setup:** Created the AI instructions file with strict rules (no JavaScript, BEM naming, base-4 spacing, accessibility requirements) that kept the AI aligned across sessions.
5. **Execution:** Built phase by phase, each session starting by reading the context files. The AI Decision Log captured 85 implementation decisions — for example, using `:user-valid` instead of `:valid` so forms don't show errors before the user types, or limiting pure-CSS tabs to 5 panels to avoid selector bloat.

### Results

| Metric | Result |
|--------|--------|
| Phases / tasks | 8 phases, 134 tasks |
| AI implementation decisions logged | 85 |
| CSS (v1.0) | 2,316 lines, ~441 class selectors, 114 custom properties |
| File size | 39KB minified at v1.0, ~40KB after v1.1 (target: under 50KB) |
| Color contrast audit | 19 of 20 pairings pass WCAG AA; the exception (disabled buttons) is exempt and was still improved |
| JavaScript in components | Zero — the core principle held (the only script on the site is analytics on the landing page) |

### What It Proved

- Clear specification dramatically reduces AI hallucination and drift
- The AI instructions file is essential for maintaining consistency across sessions
- Logging decisions creates a valuable record that's useful long after the project is done
- The process works end-to-end for real, published projects

### What It Changed in Cornerstone

Purissimo also exposed gaps. Each became part of the process:

- **The AI checked off tasks it could not do.** Deployment, release tagging, and social sharing were marked complete while actually left for the owner. → Tasks only a human can do are now marked `[human]` and never checked off by the AI.
- **Deferred work had no home.** Browser-based accessibility audits were pushed from one phase to the next and tracked only inside log entries. → ROADMAP.md now has **Current State**, including what's waiting on the human.
- **The instructions file needed a better name.** It started as `CLAUDE.md`, then became `AI.md` to be tool-agnostic — but no tool reads `AI.md` on its own. → Cornerstone now uses `AGENTS.md`, which is both tool-agnostic and read automatically.
- **Two kinds of decisions got mixed.** Product choices (typeface, spacing) and implementation choices (CSS techniques) are different and need different reviewers. → The two decision logs now have explicit, separate jobs.

---

## FAQ

**Q: How long does Discovery take?**
A: Usually 15-30 minutes of back-and-forth. Don't rush it — the time invested here saves hours later.

**Q: Can I modify the specification later?**
A: Yes. The specification is a living document. Update it when requirements change, bump its version, review AGENTS.md, and log the change in the spec's Decision Log.

**Q: Do I need all the files?**
A: For best results, yes. Each serves a different purpose. For small projects, you can simplify them.

**Q: Is the Prototype phase required?**
A: No. It's optional and useful for any project type — UI, API, CLI, data pipeline — when you need to validate a risky assumption. Skip it when requirements are very clear and there's no significant uncertainty.

**Q: Which AI tools work with Cornerstone?**
A: Any AI assistant for Discovery/Specification. AI coding tools (Claude Code, Cursor, GitHub Copilot, etc.) for Execution. The process is tool-agnostic.

**Q: Can I use this for non-technical projects?**
A: Yes. The process works for any project that benefits from structured planning — writing, research, events, etc. Adapt the templates as needed.

**Q: What if I'm mid-project and want to adopt Cornerstone?**
A: Start by writing a SPECIFICATION.md that captures the current state. Then create a ROADMAP.md for the remaining work. Then create AGENTS.md. You don't need to start over — PROMPTS.md has a prompt for this.

**Q: Why AGENTS.md and not a custom file name?**
A: Because AI coding tools read AGENTS.md automatically. A custom name only works when you remember to ask the AI to read it. When a tool's own file takes precedence (like an existing CLAUDE.md in Claude Code), that file gets a one-line pointer to AGENTS.md.

---

## Credits

Cornerstone was developed by Rafael Craice through practical application on real projects — most notably [Purissimo](https://craice.github.io/purissimo/) — refining the process through iteration.

The framework draws on principles from architectural practice, product design, and the lived experience of building things with AI.

---

## License

MIT — Use freely, adapt as needed, share with others.

---

*"No architect starts construction without a plan. Neither should you."*
