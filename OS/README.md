# OS

The system's brain. Everything the agent needs to know about **how** to work lives here. Your actual work lives outside this folder.

| Folder | What's inside |
|---|---|
| `Rules/` | Principles and conventions the agent always follows |
| `Context/` | Who you are and what you're working on |
| `Skills/` | The index of every skill and what it does |
| `CHANGELOG.md` | Every change to the system, newest first |

The skill files themselves live in `.agents/skills/`, because that's where Antigravity loads them from. `OS/Skills/Skills-Index.md` is the map.
