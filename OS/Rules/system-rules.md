# System Rules

## Principles

### 1. Everything in one folder
Work, ideas, plans, and the system that manages them all live here. One source of truth.

### 2. Data vs intelligence
- **Intelligence** (how the system works): `AGENTS.md`, `OS/`, `.agents/skills/`
- **Learning** (what the system has learned about me): `Meta/`
- **Taste** (how I want things to look and sound): `Taste/`
- **Data** (my actual work): `Daily/`, `Projects/`, `Meetings/`, `Ideas/`, `Builds/`, `Inbox/`, `Tasks.md`

Skills read intelligence and write data. Only `start`, `reflect`, `learn`, `taste`, and new skills change intelligence, learning, or taste.

### 3. Adapt to me, not the other way around
The system learns from my corrections (`reflect`) and my patterns (`learn`), not from what I say I'll do.

### 4. Friction is signal
When something is annoying or wrong, it's data. Capture it with `reflect` right away.

### 5. Keep it short
Show what matters now. Long output gets ignored.

## Conventions

- Daily plans go in `Daily/YYYY-MM-DD.md`
- Tasks live in `Tasks.md`
- Each project has a note in `Projects/` and a row in `OS/Context/project-registry.md`
- Meeting notes go in `Meetings/YYYY-MM-DD-<project>.md`
- New ideas go in `Ideas/`
- Prototypes and slide decks go in `Builds/<name>/`
- Anything other people will see follows `Taste/taste.md`
- Unprocessed files go in `Inbox/`
- School work goes in `Academics/` (used by the student pack in `Examples/student/`)
- Use [[wikilinks]] to connect related notes
- Don't invent facts. If something isn't in my notes, say so

## When the system changes

Whenever a skill, rule, or context file is added or changed:
1. Add a line to the top of `OS/CHANGELOG.md`: date, what changed, why
2. If it's a new skill, add it to `OS/Skills/Skills-Index.md`
