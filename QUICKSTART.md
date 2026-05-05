# Quickstart

This repository is an agent orchestration workspace for a developer to add to their environment and direct an AI team to deliver tasks.

## Quickstart steps

1. Clone this repo into your workspace.
2. Read `init/README.md` and `QUICKSTART.md`.
3. Create a request under `user_requests/YYYYMMDD-<topic>/README.md`.
4. Start an internal coordination thread under `msgs/YYYYMMDD-<topic>/README.md`.
5. Track active work in `tasks/YYYYMMDD-<topic>.md`.
6. Use `dev_team/` roles and `specs/` docs to align execution.
7. Archive finished requests and tasks in `archive/`.

## Example flow

- `user_requests/20260506-add-feature/README.md`: request intake.
- `msgs/20260506-add-feature/README.md`: internal coordination.
- `tasks/20260506-add-feature.md`: execution plan and status.
- `archive/`: closed request and task files.

## Notes

- This repo is intentionally lightweight and documentation-first.
- Use the templates in `templates/` to create consistent requests, tasks, and evaluation notes.
- The repo is not an autonomous agent runtime, but it is a workspace for directing agents and tracking their output.
