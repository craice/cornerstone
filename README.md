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
5. **Setup** — Prepare AI context in AGENTS.md, read automatically by AI coding tools
6. **Execution** — Build phase by phase, logging progress and decisions, picking up each session from where the last one stopped

## Quick Start

1. Read `CORNERSTONE.md` for the full process
2. Copy templates from `/templates` to your project
3. Follow the phases

Or paste the [One-Prompt Kick-off](PROMPTS.md#one-prompt-kick-off) to run Discovery through Setup in a single conversation. Every prompt lives in `PROMPTS.md`.

## Files

```
cornerstone/
├── CORNERSTONE.md                     # The complete process guide
├── PROMPTS.md                         # Every prompt, in one place
├── README.md                          # This file
├── VISUAL_OVERVIEW.md                 # Diagrams and visual reference
├── LICENSE
└── templates/
    ├── DISCOVERY.template.md          # Structured discovery checklist
    ├── SPECIFICATION.template.md      # What to build
    ├── SPECIFICATION.lite.template.md # What to build — one page, for small projects
    ├── PROTOTYPE.template.md          # Lightweight prototyping guide
    ├── ROADMAP.template.md            # How to build it, and where you stopped
    └── AGENTS.template.md             # AI behavioral instructions
```

## Case Study

Cornerstone was refined building [Purissimo](https://craice.github.io/purissimo/), a pure HTML/CSS design system with zero JavaScript: 8 phases, 134 tasks, 85 AI decisions logged, and a 39KB minified result with zero JavaScript in its components. See the [full case study](CORNERSTONE.md#case-study-purissimo), including what the project changed in Cornerstone itself.

## Credits

Developed by [Rafael Craice](https://github.com/craice) — product designer at the intersection of design, product, and technology.

## License

[MIT](LICENSE)