# Single-Agent Role-Play Example

- Purpose: show how one agent can simulate multiple roles using `msgs/`.
- Use this pattern when only one agent is active but the process still needs role separation.
- For agent-related requests, include the Senior Agent Developer and an Expert Agent Reviewer.

## Example

DEV: task: start branch `feature/git-guidance` and implement git guidance docs
REVIEW: task: check docs for clarity, consistency, and protocol compliance
DEV: note: updated repo docs and added review workflow guidance
SENIOR AGENT DEVELOPER: note: ensure agent communication roles and review flow are included
REVIEW: ask: does this meet the request and is it deliverable?
QA: task: verify guidance is complete and actionable
REVIEW: decision: result is deliverable, or more work is needed if gaps remain
PM: note: confirm changes align with repo improvement goals and mark ready for user confirmation
