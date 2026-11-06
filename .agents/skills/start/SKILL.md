---
name: start
description: Sets up this personal OS for a new user. First asks who I am and fills in AGENTS.md and project notes, then asks about tasks I repeat and helps me turn one into my first skill. Use when I say start, set me up, get started, or when AGENTS.md still has [placeholders] in it.
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
3. Update AGENTS.md:
   - Replace every [placeholder] and HTML comment in "About me", "My goals right now", and "How I work" with my answers, in first person.
   - Leave "How this vault works" and "Preferences" exactly as they are.
4. For each project or job I named, create Projects/<Project Name>.md with:
   - One line on what it is
   - Status: just started
   - Next step: [add one]
   - GitHub: owner/repo, only if I mentioned a repo for it
5. If Projects/Example-Project.md still exists and I named at least one project, delete it.
6. Add any deadlines I mentioned to Tasks.md.
7. Summarize what you set up in 3 lines or fewer.

## Part 2: Find my first skill

8. Say in one line: "Now let's find something worth turning into a skill."
9. Ask:
   1. What's a task you do every week that feels repetitive?
   2. What do you start with for that task? (a transcript, rough notes, a list, a link, something else)
   3. What should the finished result look like, and where should it go?
10. Look at the skills already in .agents/skills/. If one already does this, tell me which one and ask if I want to use it or build my own.
11. Otherwise, suggest one skill in two lines: a short kebab-case name, and what it would do. Ask: "Want to build it now? I'll do it once with you first."
12. If I say no, add "Build a skill for: <the task>" to Tasks.md and stop.

## Part 3: Build it together

13. Ask me for a real example input: a file path, or text I paste in.
14. Do the task once on that example, following my answers from Part 2. Save the result where I said it should go. Update any related project note and Tasks.md if it makes sense.
15. Show me what you made and ask: "Anything to change before I save this as a skill?" Apply my changes.
16. Save .agents/skills/<name>/SKILL.md in the same format as the other skills:
    - Frontmatter with `name` and a `description` that says what it does and starts its second sentence with "Use when"
    - Numbered steps that describe what you just did, written so they work for any future input, not just this example
    - A rule to only use what's in the source, and mark anything unclear as [check this]
17. Show me the new SKILL.md, and tell me in one line how to run it next time.
