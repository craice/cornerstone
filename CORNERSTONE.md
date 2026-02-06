# Cornerstone

> From idea to implementation through human-AI collaboration

---

## What is Cornerstone?

Cornerstone is a structured process for building projects in collaboration with AI. It transforms a rough idea into a well-defined specification, then into an actionable roadmap, and finally into a finished product.

The name comes from architecture: the cornerstone is the first stone laid, determining the position and alignment of the entire structure. In the same way, this process establishes the foundation before building begins.

### Core Philosophy

1. **Clarity before code** — Define what you're building before you build it
2. **Questions before answers** — Discovery through dialogue leads to better outcomes
3. **Incremental progress** — Break work into phases that can be validated independently
4. **Documented decisions** — Track what was decided and why for future reference
5. **Human direction, AI execution** — You set the vision, AI helps realize it

---

## The Process

Cornerstone has 5 phases:

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│  DISCOVERY  │ ──▶ │    SPEC     │ ──▶ │   ROADMAP   │ ──▶ │    SETUP    │ ──▶ │  EXECUTION  │
│             │     │             │     │             │     │             │     │             │
│ Define the  │     │ Document    │     │ Break into  │     │ Prepare     │     │ Build phase │
│ idea        │     │ everything  │     │ phases      │     │ AI context  │     │ by phase    │
└─────────────┘     └─────────────┘     └─────────────┘     └─────────────┘     └─────────────┘
```

---

## Phase 1: Discovery

**Goal:** Transform a vague idea into a clear vision through structured dialogue.

### How It Works

You start with an idea — it can be rough, incomplete, even just a feeling. Through a series of questions, the AI helps you refine and expand that idea into something concrete.

### What to Bring

- A basic concept or problem to solve
- Any constraints you know (technology, timeline, audience)
- References or inspirations (optional)

### What You'll Define

- **Purpose** — Why does this project exist?
- **Audience** — Who is it for?
- **Scope** — What's included and what's not?
- **Constraints** — Technical, time, or resource limitations
- **Success criteria** — How will you know it's done?
- **Differentiators** — What makes this unique?

### How to Start

Prompt an AI assistant with your idea and explicitly ask for questions:

```
I want to create [brief description of your idea]. 
Help me structure this. Ask questions to understand better.
```

**Important:** Don't rush this phase. Good questions lead to good specifications. Let the AI ask multiple rounds of questions until the vision is clear.

### Tips for Discovery

- Answer honestly, including "I don't know" — the AI can suggest options
- Share constraints early — they shape decisions
- Provide references when you have them
- Think out loud — partial thoughts help the AI understand your direction
- Ask the AI for suggestions when you're stuck

---

## Phase 2: Specification

**Goal:** Create a comprehensive document that defines everything about the project.

### How It Works

Based on the Discovery phase, the AI generates a detailed specification document (SPECIFICATION.md) that captures all decisions, requirements, and guidelines.

### What the Specification Includes

1. **Overview** — Project summary, key facts, what makes it unique
2. **Philosophy** — Core principles and values guiding the project
3. **Technical Details** — Stack, structure, conventions, tokens
4. **Components/Features** — Detailed description of each part
5. **Requirements** — Quality standards, accessibility, performance
6. **Constraints** — Browser support, dependencies, limitations

### How to Generate

After Discovery is complete:

```
Based on our conversation, create a complete SPECIFICATION.md 
that captures everything we defined. Be comprehensive.
```

### Review Checklist

Before moving on, verify:

- [ ] All decisions from Discovery are captured
- [ ] Nothing is ambiguous or left undefined
- [ ] Technical constraints are documented
- [ ] Success criteria are measurable
- [ ] You could hand this to someone else and they'd understand the project

---

## Phase 3: Roadmap

**Goal:** Break the specification into phases and actionable tasks.

### How It Works

The specification defines *what* to build. The roadmap defines *how* and *when*. It divides the work into logical phases, each with specific tasks that can be checked off.

### What the Roadmap Includes

1. **Phases** — Logical groupings of related work
2. **Tasks** — Specific, actionable items with unique IDs
3. **Dependencies** — What must be done before what
4. **Validation criteria** — How to verify each phase is complete
5. **Execution Log** — Space to record what was done (filled during execution)
6. **Decision Log** — Space to record decisions made (filled during execution)

### How to Generate

```
Based on SPECIFICATION.md, create a ROADMAP.md with:
- Logical phases
- Numbered tasks with checkboxes
- Validation criteria per phase
- Execution Log section (empty, to be filled)
- AI Decision Log section (empty, to be filled)
```

### Good Phase Design

Each phase should:

- Be completable in one work session (ideally)
- Have a clear, verifiable outcome
- Not depend on unfinished work from later phases
- Build on previous phases naturally

---

## Phase 4: Setup

**Goal:** Prepare the AI context file for execution.

### How It Works

Create an AI.md file that gives any AI tool the context it needs to work on your project. This file stays in the project root and serves as persistent instructions.

### What AI.md Includes

1. **Project Overview** — Brief description and key facts
2. **Key Files** — What to read before starting work
3. **Core Principles** — Rules that must never be violated
4. **Technical Stack** — Languages, tools, conventions
5. **File Structure** — Where things go
6. **Naming Conventions** — How to name things
7. **Working Process** — How to approach tasks
8. **Logging Requirements** — How to document work
9. **Validation Checklist** — How to verify quality
10. **Do's and Don'ts** — Explicit guidance

### How to Generate

```
Create an AI.md file with instructions for AI tools to work on this project.
Include everything an AI would need to understand context, conventions, 
and constraints. Reference SPECIFICATION.md and ROADMAP.md.
```

### Project Structure

After Setup, your project folder should contain:

```
your-project/
├── AI.md                    # AI context and instructions
├── SPECIFICATION.md         # What to build
├── ROADMAP.md   # How to build it (phases + tasks)
└── ... (project files will be added during execution)
```

---

## Phase 5: Execution

**Goal:** Build the project phase by phase, with documentation.

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

Before moving to the next phase:

```
Run validation checks for Phase [N] as defined in the roadmap.
```

### Handling Problems

If something doesn't work or needs clarification:

1. Stop and discuss before proceeding
2. Update the specification if requirements change
3. Document the decision in the AI Decision Log
4. Continue execution

---

## Templates

Cornerstone includes three template files to start your projects:

| Template | Purpose |
|----------|---------|
| `SPECIFICATION.template.md` | Structure for defining your project |
| `ROADMAP.template.md` | Structure for phases and tasks |
| `AI.template.md` | Structure for AI instructions |

Copy these templates into your project and fill them in through the Cornerstone process.

---

## Quick Start

### Option A: Full Process (Recommended for New Projects)

1. Start a conversation with an AI assistant
2. Share your idea and ask for Discovery questions
3. Answer questions until the vision is clear
4. Ask AI to generate SPECIFICATION.md
5. Review and adjust the specification
6. Ask AI to generate ROADMAP.md
7. Review and adjust the roadmap
8. Ask AI to generate AI.md
9. Create project folder with all three files
10. Execute phase by phase using an AI coding tool

### Option B: Quick Start (For Simpler Projects)

1. Copy the three templates to your project folder
2. Fill in SPECIFICATION.md manually or with AI help
3. Fill in ROADMAP.md with your planned phases
4. Fill in AI.md with project-specific instructions
5. Execute with an AI coding tool

---

## Best Practices

### For Discovery

- Let the AI ask at least 3 rounds of questions
- Don't skip details — they matter later
- Share your "why" not just your "what"
- Include constraints early

### For Specification

- Be specific, not vague
- Include examples where helpful
- Define what's out of scope
- Make success criteria measurable

### For Roadmap

- Keep phases focused (5-15 tasks each)
- Include validation criteria
- Allow for iteration
- Don't over-plan — you can adjust

### For Execution

- Do one phase at a time
- Validate before moving on
- Keep logs updated
- Review AI decisions regularly

---

## When to Use Cornerstone

**Good fit:**
- Design systems
- Websites and web apps
- Documentation projects
- Content systems
- APIs and backends
- Any project that benefits from upfront planning

**Maybe not ideal for:**
- Quick experiments or prototypes
- Highly uncertain/exploratory work
- Projects where requirements will change radically
- Very small tasks (< 1 hour of work)

---

## FAQ

**Q: How long does Discovery take?**
A: Usually 15-30 minutes of back-and-forth. Don't rush it.

**Q: Can I modify the specification later?**
A: Yes. The specification is a living document. Update it when requirements change.

**Q: Do I need all three files?**
A: For best results, yes. Each serves a different purpose. For small projects, you can simplify them.

**Q: Which AI tools work with Cornerstone?**
A: Any AI assistant for Discovery/Specification/Roadmap. AI coding tools (Claude Code, GitHub Copilot, Cursor, etc.) for Execution.

**Q: Can I use this for non-technical projects?**
A: Yes. The process works for any project that benefits from structured planning — writing, research, events, etc. Adapt the templates as needed.

---

## Credits

Cornerstone was developed by Rafael Craice through practical application on real projects, refining the process through iteration.

---

## License

MIT — Use freely, adapt as needed, share with others.

---

*"The cornerstone determines the entire structure. Lay it with care."*
