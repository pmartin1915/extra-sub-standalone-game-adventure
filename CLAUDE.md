# extra-sub-standalone-game-adventure -- CLAUDE.md

This is a **Claude-owned sandbox project** built autonomously by the budget dispatcher.

## Charter

Build a **playable game**. The specific genre and mechanics are for the model to choose and justify during the research/planning phase. The game should be fun, interactive, and progressively more complex as dispatch cycles add features.

**Constraints on genre choice:**
- Must be implementable in TypeScript (Node.js CLI or browser-based)
- Must be playable (not just a simulation or visualization)
- Must have clear win/loss conditions or progression
- Avoid overlap with dnd-game (no tabletop RPG mechanics) and sand-physics (no particle simulation)

## Tech Stack

TypeScript, Node.js. Browser-based via Vite if graphical. Terminal-based is acceptable for text games.

## In Scope

- Game design documents, architecture plans
- TypeScript source code under `src/`
- Unit tests for game logic
- Asset descriptions (text-based; no binary assets initially)

## Out of Scope (NEVER)

- Editing files outside this sandbox
- External API calls or paid services
- `npm install` without Perry's approval

## Hard Path Constraints

Claude may ONLY touch files under:
```
c:\Users\perry\DevProjects\sandbox\extra-sub-standalone-game-adventure\**
```

## State Files

- `ai/STATE.md` -- current context, what's done, what's next
- `ai/DECISIONS.md` -- append-only decision log
- `ROADMAP.md` -- longer-horizon goals and status
