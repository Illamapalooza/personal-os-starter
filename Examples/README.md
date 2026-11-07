# Example skill packs

Ready-made skills you can turn on. They live here, not in `.agents/skills/`, so they don't load until you want them.

| Pack | Skills | For |
|---|---|---|
| `student/` | `class-summary`, `study-prep`, `thesis` | Students: lectures, exams, thesis and subjects |

## Turn on a pack

```bash
cp -R Examples/student/*/ .agents/skills/
```

Then ask the agent: `Add the student skills to OS/Skills/Skills-Index.md and log it in the changelog.`

Each skill is just a folder with a `SKILL.md`. Open one, read it, and change it to fit how you study.
