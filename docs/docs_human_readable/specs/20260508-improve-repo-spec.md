# Spec: Workspace Improvement - Expert Utilization

- date: 2026-05-08
- status: DRAFT
- task: 20260508-improve-repo

## Overview
The goal is to improve the results the user gets from the agent team by making the "AI Experts" more accessible, specialized, and integrated into the workflow.

## Proposed Changes

### 1. Unified Expert Interaction Protocol
Create a new file [dev_team/INTERACTION_PROTOCOL.md](dev_team/INTERACTION_PROTOCOL.md) that defines *how* and *when* to invoke specific experts. 
- **Discovery Phase:** Use `Expert Ambiguity Analyst` and `Expert Product Manager`.
- **Planning Phase:** Use `Planner` and `Orchestrator`.
- **Implementation Phase:** Use `Senior Principal Dev Programmer`.
- **Verification Phase:** Use `Expert QA` and `Expert Code Reviewer`.

### 2. Expert Specialist Role Enhancement
Update individual expert files in `dev_team/` to include:
- "Key Skills"
- "Trigger Events" (when to use them)
- "Output Expectation" (what they should provide)

### 3. Template Updates
Update `templates/task-template.md` to include a section for "Expert Consultation Log" to track which experts were used and what value they added.

### 4. Role Discovery improvements
Update [dev_team/README.md](dev_team/README.md) to categorize roles into "Core Team", "Consultants", and "Quality & Oversight".

## Impact
Users will have a clearer mental model of the virtual team, leading to higher quality outputs and more efficient delegation.
