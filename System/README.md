# How this system works

The manual for humans. The agent doesn't need this file; you do.

## The layers

```
┌────────────────────────────────────────────────────┐
│ YOU         direct, review, correct                │
├────────────────────────────────────────────────────┤
│ AGENTS.md   boot: tells the agent what to read     │
├────────────────────────────────────────────────────┤
│ OS/         intelligence: rules, context, skills   │
│ .agents/    the skills themselves                  │
├────────────────────────────────────────────────────┤
│ Meta/       learning: preferences, patterns        │
│ Taste/      how things should look and sound       │
├────────────────────────────────────────────────────┤
│ Data        Daily/ Projects/ Meetings/ Ideas/      │
│             Builds/ Inbox/ Tasks.md                │
└────────────────────────────────────────────────────┘
```

## What happens when you run a skill

1. You type `/daily-open`
2. The agent boots from `AGENTS.md`: reads the rules, who you are, your projects, and your preferences
3. It loads `.agents/skills/daily-open/SKILL.md` and follows the steps
4. It reads your data and writes today's plan to `Daily/`

## How it improves

- **You correct it** → `reflect` writes a rule to `Meta/Preferences.md` → every skill follows it from then on
- **You use it for a week** → `learn` reads your notes, writes `Meta/Patterns.md`, and suggests new skills in `Meta/Optimizations.md`
- **You share a design you like** → `taste` turns it into principles in `Taste/taste.md` → every slide deck and prototype follows them
- **You add a skill** → it's logged in `OS/CHANGELOG.md` and listed in `OS/Skills/Skills-Index.md`

## The one rule

Intelligence and data stay separate. You can delete every note and the system still works. You can swap the agent and your notes still make sense.
