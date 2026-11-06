# Personal OS Starter

Most of us use AI to build apps. This starter helps you build a system for yourself: a folder of markdown files and an agent that reads them.

It's made for [Google Antigravity](https://antigravity.google/) and [Obsidian](https://obsidian.md/), but everything is plain files, so other agents that read `AGENTS.md` can use it too.

## How it works

| Part | Where it lives | What it does |
|---|---|---|
| **Context** | `AGENTS.md` | Tells the agent who you are and how you work |
| **Skills** | `.agents/skills/` | Teaches the agent the things you repeat |
| **Notes** | Everything else | Gives the agent something to remember and connect |

## Set it up

1. [Install Antigravity](https://antigravity.google/download) and sign in with your Google account.
2. Get this repo. Click **Use this template** on GitHub, or run:

   ```bash
   git clone https://github.com/Illamapalooza/personal-os-starter.git
   ```

3. Open the folder in Antigravity.
4. Optional: open the same folder as a vault in Obsidian, so you can read your notes and see how they connect.

## Build your first skill

### 1. Make it yours

Let the agent set you up. In the agent panel, type:

```text
Use the start skill
```

In the CLI (`agy`), you can type `/start` instead.

It asks you 5 quick questions, fills in `AGENTS.md`, and creates a note for each of your projects. Then start a new conversation and ask:

```text
What should I focus on today?
```

Prefer to do it by hand? Edit `AGENTS.md` directly.

### 2. Teach it something you repeat

Pick one task you do every week, such as class notes, meeting minutes, or a weekly plan. Do it once with the agent:

```text
Help me with this task: [paste your messy input]
```

When you like the result, save it:

```text
That worked. Save what you just did as a skill I can reuse.
```

No task in mind? Try it on `Inbox/sample-lecture.txt`.

### 3. Correct it once

Run your skill and tell it what to change:

```text
That's too long. Add a rule to AGENTS.md to keep it shorter.
```

Now you won't have to say that again.

## Skills included

| Skill | What it does |
|---|---|
| `start` | Asks you a few questions and sets up `AGENTS.md` and your projects |
| `capture` | Parks an idea or task, so you can get back to what you were doing |
| `class-summary` | Turns a messy transcript or rough notes into a clean study note |
| `study-prep` | Makes flashcards and a quiz from your notes |
| `daily-open` | Plans your day from your tasks, projects, notes, and ideas |
| `daily-close` | Records what got done and what carries over |
| `weekly-review` | Looks back on your week and sets next week's focus |
| `reflect` | Turns your corrections into lasting rules |

Change them, delete them, or add your own. They're only markdown.

## Keep it safe

- **Keep secrets out.** Don't put passwords, API keys, or sensitive personal data in this folder. The agent can read what's here and may send it to its model.
- **Keep it private.** Once you add your own notes, make your copy a private repo.
- **Check its work.** The agent can get things wrong, so compare important notes with the source.
- **Follow your school's AI policy.** Use this to understand and organize your learning, not to submit AI work as your own.

## License

[MIT](LICENSE)
