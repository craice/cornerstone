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
│   │Discovery │   │SPEC      │   │HTML/CSS  │   │ROADMAP   │   │AI        │   │Working   │    │
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
│   Cardboard maquette to test           HTML/CSS sketch to test                   │
│   proportions and concept              layout and visual direction               │
│                                                                                  │
│   Construction Documents ············> Roadmap                                   │
│   Detailed blueprints with             ROADMAP.md — phases, tasks,               │
│   dimensions and sequences             deliverables, validation                  │
│                                                                                  │
│   Site Preparation ··················> Setup                                     │
│   Survey, utilities, builder           AI.md — context, principles,              │
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
║  │  AI creates lightweight HTML/CSS prototype                      │                      ║
║  │  ├── Test layout and structure                                  │                      ║
║  │  ├── Test visual direction                                      │                      ║
║  │  ├── Test component design                                      │                      ║
║  │  └── Test content hierarchy                                     │                      ║
║  │                                                                 │                      ║
║  │  YOU review — confirms vision or loops back to Spec             │                      ║
║  └─────────────────────────────────────────────────────────────────┘                      ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 4: ROADMAP (Construction Documents)                                                ║
║  ┌─────────────────────────────────────────────────────────────────┐                      ║
║  │  AI generates ROADMAP.md                                        │                      ║
║  │  ├── Phase 1: [Tasks 1.1 - 1.n]                                 │                      ║
║  │  ├── Phase 2: [Tasks 2.1 - 2.n]                                 │                      ║
║  │  ├── Phase N: [Tasks N.1 - N.n]                                 │                      ║
║  │  ├── Execution Log (empty)                                      │                      ║
║  │  └── AI Decision Log (empty)                                    │                      ║
║  │                                                                 │                      ║
║  │  YOU review and approve                                         │                      ║
║  └─────────────────────────────────────────────────────────────────┘                      ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 5: SETUP (Site Preparation)                                                        ║
║  ┌─────────────────────────────────────────────────────────────────┐                      ║
║  │  AI generates AI.md (behavioral guide, not spec copy)           │                      ║
║  │  ├── Project overview (brief)                                   │                      ║
║  │  ├── Core principles (rules)                                    │                      ║
║  │  ├── Working process                                            │                      ║
║  │  ├── Logging requirements                                       │                      ║
║  │  └── Do's and Don'ts                                            │                      ║
║  │                                                                 │                      ║
║  │  Project folder ready:                                          │                      ║
║  │  your-project/                                                  │                      ║
║  │  ├── AI.md                                                      │                      ║
║  │  ├── SPECIFICATION.md                                           │                      ║
║  │  ├── ROADMAP.md                                                 │                      ║
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
Discovery      Programming Brief        (conversation)        Understand needs through Q&A
Specification  Schematic Design         SPECIFICATION.md      Define what to build
Prototype      Study Model              HTML/CSS files        Test ideas visually (optional)
Roadmap        Construction Documents   ROADMAP.md            Plan how to build it
Setup          Site Preparation         AI.md                 Prepare AI context
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
