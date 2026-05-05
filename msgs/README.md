# Messages

- `user_requests/` = user request intake and user-team chat.
- `msgs/` = internal team chat only.
- Use `user_requests/` for user-facing messages and questions.
- Keep messages short and on-topic.
- Support sub-threads by using dedicated dirs for each request and thread.
- Use `@role` or `@name` for direct attention in messages.
- New member start with `../init/README.md`.
- For agent-driven requests, explicitly simulate reviewer feedback and back-and-forth communication.
- Include the Senior Agent Developer and Expert Agent Reviewer roles when the request is about agents or repo process.

## Structure
- One thread per request/issue.
- Use sub-channels only for parallel work.
- Keep each thread focused.

## Use
- Start thread: `task: <short>`.
- Update with `WIP`, `Q?`, `BLOCK`, `DONE`, `ACK`.
- Append new messages as work progresses; do not leave the thread as a summary written only at the end.
- If thread is >2 lines, create a doc and link it.
- Use the syntax in `[[../communication_protocol/format.md]]` for role-prefixed messages.
- Link `[[../communication_protocol/README]]` for rules.
- See `single-agent-role-play.md` for a single-agent role-play example.
