# STATE -- extra-sub-standalone-game-adventure

## Current Context

BUILD pipeline enabled 2026-05-25. `ai/pipelines.json` defines the
`build-mvp` pipeline; step 1 (`research`) is the first runnable step.

The pipeline is the cursor — read `ai/pipeline-state.json` to see which
step is in flight. This STATE.md is a fallback narrative for sessions
that haven't loaded the pipeline file yet.

## What's Done

- [x] Scaffold metadata: CLAUDE.md, DISPATCH.md, ai/STATE.md, ROADMAP.md
- [x] BUILD pipeline authored at ai/pipelines.json (build-mvp, 6 steps)
- [x] `feature` and `proposal` added to DISPATCH.md opportunistic_tasks

## Next

**Next:** Run pipeline step 1 — `research` task picks a game genre + core
mechanic that fits CLAUDE.md constraints (TypeScript, playable, not
RPG/sand), writes rationale to `ai/DECISIONS.md`.

## Pipeline structure

See `ai/pipelines.json`:

1. research → `ai/DECISIONS.md` (genre choice)
2. proposal → `ai/GDD.md` (game design doc) [depends on 1]
3. feature → scaffold package.json, tsconfig, src/, smoke test [depends on 2]
4. feature → first GDD feature [depends on 3]
5. feature → core loop (input → update → render) [depends on 4]
6. audit → MVP review [depends on 5]

After build-mvp completes, author a `build-content` pipeline to add
levels/enemies/progression (or wait for Phase B `plan-feature` task).
