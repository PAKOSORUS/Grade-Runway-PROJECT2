# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Current state

The repository (Grade-Runway, "PROECT2") currently contains **only a documentation skeleton under `docs/`**. There is no source code, build system, linter, or test setup yet, and it is not a git repository. Add build/lint/test commands here once code exists.

Documentation is written in **Thai**, and each folder's `index.md` describes what belongs there. Keep new docs consistent with that language.

## Docs structure (`docs/`)

The folders are numbered to follow the project workflow, and each `index.md` links to the next stage using Obsidian-style wikilinks (e.g. `[[../02-plan/index|02-plan]]`):

- `00-archived` — retired docs. Never delete docs outright; move them here to preserve decision history.
- `01-requirements/` — flow: `01-spec` (source of truth for requirements) → `02-plan` (roadmap/milestones) → `03-task` (actionable task breakdown).
- `02-design/` — `01-prototypes` (UI/UX wireframes, design system) and `02-technical` (architecture, DB schema, API design, tech choices). Technical design is the blueprint developers code against and the basis for the test plan.
- `03-testing/` — `01-test-plan` (derived from spec + design) → `02-test-result` (pass/fail, bugs).
- `04-retrospectives` — lessons learned per phase/sprint, drawing on test results and the log.
- `05-log` — chronological changelog, decision log, and incidents.

When adding docs, put them in the matching stage folder, and keep the wikilink flow between stages intact (use `[[relative/path/index|label]]` links).
