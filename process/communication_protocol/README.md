# Communication Protocol

- Purpose: approved team messaging style and tokens.
- Use only for chat rules and shorthand.
- All docs outside `/specs` use this compact style.

## Folders
- `user_requests/` = user request intake and user-team chat
- `user_specs/` = user-facing product specs
- `msgs/` = live team chat only
- `workflow/` = process rules and handoff steps
- `communication_protocol/` = approved shorthand and format
- `tasks/` = actual work items and status
- `decisions/` = formal decisions and reasons
- `archive/` = closed or old threads/docs
- `glossary/` = terms, acronyms, team shorthand

## Notes
- Use `[[format]]`, `[[acronyms]]`, `[[common-phrases]]`, `[[../msgs/README]]`, `[[../glossary/README]]`, `[[../init/README]]`.
- Keep lines short.
- Use `Q?` for questions, `ACK` for receipt.
- If a doc grows beyond 2 lines, link it, do not expand chat.
- Team communication supports Obsidian-like folder structure and sub-threads.
- Use `@role` or `@name` when you need direct attention.
- If one agent is acting as multiple roles, keep internal messages in `msgs/` and use role-prefixed syntax.
- Before any execution/edit step, open or update the matching `msgs/YYYYMMDD-<topic>/README.md` thread.
- Use `ORCH > ACK`, `XAA > r/o`, `XPM > decision`, `PLAN > scope`, `SPDP > WIP/DONE`, `XQA > note` in that thread before implementation starts.
- If the thread is missing, create it first; do not begin code changes before the internal coordination exists.

## No redundancy
- Avoid filler words and articles.
- Prefer `task: book` not `task: a book`.
- Prefer `need info` not `I need more info`.
- Prefer `confirm` not `please confirm`.
- Prefer `done` not `finished successfully`.
- Prefer `deploy prod` not `deploy to production environment`.
