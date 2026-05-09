# Team Interaction Protocol

This document defines how the virtual agent team interacts and when specific experts should be consulted during the task lifecycle.

## Task Lifecycle & Expert Invocations

### 1. Intake & Discovery
- **Trigger:** New entry in `user_requests/`.
- **Experts:** `Expert Ambiguity Analyst`, `Expert Product Manager`.
- **Output:** Defined acceptance criteria and clarified requirements.

### 2. Planning & Strategy
- **Trigger:** Requirements are clear.
- **Experts:** `Planner`, `Orchestrator`, `Expert UX/Product Designer`.
- **Output:** Technical spec in `specs/` and task list in `tasks/`.

### 3. Implementation
- **Trigger:** Plan is approved.
- **Experts:** `Senior Principal Dev Programmer`, `Junior Dev Programmer`, `Expert DevOps / Infrastructure Engineer`.
- **Output:** Code changes, file creations, and technical execution.
- **Constraint:** ALL internal team synchronization in `msgs/` MUST use the **Op-Urgency** Jargon (defined in `communication_protocol/`). Non-compliance is a protocol failure.

### 4. Quality Assurance & Review
- **Trigger:** Implementation is complete.
- **Experts:** `Expert QA`, `Expert Code Reviewer`, `Expert Agent Reviewer`.
- **Output:** Test results, review notes, and final validation.

### 5. Evaluation & Handoff
- **Trigger:** Task is ready for final delivery.
- **Experts:** `Evaluator`, `Supervisor`.
- **Output:** Final review summary and archival.

## Consulting Experts
When a core agent (e.g., ORCHESTRATOR) needs deep expertise:
1. Identify the need (e.g., "I need a security audit").
2. Invoke the expert role (e.g., CONSULT: `Expert DevOps / Infrastructure Engineer`).
3. Log the consultation in the `tasks/` entry.
