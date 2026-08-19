# DECISIONS.md — Decision Log

This file records decisions that affect how future agents should interpret or modify the project.

## D-001 — Repository acts as durable project memory
- Date: 2026-08-19
- Status: accepted
- Decision: Treat the repository documentation as the persistent memory of Project 07.
- Reason: The project must be transferable between different AI systems without relying on conversation history.
- Consequence: Important context, decisions, current state, and handoff instructions must be committed to the repository.

## D-002 — Keep human source material intact
- Date: 2026-08-19
- Status: accepted
- Decision: Preserve the pre-existing `README.md` content rather than replacing it with AI-oriented documentation.
- Reason: It is the original project/reference material and may contain requirements or useful external context.
- Consequence: AI-specific memory lives in dedicated files and the README can remain human-facing.

## D-003 — Separate facts from assumptions
- Date: 2026-08-19
- Status: accepted
- Decision: Unknown project details must be explicitly marked as unknown instead of inferred as facts.
- Reason: Portability is only useful if the memory is trustworthy.
- Consequence: Future agents must document hypotheses and update them when evidence becomes available.
