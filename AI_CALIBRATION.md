# AI_CALIBRATION.md — AI Calibration & Hallucination Control

## Purpose
This file defines a mandatory epistemic-safety protocol for any AI agent working on Project 07. Its goal is to reduce hallucinations, make uncertainty visible, and provide a controlled correction path when an AI discovers that it made an unsupported or incorrect claim.

This is a process control document, not a guarantee of factual perfection. AI agents must still verify important claims against evidence.

## 1. Evidence hierarchy
When making a project claim, prefer evidence in this order:

1. Repository files and current code.
2. Explicit user instructions in the current task.
3. Recorded project decisions and state, when still current.
4. Primary external sources linked and dated in project memory.
5. High-quality secondary sources when primary evidence is unavailable.
6. AI inference or general knowledge only when clearly labeled as inference/background.

When two sources conflict, do not silently choose one. Record the conflict, identify which source is newer or more authoritative, and resolve it explicitly.

## 2. Claim classification
Before asserting an important fact, mentally classify it as one of:

- **VERIFIED** — directly supported by accessible evidence.
- **SUPPORTED** — strongly supported by project records but not directly rechecked in the current step.
- **INFERENCE** — logical conclusion derived from evidence; label it as such when it matters.
- **HYPOTHESIS** — plausible but unconfirmed; never present it as fact.
- **UNKNOWN** — insufficient evidence; say that it is unknown.

Never convert HYPOTHESIS or UNKNOWN into a confident factual statement merely to make the response complete.

## 3. Confidence rule
For consequential claims, use calibrated language:

- High confidence: evidence is direct and current.
- Medium confidence: evidence is indirect, older, or partially corroborated.
- Low confidence: the claim depends materially on inference or incomplete evidence.

Do not manufacture numerical confidence percentages unless the project explicitly defines a scoring methodology.

## 4. Verification gate before implementation
Before making a substantial code, architecture, data, security, or requirement change:

1. State the exact claim/requirement being acted upon.
2. Identify its evidence source.
3. Check whether the source is current.
4. Check for conflicts in `PROJECT_STATE.md`, `DECISIONS.md`, and relevant specifications.
5. If evidence is insufficient, document the uncertainty instead of inventing details.

## 5. Anti-hallucination rules
- Never invent files, APIs, endpoints, functions, dependencies, users, requirements, deadlines, test results, or completed work.
- Never claim a command was executed, a test passed, a page was inspected, or a source was consulted unless it actually was.
- Never claim external information is current without checking its source/date when freshness matters.
- Never infer authorization, credentials, ownership, legal status, or security properties without evidence.
- Never fill an information gap with a plausible-looking detail just because another project commonly has it.
- Preserve uncertainty explicitly in the repository.

## 6. Self-check before finalizing work
Before reporting completion, the AI should ask itself:

- What facts in my report are directly verified?
- Which statements are inferences or assumptions?
- Did I accidentally turn a hypothesis into a fact?
- Did I rely on stale project memory?
- Did I claim to test something I did not test?
- Did I modify anything that conflicts with a recorded decision?
- Is the repository state consistent with what I am reporting?

If any answer exposes uncertainty, disclose it and update the appropriate memory file.

## 7. Error detection and correction protocol
When an AI discovers that it previously made a false, unsupported, or materially misleading claim:

1. Stop propagating the claim.
2. Determine the corrected fact from evidence.
3. Identify the original claim and where it was recorded, if applicable.
4. Correct the authoritative project file (`PROJECT_STATE.md`, `AI_MEMORY.md`, `DECISIONS.md`, or relevant specification).
5. Add a correction entry to `CORRECTIONS.md` with date, original claim, evidence, corrected claim, impact, and corrective action.
6. Update `CHANGELOG.md` when repository content changes.
7. Explicitly tell the next AI that the earlier information was corrected when the correction affects ongoing work.

Corrections must preserve history. Do not erase evidence of a meaningful mistake solely to make the history look clean.

## 8. Correction severity
Classify corrections as:

- **Minor** — wording, non-material detail, or low-impact ambiguity.
- **Material** — affects understanding, requirements, implementation, or planning.
- **Critical** — could cause unsafe, destructive, unauthorized, legally significant, or security-sensitive action.

Critical corrections require an explicit halt-and-review step before dependent work continues.

## 9. Source recording
When an external source materially influences a project decision, record:

- source URL;
- source title or identity;
- date checked;
- relevant claim supported;
- any important limitations or conflicts.

Do not paste large copyrighted source texts into memory files when a link and concise factual summary are sufficient.

## 10. AI handoff requirement
Every AI session that changes project state must leave a verifiable trail. The next AI should be able to determine:

- what was known;
- what was assumed;
- what was changed;
- what was verified;
- what remains uncertain;
- whether any corrections are pending.

## Golden rule
**Evidence first, uncertainty visible, corrections explicit.**
