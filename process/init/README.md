# Init

- Purpose: onboarding starting point for the developer tool.
- This repo is built for a developer who manages a virtual AI team.
- It serves as a workspace the developer can add to their environment to orchestrate agents and deliver tasks through the team.
- Use this file first.

## Folders
- `git_management/` = git workflow and commit guidance
- `user_requests/` = user request intake and user-team chat
- `user_specs/` = user-facing product specs
- `msgs/` = internal team chat only
- `workflow/` = process rules and handoff
- `communication_protocol/` = shorthand and format
- `tasks/` = work items and status
- `decisions/` = formal decisions
- `archive/` = closed content
- `glossary/` = terms and acronyms
- `dev_team/` = roles and skills
- `specs/` = technical documentation and implementation notes

## Read order
1. `init/README.md`
2. `communication_protocol/README.md`
3. `workflow/README.md`
4. `git_management/README.md`
5. `user_requests/README.md`
6. `user_specs/README.md`
7. `msgs/README.md`
8. `tasks/README.md`
9. `decisions/README.md`
10. `glossary/README.md`
11. `dev_team/README.md`
12. `archive/README.md`
13. `specs/README.md`

## Quick start
- Read `init` first.
- Then read `QUICKSTART.md`, `communication_protocol`, `workflow`, and `git_management`.
- After that, use `msgs` to coordinate and `tasks` to track work.
- Use `templates/` for consistent requests, tasks, message threads, and evaluations.
- Use `user_requests/` for new requests and follow-up.
- For every new request, also create a `msgs/YYYYMMDD-<topic>/README.md` internal discussion thread.
- For repo improvements, open a request under `user_requests/` and track it in `tasks/`.
- Review `git_management/README.md`, `git_management/commit_msg_conventions.md`, and `git_management/commit_frequency.md` before committing or pushing.
- If only one agent is active, use `msgs/` to simulate team roles internally with communication protocol syntax.
- Use `decisions` and `glossary` as needed.
- Only use `specs` when you need technical detail.
