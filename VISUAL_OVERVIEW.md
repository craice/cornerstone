# Cornerstone Process — Visual Overview

## Linear Flow

```
┌─────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                             │
│   ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐            │
│   │          │    │          │    │          │    │          │    │          │            │
│   │ DISCOVERY│───▶│   SPEC   │───▶│ ROADMAP  │───▶│  SETUP   │───▶│EXECUTION │            │
│   │          │    │          │    │          │    │          │    │          │            │
│   └──────────┘    └──────────┘    └──────────┘    └──────────┘    └──────────┘            │
│        │               │               │               │               │                  │
│        ▼               ▼               ▼               ▼               ▼                  │
│   ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐            │
│   │Questions │    │SPEC      │    │ROADMAP   │    │AI        │    │Working   │            │
│   │& Answers │    │.md       │    │.md       │    │.md       │    │Product   │            │
│   └──────────┘    └──────────┘    └──────────┘    └──────────┘    └──────────┘            │
│                                                                                             │
└─────────────────────────────────────────────────────────────────────────────────────────────┘
```

## Detailed Flow with Activities

```
╔═══════════════════════════════════════════════════════════════════════════════════════════╗
║                              CORNERSTONE PROCESS                                          ║
╠═══════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                           ║
║  PHASE 1: DISCOVERY                                                                       ║
║  ┌─────────────────────────────────────────────────────────────────┐                     ║
║  │  YOU                              AI                            │                     ║
║  │  ────                             ──                            │                     ║
║  │  Share idea ──────────────────▶ Ask questions                  │                     ║
║  │  Answer questions ◀────────────── Clarify                      │                     ║
║  │  Provide details ─────────────▶ Refine understanding           │                     ║
║  │  Confirm direction ◀──────────── Summarize                     │                     ║
║  └─────────────────────────────────────────────────────────────────┘                     ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 2: SPECIFICATION                                                                   ║
║  ┌─────────────────────────────────────────────────────────────────┐                     ║
║  │  AI generates comprehensive SPECIFICATION.md                    │                     ║
║  │  ├── Overview & purpose                                         │                     ║
║  │  ├── Philosophy & principles                                    │                     ║
║  │  ├── Technical details                                          │                     ║
║  │  ├── Features / Components                                      │                     ║
║  │  └── Requirements & constraints                                 │                     ║
║  │                                                                  │                     ║
║  │  YOU review and approve                                         │                     ║
║  └─────────────────────────────────────────────────────────────────┘                     ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 3: ROADMAP                                                                         ║
║  ┌─────────────────────────────────────────────────────────────────┐                     ║
║  │  AI generates ROADMAP.md                                        │                     ║
║  │  ├── Phase 1: [Tasks 1.1 - 1.n]                                │                     ║
║  │  ├── Phase 2: [Tasks 2.1 - 2.n]                                │                     ║
║  │  ├── Phase 3: [Tasks 3.1 - 3.n]                                │                     ║
║  │  ├── ...                                                        │                     ║
║  │  ├── Execution Log (empty)                                      │                     ║
║  │  └── AI Decision Log (empty)                                    │                     ║
║  │                                                                  │                     ║
║  │  YOU review and approve                                         │                     ║
║  └─────────────────────────────────────────────────────────────────┘                     ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 4: SETUP                                                                           ║
║  ┌─────────────────────────────────────────────────────────────────┐                     ║
║  │  AI generates AI.md                                             │                     ║
║  │  ├── Project context                                            │                     ║
║  │  ├── Core principles                                            │                     ║
║  │  ├── Technical conventions                                      │                     ║
║  │  ├── Working process                                            │                     ║
║  │  └── Logging requirements                                       │                     ║
║  │                                                                  │                     ║
║  │  Project folder ready:                                          │                     ║
║  │  your-project/                                                  │                     ║
║  │  ├── AI.md                                                      │                     ║
║  │  ├── SPECIFICATION.md                                           │                     ║
║  │  └── ROADMAP.md                                                 │                     ║
║  └─────────────────────────────────────────────────────────────────┘                     ║
║                                        │                                                  ║
║                                        ▼                                                  ║
║  PHASE 5: EXECUTION                                                                       ║
║  ┌─────────────────────────────────────────────────────────────────┐                     ║
║  │                                                                  │                     ║
║  │  ┌──────────────┐                                               │                     ║
║  │  │ Start Phase  │◀─────────────────────────────┐               │                     ║
║  │  └──────┬───────┘                              │               │                     ║
║  │         ▼                                       │               │                     ║
║  │  ┌──────────────┐                              │               │                     ║
║  │  │Execute Tasks │                              │               │                     ║
║  │  └──────┬───────┘                              │               │                     ║
║  │         ▼                                       │               │                     ║
║  │  ┌──────────────┐                              │               │                     ║
║  │  │Mark Complete │  ─ [x] Task                  │               │                     ║
║  │  └──────┬───────┘                              │               │                     ║
║  │         ▼                                       │               │                     ║
║  │  ┌──────────────┐                              │               │                     ║
║  │  │  Validate    │                              │               │                     ║
║  │  └──────┬───────┘                              │               │                     ║
║  │         ▼                                       │               │                     ║
║  │  ┌──────────────┐                              │               │                     ║
║  │  │ Update Logs  │  ─ Execution Log             │               │                     ║
║  │  │              │  ─ AI Decision Log           │               │                     ║
║  │  └──────┬───────┘                              │               │                     ║
║  │         ▼                                       │               │                     ║
║  │  ┌──────────────┐     No    ┌──────────────┐  │               │                     ║
║  │  │ More phases? │──────────▶│    DONE!     │  │               │                     ║
║  │  └──────┬───────┘           └──────────────┘  │               │                     ║
║  │         │ Yes                                   │               │                     ║
║  │         └───────────────────────────────────────┘               │                     ║
║  │                                                                  │                     ║
║  └─────────────────────────────────────────────────────────────────┘                     ║
║                                                                                           ║
╚═══════════════════════════════════════════════════════════════════════════════════════════╝
```

## File Outputs by Phase

```
Phase        Output File           Purpose
─────        ───────────           ───────
Discovery    (conversation)        Define requirements through Q&A
Spec         SPECIFICATION.md      Document what to build
Roadmap      ROADMAP.md            Document how to build it
Setup        AI.md                 Prepare AI context
Execution    (project files)       Build the actual product
             + Updated logs        Track progress and decisions
```

## Roles

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│   HUMAN                          AI                           │
│   ─────                          ──                           │
│                                                                │
│   • Sets vision                  • Asks clarifying questions  │
│   • Makes decisions              • Generates documents        │
│   • Reviews & approves           • Executes tasks             │
│   • Provides direction           • Logs decisions             │
│   • Validates results            • Follows specifications     │
│                                                                │
│   DIRECTION ──────────────────▶                               │
│             ◀────────────────── EXECUTION                     │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```
