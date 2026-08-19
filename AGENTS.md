# AGENTS.md — Project 07 AI Operating Instructions

## Purpose
This file is the entry point for any AI agent that opens this repository.
The repository itself is the durable memory of Project 07. Do not depend on prior chat history.

## First-read protocol
Before changing anything:
1. Read `AGENTS.md`.
2. Read `AI_MEMORY.md`.
3. Read `PROJECT_STATE.md`.
4. Read `DECISIONS.md`.
5. Read the current `README.md` and inspect the repository tree.
6. Read the latest entries in `CHANGELOG.md`.

## Source of truth
- Current project reality: `PROJECT_STATE.md`
- Long-term project context: `AI_MEMORY.md`
- Decisions and rationale: `DECISIONS.md`
- Change history: `CHANGELOG.md`
- Human-facing project/reference material: `README.md`

When documents disagree, prefer the newest explicit decision/state entry and document the resolution in `DECISIONS.md` or `PROJECT_STATE.md`.

## Non-negotiable behavior
- Never invent project facts, requirements, files, people, deadlines, or completed work.
- Preserve existing useful source material unless the task explicitly requests removal.
- Before implementing a substantial change, update the project state/plan when appropriate.
- After implementing a change, record what changed in `CHANGELOG.md` and update `PROJECT_STATE.md` if the current state has changed.
- Keep documentation synchronized with the repository. A future AI must be able to understand the project without asking the previous AI.
- Use clear, stable filenames and avoid putting critical knowledge only in chat.
- Do not store secrets, tokens, passwords, private keys, or personal authentication material in the repository.
- When external information is used, record the source URL and the date checked in the relevant memory/decision file.

## Working style
Prefer small, reversible changes. Explain intent in commit messages. Keep generated artifacts separate from authoritative documentation.

## Handoff requirement
At the end of a work session, leave enough information for another AI to continue immediately:
- what was requested;
- what was inspected;
- what was changed;
- what remains;
- blockers/unknowns;
- next recommended action.
