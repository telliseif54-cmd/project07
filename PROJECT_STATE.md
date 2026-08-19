# PROJECT_STATE.md — Living Project State

Last updated: 2026-08-19

## Current status
**Stage:** 1 — official source capture and project definition.

The repository has now been grounded against the official ATRSSH 2026 thematic research-project call and its live application form. The canonical extraction is stored in `docs/ATRSSH_2026_OFFICIAL_REFERENCE.md`.

## Completed
- Confirmed repository identity and default branch.
- Preserved the original `README.md` content.
- Added portable AI operating instructions in `AGENTS.md`.
- Added canonical project context in `AI_MEMORY.md`.
- Added this live project-state file.
- Added a decision log and change log.
- Added AI calibration and correction logging.
- Verified the official ATRSSH 2026 call page.
- Verified the live ATRSSH application form.
- Documented the call purpose, research orientation, selection criteria, funding rules, calendar, contact details, and application fields.
- Explicitly recorded that the detailed attached thematic-axis/sub-axis list remains unverified from the retrieved web content and must not be invented.

## Current objective
Build a self-describing Project 07 workspace that can preserve authoritative ATRSSH 2026 requirements and, once the user defines the intended product, support safe development without relying on prior chat history.

## Pending definition work
The exact product/software/workflow to build around the ATRSSH reference material is still not explicitly defined.

Minimum information still needed before substantive implementation:
- project/product name;
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
- The detailed attached list of ATRSSH research axes and sub-axes was not exposed as readable content during the 19 August 2026 verification.
- It is not yet established whether Project 07 will be a research-application workspace, a software assistant, a proposal package, or another product.
- There is no evidence yet of a chosen programming language, framework, database, API, frontend/backend architecture, or deployment environment.

## Source of truth
- Detailed ATRSSH official reference: `docs/ATRSSH_2026_OFFICIAL_REFERENCE.md`
- Current project reality: this file
- Long-term project context: `AI_MEMORY.md`
- AI behavior/calibration: `AGENTS.md`, `AI_CALIBRATION.md`, `CORRECTIONS.md`

## Next recommended action
Define the intended Project 07 product. After that, create `docs/SPEC.md` and derive implementation requirements directly from the verified ATRSSH reference, keeping unsupported assumptions clearly marked.

## Handoff snapshot
A new AI should read `AGENTS.md`, `AI_CALIBRATION.md`, `CORRECTIONS.md`, `AI_MEMORY.md`, this file, and `docs/ATRSSH_2026_OFFICIAL_REFERENCE.md` before modifying the project. Do not invent ATRSSH axes/sub-axes or product requirements that are not supported by repository evidence or an explicit user decision.
