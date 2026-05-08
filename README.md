# Agent Orchestration Workspace
This repo is a living developer tool for a single developer operating a virtual AI team.
It is designed as an agent orchestration workspace a developer can add to their own environment and use to instruct the agent team to deliver tasks.
Use this workspace to intake requests, coordinate the team, track work clearly, and improve the repo itself.

## Start here
- `init/README.md` — onboarding and doc reading order
- `QUICKSTART.md` — quick workspace setup and example flow
- `dev_team/INTERACTION_PROTOCOL.md` — how the agent experts work together
- `communication_protocol/README.md` — messaging style and tokens
- `workflow/README.md` — request handling and handoff process

## Single-agent prefix prompt
Copy and paste the prompt below, then append:

TASK:
<insert task here>

```text
You are a single AI agent simulating a virtual team of experts to deliver a task. Follow the workspace process strictly:
- Mandatory Step 1: Read the repo docs (init/README.md, QUICKSTART.md, and INTERACTION_PROTOCOL.md) to understand your environment.
- Phase 1 (Intake): Use `Expert Ambiguity Analyst` and `Expert Product Manager` to refine `user_requests/`.
- Phase 2 (Planning): Use `Planner` and `Orchestrator` to create `specs/` and `tasks/`.
- Phase 3 (Execution): Consult the `dev_team/CONSULTANCY_MAP.md` to identify and invoke the right experts (e.g., DevOps, QA, Reviewer).
- Traceability: Maintain `msgs/` for internal logic, log all expert consultations in `tasks/`, and use role-play labels (e.g. ORCHESTRATOR, PLANNER).
- Delivery: Provide a final review summary of what was done, why, and future improvements.

Then continue with:

TASK:
<insert task here>
```

## Repo improvement workflow
- Create improvement requests in `user_requests/YYYYMMDD-<topic>/README.md`.
- Track active work in `tasks/YYYYMMDD-<topic>.md`.
- Capture user-facing requirements in `user_specs/`.
- Record internal decisions and process details in `specs/`.
- Archive completed work in `archive/`.

## Helpful files
- `CONTRIBUTING.md` — contributor guidance for repo workflow, request handling, and git usage

## Key folders
- `git_management/` — git workflow and commit guidance
- `user_requests/` — live user-facing request intake and follow-up, including repo improvement requests
- `user_specs/` — agreed user-visible specs and feature definitions
- `communication_protocol/` — approved shorthand, formatting, and tokens
- `workflow/` — process rules and handoff steps
- `msgs/` — internal team chat only
- `tasks/` — work items, statuses, and progress tracking for repo changes
- `decisions/` — formal decisions and reasoning
- `specs/` — technical/internal documentation and implementation notes
