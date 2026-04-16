# DISPATCH.md -- extra-sub-standalone-game-adventure

> Claude-owned sandbox. Playable game (genre TBD).
> Read CLAUDE.md first.

## Pre-Approved Tasks (No Confirmation Needed)

| Task Keyword | Description | Success Criteria | Delegate To |
|---|---|---|---|
| `explore` | Research game genres and mechanics, evaluate approaches | Notes written to `ai/` | `gemini-2.5-pro` |
| `research` | Deep research on chosen genre, game design patterns | Research note in `ai/` | `gemini-2.5-pro` |
| `audit` | Review existing code for bugs, quality, balance issues | Report written to `ai/` | `gemini-2.5-pro` |
| `tests-gen` | Generate test cases for game logic | Tests pass | `codestral-latest` |
| `docs-gen` | Generate or improve documentation | Docs written | `mistral-large-latest` |
| `self-audit` | Read STATE.md and assess progress vs roadmap | `ai/AUDIT.md` updated | `gemini-2.5-pro` |
| `roadmap-review` | Evaluate roadmap items, re-scope as needed | ROADMAP.md updated | `gemini-2.5-pro` |

## Requires Confirmation (Never Auto-Execute)

- `deploy` -- no deployment
- `delete` -- no file deletion without Perry's approval
- `install` -- no dependency changes

## Path Firewall

Autonomous work may only read/write files under:
```
c:\Users\perry\DevProjects\sandbox\extra-sub-standalone-game-adventure\**
```

## Opportunistic Lane (Budget Dispatcher)

**Eligible for autonomous execution:** `explore`, `research`, `audit`, `tests-gen`, `docs-gen`, `self-audit`, `roadmap-review`

**Branch naming:** `auto/sandbox-game-adventure-<task>-<YYYYMMDD-HHMMSS>`

**Commit prefix:** `[opportunistic][dispatch.mjs][<model>]`
