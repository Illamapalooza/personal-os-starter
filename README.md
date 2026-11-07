# Personal OS Starter

Most of us use AI to build apps. This starter helps you build a system for yourself: a folder of markdown files and an agent that reads them.

It's made for [Google Antigravity](https://antigravity.google/) and [Obsidian](https://obsidian.md/), but everything is plain files, so other agents that read `AGENTS.md` can use it too.

## How it works

It's built like an operating system, in layers:

| Layer | Where it lives | What it does |
|---|---|---|
| **Boot** | `AGENTS.md` | Tells the agent what to read before doing anything |
| **OS** | `OS/` | The brain: rules, who you are, your projects, the skills index, and a changelog |
| **Skills** | `.agents/skills/` | The apps: things you repeat, written once as plain-English recipes |
| **Meta** | `Meta/` | What the system learns: rules from your corrections, and patterns in your weeks |
| **Taste** | `Taste/` | How you want things to look and sound. Slides and prototypes follow it |
| **System** | `System/` | The manual for humans: how it all fits together |
| **Data** | `Daily/`, `Projects/`, `Meetings/`, `Ideas/`, `Builds/`, `Inbox/`, `Tasks.md` | Your actual work |

The key idea: **intelligence and data stay separate.** Skills read `OS/` and `Meta/`, and write to your data folders. Read `System/README.md` for the full picture.

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

Let the agent set you up. In the Antigravity App or the CLI (`agy`), type:

```text
/start
```

If the slash command doesn't show up, type `Use the start skill` instead.

It asks a few quick questions about you, fills in `OS/Context/about-me.md`, and registers each of your projects. Then it asks about tasks you repeat and helps you build your first skill by doing one with you. Afterwards, start a new conversation and ask:

```text
What should I focus on today?
```

Prefer to do it by hand? Edit `OS/Context/about-me.md` directly.

### 2. Teach it something you repeat

Pick one task you do every week, such as meeting notes, a status update, or a weekly plan. Do it once with the agent:

```text
Help me with this task: [paste your messy input]
```

When you like the result, save it:

```text
That worked. Save what you just did as a skill I can reuse.
```

No task in mind? Try it on `Inbox/sample-meeting.txt`.

### 3. Correct it once

Run your skill and tell it what to change:

```text
That's too long. Keep it to 3 bullets.
```

Then type `/reflect`. It saves the rule to `Meta/Preferences.md`, so you won't have to say it again.

## Skills included

| Skill | What it does |
|---|---|
| `start` | Sets up your context and projects, then helps you build your first skill |
| `capture` | Parks an idea or task, so you can get back to what you were doing |
| `meeting-notes` | Turns a messy meeting into clean notes, and updates the project and your tasks |
| `idea-to-mvp` | Turns an idea into a one-page spec and a working prototype |
| `switch` | Catches you up on a project: where you left off and the next step |
| `daily-open` | Plans your day from your tasks, projects, notes, and ideas |
| `daily-close` | Records what got done and what carries over |
| `weekly-review` | Looks back on your week and sets next week's focus |
| `taste` | Learns your design taste from a link, screenshot, or description |
| `slides` | Builds an HTML slide deck that follows your taste |
| `reflect` | Turns your corrections into lasting rules in `Meta/` |
| `learn` | Finds patterns in your week and suggests new skills |

Change them, delete them, or add your own. They're only markdown.

## Example skill packs

Students: there's a ready-made pack in `Examples/student/` with `class-summary`, `study-prep` (reviewers, flashcards, practice tests), and `thesis`. Turn it on with:

```bash
cp -R Examples/student/*/ .agents/skills/
```

See `Examples/README.md` for details.

## Keep it safe

- **Keep secrets out.** Don't put passwords, API keys, or sensitive personal data in this folder. The agent can read what's here and may send it to its model.
- **Keep it private.** Once you add your own notes, make your copy a private repo.
- **Check its work.** The agent can get things wrong, so compare important notes with the source.
- **Follow your school's AI policy.** Use this to understand and organize your learning, not to submit AI work as your own.

## License

[MIT](LICENSE)
