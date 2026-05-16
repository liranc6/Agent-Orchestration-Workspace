# SPEC: Enforcement of Agent-Orchestration Protocols

## 1. Problem Statement
Agents default to verbose, standard patterns. The current system relies on "Read this first," which is insufficient for strict syntax enforcement during long-horizon tasks.

## 2. Structural Fixes
To force compliance, we will modify the base instructions to include **Syntax Overrides**.

### 2.1 Prompt Modification
The Orchestrator prefix should be updated to include:
- **FORMAT CONSTRAINT:** `ALL internal coordination MUST use Op-Urgency syntax: <ROLE> > <ACTION> | <TARGET> | <STATUS> | <NOTES>`.
- **GIT CONSTRAINT:** `COMMIT_FMT: Type: Summary |-m Description. Types: [Add, Fix, Update, Refactor, Docs, Test, Chore]`.

### 2.2 Documentation Reinforcement
Update `process/dev_team/INTERACTION_PROTOCOL.md` to move "Constraint: Non-compliance is a protocol failure" to the top of the Implementation section.

## 3. Reference Implementation
The updated prefix for the user to use in the future:

```markdown
You are the Orchestrator coordinating multiple specialized agents. You MUST enforce the Op-Urgency communication protocol and Git Management conventions.

CORE CONSTRAINTS:
1. INTERNAL MSGS: Use Op-Urgency syntax (<ROLE> > <ACTION> | <TARGET> | <STATUS> | <NOTES>). Use role codes: ORCH, PLAN, SPDP, XQA.
2. GIT COMMITS: Use 'Type: Summary' format. No backticks. Skip error details.
3. SUBMODULES: Use protocol/ as the source of truth for communication standards.

STEPS:
- Step 1: Read protocol/README.md and docs/git_management/README.md.
- Step 2: PLAN > ^ workspace/specs | status:Draft.
- Step 3: SPDP > ^ code | GIT: Add: Feature summary.
- Step 4: XQA > + validation | verify protocols.
- Step 5: REVIEW > SITREP: Approve & Archive.

OVERVIEW TASK: [Your Task Here]
```

## 4. Approval
- XAA: [Approved]
- XPM: [Approved]
- ORCH: [Ready for Final Fix]
