# Contributing

This repo is a documentation-driven developer tool for a virtual AI team.
Use this guide to contribute improvements, create requests, and keep the repo consistent.

## Start here
1. Read `init/README.md` first.
2. Review `communication_protocol/README.md` and `workflow/README.md`.
3. Use `user_requests/` for new user-facing requests.
4. Track active work in `tasks/`.
5. Store technical decisions in `specs/` and user-facing requirements in `user_specs/`.
6. Keep internal discussion in `msgs/` when needed.

## Repo improvement workflow
- Create the request in `user_requests/YYYYMMDD-<topic>/README.md`.
- Track the change in `tasks/YYYYMMDD-<topic>.md`.
- Document internal process in `specs/`.
- When complete, archive closed items to `archive/`.

## Git workflow
- Use a dedicated branch for each request or task.
- Suggested branch names:
  - `feature/<short-description>`
  - `fix/<short-description>`
  - `chore/<short-description>`
- Commit small, self-contained changes.
- Follow `git_management/commit_msg_conventions.md` for commit messages.

## Documentation style
- Keep prose concise and actionable.
- Use the compact format from `workflow/README.md`.
- Avoid mixing user-facing content with internal role-play messages.
- Keep active folders clean by archiving completed work.

## Notes
- If only one agent is active, use `msgs/` to simulate internal roles.
- Do not place internal process or review chatter inside `user_requests/` or `user_specs/`.
- Link the relevant request, task, or spec in any PR or update.
