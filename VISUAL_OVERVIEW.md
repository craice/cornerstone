# Cornerstone Process — Visual Overview

## Linear Flow

```
┌──────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                              │
│   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐    │
│   │          │   │          │   │          │   │          │   │          │   │          │    │
│   │DISCOVERY │──>│   SPEC   │──>│PROTOTYPE │──>│ ROADMAP  │──>│  SETUP   │──>│EXECUTION │    │
│   │          │   │          │   │(optional)│   │          │   │          │   │          │    │
│   └──────────┘   └──────────┘   └──────────┘   └──────────┘   └──────────┘   └──────────┘    │
│        │              │              │              │              │              │          │
│        ▼              ▼              ▼              ▼              ▼              ▼          │
│   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐    │
│   │Discovery │   │SPEC      │   │Prototype │   │ROADMAP   │   │AGENTS    │   │Working   │    │
│   │Checklist │   │.md       │   │files     │   │.md       │   │.md       │   │Product   │    │
│   └──────────┘   └──────────┘   └──────────┘   └──────────┘   └──────────┘   └──────────┘    │
│                                                                                              │
└──────────────────────────────────────────────────────────────────────────────────────────────┘
```

## Flow with Iteration Loops

```
┌──────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                              │
│   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐    │
│   │          │   │          │   │          │   │          │   │          │   │          │    │
│   │DISCOVERY │──>│   SPEC   │──>│PROTOTYPE │──>│ ROADMAP  │──>│  SETUP   │──>│EXECUTION │    │
│   │          │   │          │   │(optional)│   │          │   │          │   │          │    │
│   └──────────┘   └──────────┘   └──────────┘   └──────────┘   └──────────┘   └──────────┘    │
│                       ▲              │                                            │          │
│                       │   prototype  │                                            │          │
│                       │   reveals    │                                            │          │
│                       └──────────────┘                                            │          │
│                       ▲                                                           │          │
│                       │              execution reveals                            │          │
│                       │              spec was incomplete                          │          │
│                       └──────────────────────────────────────────────────────────-┘          │
│                                                                                              │
└──────────────────────────────────────────────────────────────────────────────────────────────┘
```

## Architecture Analogy

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│                                                                                  │
│   ARCHITECTURE                              CORNERSTONE                          │
│   ────────────                              ───────────                          │
│                                                                                  │
│   Programming Brief ·················> Discovery                                 │
│   "What do you need? How do you        "Purpose, Audience, Scope,                │
│    live? What's your budget?"          Constraints, Quality, Identity"           │
│                                                                                  │
│   Schematic Design ··················> Specification                             │
│   Floor plans, elevations,             SPECIFICATION.md — complete               │
│   materials, systems                   project definition                        │
│                                                                                  │
│   Study Model ·······················> Prototype                                 │
│   Cardboard maquette to test           Minimal sketch to test                    │
│   proportions and concept              the riskiest assumption                   │
│                                                                                  │
│   Construction Documents ············> Roadmap                                   │
│   Detailed blueprints with             ROADMAP.md — phases, tasks,               │
│   dimensions and sequences             deliverables, validation                  │
│                                                                                  │
│   Site Preparation ··················> Setup                                     │
│   Survey, utilities, builder           AGENTS.md — context and                   │
│   instructions                         behavioral rules                          │
│                                                                                  │
│   Construction ······················> Execution                                 │
│   Build in planned sequences,          Build phase by phase,                     │
│   log progress, flag issues            log progress, flag issues                 │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

## Detailed Flow with Activities

```
╔═══════════════════════════════════════════════════════════════════════════════════════════╗
║                              CORNERSTONE PROCESS                                          ║
╠═══════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                           ║
║  PHASE 1: DISCOVERY (Programming Brief)                                                   ║
║  ┌─────────────────────────────────────────────────────────────────┐                      ║
║  │  YOU                              AI                            │                      ║
║  │  ────                             ──                            │                      ║
║  │  Share idea ────────────────────> Ask questions (6 dimensions)  │                      ║
║  │  Answer questions <────────────── Challenge assumptions         │                      ║
║  │  Provide details ───────────────> Refine understanding          │                      ║
║  │  Confirm direction <───────────── Summarize                     │                      ║
║  │                                                                 │                      ║
║  │  Dimensions: Purpose · Audience · Scope                         │                      ║
║  │              Constraints · Quality · Identity                   │                      ║
║  └─────────────────────────────────────────────────────────────────┘                      ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 2: SPECIFICATION (Schematic Design)                                                ║
║  ┌─────────────────────────────────────────────────────────────────┐                      ║
║  │  AI generates comprehensive SPECIFICATION.md                    │                      ║
║  │  ├── Overview & purpose                                         │                      ║
║  │  ├── Philosophy & decision framework                            │                      ║
║  │  ├── Technical details                                          │                      ║
║  │  ├── Features / Components                                      │                      ║
║  │  └── Requirements & constraints                                 │                      ║
║  │                                                                 │                      ║
║  │  YOU review and approve                                         │                      ║
║  └─────────────────────────────────────────────────────────────────┘                      ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 3: PROTOTYPE — optional (Study Model)                                              ║
║  ┌─────────────────────────────────────────────────────────────────┐                      ║
║  │  AI creates a minimal, disposable prototype                     │                      ║
║  │  ├── UI: layout, visual direction                               │                      ║
║  │  ├── API: data model, integration                               │                      ║
║  │  ├── CLI: commands, output format                               │                      ║
║  │  └── Data: transformations, edge cases                          │                      ║
║  │                                                                 │                      ║
║  │  YOU review — confirms vision or loops back to Spec             │                      ║
║  └─────────────────────────────────────────────────────────────────┘                      ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 4: ROADMAP (Construction Documents)                                                ║
║  ┌─────────────────────────────────────────────────────────────────┐                      ║
║  │  AI generates ROADMAP.md                                        │                      ║
║  │  ├── Changelog + Current State                                  │                      ║
║  │  ├── Phases 1..N: tasks ([human] marked)                        │                      ║
║  │  ├── Deliverables + validation                                  │                      ║
║  │  ├── Execution Log (empty)                                      │                      ║
║  │  └── AI Decision Log (empty)                                    │                      ║
║  │                                                                 │                      ║
║  │  YOU review and approve                                         │                      ║
║  └─────────────────────────────────────────────────────────────────┘                      ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 5: SETUP (Site Preparation)                                                        ║
║  ┌─────────────────────────────────────────────────────────────────┐                      ║
║  │  AI generates AGENTS.md (behavioral guide, not spec copy)       │                      ║
║  │  ├── Project overview (brief)                                   │                      ║
║  │  ├── Core principles (rules)                                    │                      ║
║  │  ├── Working process                                            │                      ║
║  │  ├── Logging requirements                                       │                      ║
║  │  └── Do's and Don'ts                                            │                      ║
║  │                                                                 │                      ║
║  │  Project folder ready:                                          │                      ║
║  │  your-project/                                                  │                      ║
║  │  ├── AGENTS.md                                                  │                      ║
║  │  ├── SPECIFICATION.md                                           │                      ║
║  │  ├── ROADMAP.md                                                 │                      ║
║  │  ├── DISCOVERY.md (optional)                                    │                      ║
║  │  └── prototype/ (optional)                                      │                      ║
║  └─────────────────────────────────────────────────────────────────┘                      ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 6: EXECUTION (Construction)                                                        ║
║  ┌─────────────────────────────────────────────────────────────────┐                      ║
║  │                                                                 │                      ║
║  │  ┌──────────────┐                                               │                      ║
║  │  │ Start Phase  │<─────────────────────────────┐                │                      ║
║  │  └──────┬───────┘                              │                │                      ║
║  │         ▼                                      │                │                      ║
║  │  ┌──────────────┐                              │                │                      ║
║  │  │Execute Tasks │                              │                │                      ║
║  │  └──────┬───────┘                              │                │                      ║
║  │         ▼                                      │                │                      ║
║  │  ┌──────────────┐                              │                │                      ║
║  │  │Mark Complete │  ─ [x] Task                  │                │                      ║
║  │  └──────┬───────┘                              │                │                      ║
║  │         ▼                                      │                │                      ║
║  │  ┌──────────────┐  Problem?                    │                │                      ║
║  │  │  Validate    │───────────> Loop back to     │                │                      ║
║  │  └──────┬───────┘             Spec or Roadmap  │                │                      ║
║  │         ▼                                      │                │                      ║
║  │  ┌──────────────┐                              │                │                      ║
║  │  │ Update Logs  │  ─ Execution Log             │                │                      ║
║  │  └──────┬───────┘  ─ AI Decision Log           │                │                      ║
║  │         │          ─ Current State             │                │                      ║
║  │         ▼                                      │                │                      ║
║  │  ┌──────────────┐     No    ┌──────────────┐   │                │                      ║
║  │  │ More phases? │──────────>│    DONE!     │   │                │                      ║
║  │  └──────┬───────┘           └──────────────┘   │                │                      ║
║  │         │ Yes                                  │                │                      ║
║  │         └──────────────────────────────────────┘                │                      ║
║  │                                                                 │                      ║
║  └─────────────────────────────────────────────────────────────────┘                      ║
║                                                                                           ║
╚═══════════════════════════════════════════════════════════════════════════════════════════╝
```

## File Outputs by Phase

```
Phase          Architecture Analogy     Output File           Purpose
─────          ────────────────────     ───────────           ───────
Discovery      Programming Brief        DISCOVERY.md          Understand needs through Q&A
Specification  Schematic Design         SPECIFICATION.md      Define what to build
Prototype      Study Model              prototype/ files      Test the riskiest idea (optional)
Roadmap        Construction Documents   ROADMAP.md            Plan how to build it
Setup          Site Preparation         AGENTS.md             Prepare AI context
Execution      Construction             (project files)       Build the actual product
                                        + Updated logs        Track progress and decisions
```

## Roles

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│   HUMAN                          AI                            │
│   ─────                          ──                            │
│                                                                │
│   • Sets vision                  • Asks clarifying questions   │
│   • Makes decisions              • Generates documents         │
│   • Reviews & approves           • Creates prototypes          │
│   • Evaluates prototypes         • Executes tasks              │
│   • Provides direction           • Logs decisions              │
│   • Validates results            • Follows specifications      │
│   • Decides when to loop back    • Flags ambiguities           │
│                                                                │
│   Like an architect:             Like a builder:               │
│   designs, decides, approves     executes, documents, flags    │
│                                                                │
│             ──────────────────>                                │
│   DIRECTION                     EXECUTION                      │
│             <──────────────────                                │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```
