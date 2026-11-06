---
name: start
description: Sets up this personal OS for a new user. First asks who I am and fills in my context and projects, then asks about tasks I repeat and helps me turn one into my first skill. Use when I say start, set me up, get started, or when OS/Context/about-me.md still has [placeholders] in it.
---
Ask every question one at a time. Wait for each answer before asking the next. Keep questions short and friendly. If an answer is vague, accept it and move on.

## Part 1: Who I am

1. Say in one line that you'll ask a few quick questions to set things up.
2. Ask:
   1. What's your name, and what do you do? (student, developer, or something else)
   2. What are you working on right now? Projects, jobs, school work, or side projects. A rough list is fine.
   3. What are your top 3 goals right now?
   4. When do you focus best?
   5. When you're stuck, how do you like things explained?
   6. Describe a look you like: colors, fonts, or an app or website whose style you love. (Say "skip" to do this later.)
3. Fill in OS/Context/about-me.md. Replace every [placeholder] and HTML comment with my answers, in first person.
4. For each project I named:
   - Create Projects/<Project Name>.md with: one line on what it is, "Status: just started", "Next step: [add one]", and a "## Where I left off" section
   - Add a row to OS/Context/project-registry.md: name, [[wikilink]] to the note, GitHub repo (only if I mentioned one, otherwise "-"), status
5. If I answered question 6, fill in what you can in Taste/taste.md, and log my answer at the top of Taste/references.md. Leave the rest as [placeholders].
6. Add any deadlines I mentioned to Tasks.md.
7. Add a line to OS/CHANGELOG.md: today's date — set up context and N projects — first run of start.
8. Summarize what you set up in 3 lines or fewer.

## Part 2: Find my first skill

9. Say in one line: "Now let's find something worth turning into a skill."
10. Ask:
   1. What's a task you do every week that feels repetitive?
   2. What do you start with for that task? (a transcript, rough notes, a list, a link, something else)
   3. What should the finished result look like, and where should it go?
11. Check OS/Skills/Skills-Index.md. If a skill already does this, tell me which one and ask if I want to use it or build my own.
12. Otherwise, suggest one skill in two lines: a short kebab-case name, and what it would do. Ask: "Want to build it now? I'll do it once with you first."
13. If I say no, add "Build a skill for: <the task>" to Tasks.md and stop.

## Part 3: Build it together

14. Ask me for a real example input: a file path, or text I paste in.
15. Do the task once on that example, following my answers from Part 2 and the conventions in OS/Rules/system-rules.md. Update any related project note and Tasks.md if it makes sense.
16. Show me what you made and ask: "Anything to change before I save this as a skill?" Apply my changes.
17. Save .agents/skills/<name>/SKILL.md in the same format as the other skills:
    - Frontmatter with `name` and a `description` that says what it does and starts its second sentence with "Use when"
    - Numbered steps that describe what you just did, written so they work for any future input, not just this example
    - A rule to only use what's in the source, and mark anything unclear as [check this]
18. Register it: add a row to OS/Skills/Skills-Index.md, and a line to OS/CHANGELOG.md: today's date — added <name> — <the task it handles>.
19. Show me the new SKILL.md, and tell me in one line how to run it next time.
