# Git Management

- Purpose: define how developers should use Git, when to commit, and how to write commit messages.
- This document guides autonomous commit work and the review handoff.

## Use Git autonomously
- Commit frequently.
- Commit each self-contained logical change, bug fix, or refactor.
- Do not wait for approval to make local commits.
- Keep work small and reviewable.
- Verify tests/builds locally before pushing when possible.

## Branch workflow
- Use a dedicated branch for each task or request.
- Suggested branch names:
  - `feature/<short-description>`
  - `fix/<short-description>`
  - `chore/<short-description>`
- Make each branch goal clear in the name.
- Keep branches focused on one purpose.

## When to commit
- After completing a small, coherent piece of work.
- After fixing a bug or addressing a review point.
- After updating tests or documentation.
- Before switching contexts or starting a new work item.
- See `commit_frequency.md` for additional commit rhythm guidance.

## Commit message rules
- Follow `commit_msg_conventions.md` for the team commit message standard.
- Use an imperative summary line.
- Keep the first line short and descriptive.
- Add an optional body for context if needed.
- Use clear prefixes when helpful:
  - `feat:` for new functionality
  - `fix:` for bug fixes
  - `docs:` for documentation changes
  - `chore:` for maintenance
  - `refactor:` for code improvements
- Example messages:
  - `feat: add git management guidelines`
  - `fix: correct communication_protocol folder references`
  - `docs: document commit message style`

## Push and review process
- Push when the branch is ready for review.
- Open a PR or request a code review for the branch.
- Summarize what changed, why, and any verification steps.
- Link the relevant task or user request.

## Single-agent team simulation
- If only one agent is available, it may play all team roles itself.
- Use `msgs/` for internal role-based dialogue and keep user-facing content separate.
- Prefix internal messages with the active role using communication protocol syntax, for example:
  - `DEV: task: implement git guidance`
  - `REVIEW: task: check docs for clarity and consistency`
  - `QA: task: verify guidance is testable and complete`
  - `PM: note: confirm changes align with repo improvement goals`
- Keep each internal message focused on the role’s responsibility.
- Do not mix internal role-play messages into `user_requests/` or `user_specs/`.
- Final decisions, approvals, and specs should be documented clearly and readably.

## Code review ownership
- Expect the `Expert Code Reviewer` to handle all code reviews.
- Assign or tag the reviewer on PRs.
- The reviewer checks quality, patterns, design, and merge readiness.
- Developers continue to own their commits and respond to feedback.

## Best practice
- Keep each commit atomic and understandable.
- Avoid large, mixed changes in one commit.
- Use meaningful commit messages for future traceability.
- Treat Git as the source of truth for progress and intent.
