# Portable Project Memory

Portable Project Memory is a required project folder that records project status, decisions, session handoffs, and change history.

It exists for one reason: an embedded project should be resumable after a git pull on another machine or in another Codex session.

This is not a chat archive system. It is a project continuity record.

## Required location

```text
projects/<project_name>/memory/
```

## Required contents

```text
memory/
  current-state.md
  session-handoff.md
  decisions.md
  change-log.md
  next-steps.md
  project-state.json
  sessions/
  snapshots/
```

## Required behavior

At the end of each work session, update:

- `memory/current-state.md`
- `memory/session-handoff.md`
- `memory/change-log.md`
- `memory/next-steps.md`
- `memory/project-state.json`

Keep these short and practical. If a project can not be resumed from these files, they are not doing their job.

## File meanings

### current-state.md

A plain-language snapshot of where the project stands.

Include:

- what is working
- what is blocked
- what is being built right now

### session-handoff.md

A note for the next session.

Include:

- what was completed
- what changed
- what is partially done
- what to do next

### decisions.md

Decisions that should not be rediscovered.

Examples:

- shared inputs belong in `library/`
- writes belong in `projects/<project_name>/`
- example code is copied before modification

### change-log.md

A running list of meaningful changes.

Do not log every file save. Log milestones and behavior changes.

### next-steps.md

The next actions in order. Keep it short.

### project-state.json

A small machine-readable snapshot of status.

Recommended fields:

- project name
- vendor and board
- current focus
- active tasks
- blocked items
- next step
- last updated timestamp

### sessions/

Optional session notes. Keep them readable.

### snapshots/

Optional machine-readable snapshots.

## Commit rule

The `memory/` folder is meant to be committed with the project.

If the memory folder is not committed, the project will not resume cleanly.

## Optional chat archives

If you need to preserve full chat logs, store them separately under `memory/sessions/` or another clearly named folder.

Do not rely on raw chat logs as the primary record. The required memory files above are the authoritative continuity record.
