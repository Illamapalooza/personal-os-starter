---
name: slides
description: Builds a presentation as a single HTML file that follows my taste. Use when I ask for slides, a deck, or a presentation on a topic, or want to turn a note into a talk.
---
1. Read Taste/taste.md. If it's still mostly [placeholders], ask me for 3 words that describe the look I want, then continue.
2. Ask in one message, and accept short answers: What's the topic or source note? Who's the audience? How many minutes?
3. Plan the deck: about one slide per minute, one idea per slide. Show me the slide titles as a list and continue unless I object.
4. Build Builds/<topic>-slides/index.html as one file:
   - Inline CSS and JavaScript. No installs, no frameworks, no external requests, so it works offline.
   - Arrow keys and click to move between slides. Each slide fills a 16:9 screen.
   - Follow Taste/taste.md exactly: colors, fonts, layout, tone, and everything under "Never".
   - Short text on slides. Put anything longer in speaker notes inside an HTML comment on each slide.
5. Open it in the browser and check every slide: nothing overflows, text is readable from the back of a room, and it matches my taste. Fix what's off.
6. Tell me in 2 lines where it is and how to present it (open the file, press the arrow keys).
