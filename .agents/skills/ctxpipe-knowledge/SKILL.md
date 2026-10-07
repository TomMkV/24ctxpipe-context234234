---
name: ctxpipe-knowledge
---

# ctxpipe knowledge

Write reviewable markdown. Hydrate copies these files into the serving store; it does not infer claims from prose.

## Layout

- Greenfield: `knowledge/<area>/<unit>.md`
- Existing tree: match the folders already present
- Linked remotes: `repositories/<name>.md` with required `git`
- Do not rewrite `notion/`, `linear/`, or `confluence/`

## Schema

Knowledge files need no required keys. Optional `claims:` items use file-relative `to`. Skip an item if `to` is missing.

## Confidence

Calibrate in the file: **0.5** typical, **0.7** strong, **≥0.85** rare. Ask how sure the user is. Set `valid_to` from the source when it has an end date.

## What a good unit looks like

One unit per file. Keep it short. Link to other units instead of pasting them. Add claims only for facts you would defend. No meeting-dump blobs. No serving-store jargon (`obj_`, SPO tables) in the file.
