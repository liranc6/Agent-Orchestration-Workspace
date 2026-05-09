# Consultancy Map

This map helps the **ORCHESTRATOR** and **PLANNER** identify which experts to consult based on the specific challenge or domain of the task.

| Challenge Domain | Primary Expert | Secondary Expert | Trigger |
| :--- | :--- | :--- | :--- |
| **Requirements** | `Expert Ambiguity Analyst` | `Expert Product Manager` | User request is vague or complex. |
| **UX & UI** | `Expert UX/Product Designer` | `Expert App Designer` | New user-facing interfaces or flows. |
| **App Visuals** | `Expert App Designer` | `Expert UX/Product Designer` | Specific app layouts or branding needs. |
| **Architecture** | `Senior Principal Dev Programmer` | `Expert Code Reviewer` | High-level system design decisions. |
| **Infrastructure** | `Expert DevOps / Infrastructure Engineer` | `Senior Agent Developer` | CI/CD, environments, or tool setup. |
| **Quality** | `Expert QA` | `Expert Code Reviewer` | Complex logic requiring deep testing. |
| **Process** | `Expert Agent Reviewer` | `Orchestrator` | Improvements to this repo or workflow. |
| **Risk & Scope** | `Expert Manager` | `Planner` | Task is running over time or blocked. |

## Quick Consultation Guide

- **IF** the user says "I don't know" or "you decide", **THEN** consult `Expert Product Manager`.
- **IF** the task involves editing sensitive configs, **THEN** consult `Expert DevOps / Infrastructure Engineer`.
- **IF** the code changes affect multiple modules, **THEN** consult `Expert Code Reviewer`.
- **IF** you are adding a new agent role, **THEN** consult `Member Creator`.
