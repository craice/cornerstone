![Cornerstone](img/cornerstone-logo.png)

# Cornerstone

> A planning framework optimized for building projects with AI

Cornerstone is a structured process that transforms rough ideas into well-defined specifications, validates them through lightweight prototyping, and breaks them into actionable roadmaps — giving AI tools the context they need to execute well.

## The Problem

Most people start building with AI by typing *"build me an app."* This works for small tasks, but for anything substantial, it leads to scope drift, inconsistent results, and lost context between sessions.

Cornerstone solves this the same way architects solve the complexity of building construction: **with structured planning before execution.**

## The Architecture Analogy

| Architecture | Cornerstone | What Happens |
|-------------|-------------|--------------|
| Programming Brief | **Discovery** | Interview to understand needs |
| Schematic Design | **Specification** | Define the complete vision |
| Study Model | **Prototype** | Test ideas cheaply *(optional)* |
| Construction Docs | **Roadmap** | Detail how to build it |
| Site Preparation | **Setup** | Prepare AI context |
| Construction | **Execution** | Build phase by phase |

## The 6 Phases

```
DISCOVERY → SPECIFICATION → PROTOTYPE → ROADMAP → SETUP → EXECUTION
```

1. **Discovery** — Define the idea through structured AI-guided Q&A
2. **Specification** — Document everything in SPECIFICATION.md
3. **Prototype / PoC** — *(Optional)* Test key ideas with minimal, disposable code
4. **Roadmap** — Break work into phases in ROADMAP.md
5. **Setup** — Prepare AI context in AI.md
6. **Execution** — Build phase by phase, logging progress and decisions

## Quick Start

1. Read `CORNERSTONE.md` for the full process
2. Copy templates from `/templates` to your project
3. Follow the phases

Or use the one-prompt kick-off:

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

## Files

```
cornerstone/
├── CORNERSTONE.md                    # The complete process guide
├── README.md                         # This file
├── VISUAL_OVERVIEW.md                # Diagrams and visual reference
└── templates/
    ├── DISCOVERY.template.md         # Structured discovery checklist
    ├── SPECIFICATION.template.md     # What to build
    ├── PROTOTYPE.template.md         # Lightweight prototyping guide
    ├── ROADMAP.template.md           # How to build it
    └── AI.template.md                # AI behavioral instructions
```

## Case Study

TO DO

## Credits

Developed by [Rafael Craice](https://github.com/craice) — product designer at the intersection of design, product, and technology.

## License

MIT