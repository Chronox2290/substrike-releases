# substrike-releases

## Workflow

Shared across all Chronox2290 repos. Repo-specific rules elsewhere in this file win where they conflict.

### Plan
- 3+ steps or an architectural call: write the plan to `tasks/todo.md` as checkboxes before building. Tick items as they land.
- Check in before building only when the call is architectural, ambiguous, or hard to reverse. Otherwise state the reading of the ask in one line and go.
- If it goes sideways, stop and re-plan. Do not keep pushing a failing approach.

### Subagents
- Keep the main context clean. Big reads, research and parallel analysis go to subagents, one task each, returning a short summary.
- The expensive model plans and reviews. Fable, Sonnet or Haiku does the typing from a self-contained brief: goal, files allowed, definition of done, what to report back.

### Self-improvement loop
- Session start: read `tasks/lessons.md`.
- After any correction from Christian: add a one-line rule to `tasks/lessons.md` (the mistake, the rule that prevents it). Merge duplicates, prune stale rules, keep it short.

### Verify before done
- Never call it done without proof: run the tests, lint or build, check logs, show the result.
- Diff behaviour against main when relevant. Ask: would a staff engineer approve this?

### Elegance, balanced
- Non-trivial change: pause and ask if there is a simpler, cleaner way. If a fix feels hacky, redo it properly.
- Simple, obvious fixes: just do them. No over-engineering.

### Bugs and CI
- Given a bug report or failing CI: find the root cause and fix it. No hand-holding, no temporary patches.

### Close out
- Add a short review section to `tasks/todo.md`: what changed, how it was verified, what is still open.

### Principles
- Simplicity first. Minimal impact. Root causes, not band-aids.
