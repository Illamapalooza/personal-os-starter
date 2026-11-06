---
name: idea-to-mvp
description: Turns an idea note into a one-page spec and a small working prototype, then tracks it as a project. Use when I say build this idea, make an MVP, prototype something, or use my creative block on an idea from Ideas/.
---
1. Find the idea in Ideas/. If I didn't say which one, list them and ask.
2. Pick a short slug for it. Write Builds/<slug>/SPEC.md, under one page:
   - The problem, in one line
   - Who it's for
   - Exactly 3 must-have features
   - What's out of scope
3. Tell me the 3 features in one line each, then start building. Don't wait for approval unless I asked you to.
4. Build Builds/<slug>/index.html as a single file:
   - Inline CSS and JavaScript. No installs, no frameworks, no build step.
   - No external requests, so it works offline. Include realistic sample data.
   - Clean, modern design that works on a laptop screen.
5. Open it in the browser and check that each of the 3 features works. Fix anything broken. If you can't open a browser, tell me to open the file myself.
6. Create Projects/<Idea Name>.md with one line on what it is, "Status: prototype", a next step, and links to the spec and the build. Add a link to the project in the idea note.
7. Reply in 3 lines: what you built, where it lives, and the next step.

Rules:
- Stay within the 3 features. No login, database, payments, or deployment.
- Working beats polished. If something takes too long, cut it and say so.
