# CHANGELOG.md — Project Memory History

All notable project/memory changes are recorded here so a future AI can understand how the repository evolved.

## 2026-08-19
### Added
- `AGENTS.md` — portable operating instructions for AI agents.
- `AI_MEMORY.md` — canonical project context and facts.
- `PROJECT_STATE.md` — living status, unknowns, completed work, and next action.
- `DECISIONS.md` — durable decision log.
- `CHANGELOG.md` — this history.
- `AI_CALIBRATION.md` — evidence hierarchy, uncertainty classification, verification gates, self-checks, and hallucination correction protocol.
- `CORRECTIONS.md` — durable ledger for material AI mistakes and corrections.

### Preserved
- Existing `README.md` and its ATRSSH 2026 research-call reference material.

### Context
The repository was initially almost empty, so the first engineering action was to establish a reliable, transferable project-memory architecture before implementing product code.

### AI reliability layer
The memory system now requires future agents to distinguish verified facts from inference/hypothesis/unknowns, verify consequential claims, avoid inventing missing details, and preserve a correction trail when an error is discovered.
