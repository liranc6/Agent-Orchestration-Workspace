# SPEC: Repo Split - Agents Communication Protocol

## 1. Objective
Split the current `Agent-Orchestration-Workspace` (AOW) into two distinct repositories to isolate the core communication protocol from the orchestration implementation.

## 2. Repositories
- **Source/Orchestration Repo:** `Agent-Orchestration-Workspace` (Current)
- **New Communication Repo:** `Agents-Communication-Protocol` (Independent, self-contained)

## 3. Scope of Split
The following components will be migrated to the new `Agents-Communication-Protocol` repository:
- `process/communication_protocol/` (Core Jargon, shorthand, formats)
- `docs/glossary/` (Terms and acronyms)
- `process/workflow/` (Interaction processes that rely on the protocol)
- Relevant templates from `docs/templates/` (e.g., communication-heavy templates)

## 4. Integration Strategy
- The `Agents-Communication-Protocol` repository will be added as a submodule to `Agent-Orchestration-Workspace`.
- Path in AOW: `protocol/` (or similar, to be determined).
- References in AOW documentation (`README.md`, `init/README.md`) will be updated to point to the submodule.

## 5. Success Criteria
- `Agents-Communication-Protocol` is a functional, standalone repository.
- `Agent-Orchestration-Workspace` remains functional using the submodule.
- All documentation links are valid.
- Internal communication still adheres to the Op-Urgency protocol.

## 6. Approvals
- PLANNER: [Approved 2026-05-16]
- REVIEW: [Approved 2026-05-16]
