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
4. `user_requests/README.md`
5. `user_specs/README.md`
6. `msgs/README.md`
7. `tasks/README.md`
8. `decisions/README.md`
9. `glossary/README.md`
10. `dev_team/README.md`
11. `archive/README.md`
12. `specs/README.md`

## Quick start
- Read `init` first.
- Then read `communication_protocol` and `workflow`.
- After that, use `msgs` to coordinate and `tasks` to track work.
- Use `user_requests/` for new requests and follow-up.
- For every new request, also create a `msgs/YYYYMMDD-<topic>/README.md` internal discussion thread.
- For repo improvements, open a request under `user_requests/` and track it in `tasks/`.
- Review `git_management/commit_msg_conventions.md` and follow it for all commit messages.
- If only one agent is active, use `msgs/` to simulate team roles internally with communication protocol syntax.
- Use `decisions` and `glossary` as needed.
- Only use `specs` when you need technical detail.
