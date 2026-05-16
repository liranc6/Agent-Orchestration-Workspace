# Quickstart

This repository is an agent orchestration workspace for a developer to add to their environment and direct an AI team to deliver tasks.

## 1. Installation (Recruit the Team)

Add this workspace to your existing application as a submodule:

```bash
git submodule add https://github.com/liranc6/Agent-Orchestration-Workspace.git
git submodule update --init --recursive
```

*Alternatively, clone it directly if you are starting a new project.*

## 2. Quickstart steps

1. Read `init/README.md`, `QUICKSTART.md`, and `docs/git_management/README.md`.
2. **SYNTAX CHECK:** Ensure you are familiar with **Op-Urgency** jargon in `protocol/` and **Git Commit** formats in `docs/git_management/`. Non-compliance is a protocol failure.
3. Create a request under `user_requests/YYYYMMDD-<topic>/README.md`.
3. Start an internal coordination thread under `msgs/YYYYMMDD-<topic>/README.md` before any implementation or edit work.
4. Track active work in `tasks/YYYYMMDD-<topic>.md`.
5. Use `dev_team/` roles, `specs/` docs, and `git_management/` guidance to align execution.
6. Archive finished requests and tasks in `archive/`.

## Example flow

- `user_requests/20260506-add-feature/README.md`: request intake.
- `msgs/20260506-add-feature/README.md`: internal coordination.
- `tasks/20260506-add-feature.md`: execution plan and status.
- `archive/`: closed request and task files.

## Notes

- This repo is intentionally lightweight and documentation-first.
- Use the templates in `templates/` to create consistent requests, tasks, and evaluation notes.
- The repo is not an autonomous agent runtime, but it is a workspace for directing agents and tracking their output.
