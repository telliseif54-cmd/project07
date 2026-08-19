# PROJECT_STATE.md — Living Project State

Last updated: 2026-08-19

## Current status
**Stage:** 0 — repository foundation and project definition.

The repository was inspected before this memory layer was added. The only pre-existing file was `README.md`, containing the 2026 thematic research-project call/reference material.

No application source code, tests, package manifest, CI workflow, deployment configuration, or formal product specification has been identified yet.

## Completed
- Confirmed repository identity and default branch.
- Preserved the original `README.md` content.
- Added portable AI operating instructions in `AGENTS.md`.
- Added canonical project context in `AI_MEMORY.md`.
- Added this live project-state file.
- Added a decision log and change log.

## Current objective
Turn this repository into a self-describing project workspace whose documentation is sufficient for another AI to take over safely and continue development without access to previous conversation history.

## Pending definition work
The next substantive step is to define the actual intended project/product behind `project07`.

Minimum information still needed from repository evidence or the user:
- project name/title;
- problem being solved;
- target users;
- desired deliverables;
- technical stack, if software is intended;
- functional requirements;
- non-functional requirements;
- acceptance criteria;
- deployment target;
- constraints and exclusions.

## Unknowns / hypotheses
- It is unknown whether the ATRSSH call is the core purpose of the project or merely reference material.
- There is currently no evidence of a chosen programming language or application framework.
- There is currently no evidence of a database, API, frontend, backend, mobile app, or deployment environment.

## Next recommended action
Create a formal project specification once the intended product is known. Put it in `docs/SPEC.md`, then derive an implementation roadmap in `docs/ROADMAP.md` and update this state file.

## Handoff snapshot
A new AI should NOT start by rewriting the README or inventing an implementation. Start by reading the memory files, inspecting the tree, and resolving the project-definition gap above.
