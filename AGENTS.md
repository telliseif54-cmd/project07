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
5. Read `AI_CALIBRATION.md`.
6. Read `CORRECTIONS.md`.
7. Read the current `README.md` and inspect the repository tree.
8. Read the latest entries in `CHANGELOG.md`.

## Source of truth
- Current project reality: `PROJECT_STATE.md`
- Long-term project context: `AI_MEMORY.md`
- Decisions and rationale: `DECISIONS.md`
- AI verification / anti-hallucination protocol: `AI_CALIBRATION.md`
- Known AI errors and corrections: `CORRECTIONS.md`
- Change history: `CHANGELOG.md`
- Human-facing project/reference material: `README.md`

When documents disagree, prefer the newest explicit decision/state entry and document the resolution in `DECISIONS.md` or `PROJECT_STATE.md`.

## Non-negotiable behavior
- Never invent project facts, requirements, files, people, deadlines, or completed work.
- Preserve existing useful source material unless the task explicitly requests removal.
- Before implementing a substantial change, verify the requirement against repository evidence and `AI_CALIBRATION.md`.
- Before making consequential claims, distinguish verified facts from inference, hypothesis, and unknowns.
- Never claim a test, command, source lookup, deployment, or inspection occurred unless it actually occurred.
- When an error is discovered, follow `AI_CALIBRATION.md` and record material corrections in `CORRECTIONS.md`.
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
- what was verified;
- what remains;
- blockers/unknowns;
- whether any corrections were made;
- next recommended action.
