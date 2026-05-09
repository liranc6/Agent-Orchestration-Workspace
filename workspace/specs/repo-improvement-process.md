# Repo Improvement Process

- Purpose: document how to request, track, and complete repository improvements in this developer tool repo.
- Use this file for internal guidance on repo maintenance, documentation updates, and structural improvements.

## When to use
- The repository itself needs clearer structure or documentation.
- New folder conventions, onboarding changes, or repo workflow updates are required.
- The repo improvement work is internal and not a product feature.

## Process
1. Create a user request in `user_requests/YYYYMMDD-<topic>/README.md`.
2. Track the work in `tasks/YYYYMMDD-<topic>.md`.
3. Capture user-facing requirements in `user_specs/` if the change should be visible to users.
4. Document internal implementation or process decisions in `specs/`.
5. Use `archive/` for completed requests and tasks once the work is finalized.

## Roles
- `user_requests/` holds the request intake and visible status for the user.
- `tasks/` holds the active work item, owner, and next steps.
- `user_specs/` holds agreed requirements for user-facing repo changes.
- `specs/` holds technical or process documentation that supports the repo improvement.

## Guidelines
- Keep user request text short, clear, and focused on the outcome.
- Keep task progress updated and concrete.
- Avoid mixing internal role-play messages into `user_requests/` or `user_specs/`.
- Use `msgs/` for internal discussion when needed.
- Document the final state and any follow-up steps before closing a task.
