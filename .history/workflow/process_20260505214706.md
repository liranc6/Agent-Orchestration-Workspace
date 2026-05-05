# Process

1. Request intake
- `PM` or `Senior Product` reads request from `user_requests/`.
- Capture mission.
- If unclear, stop and clarify.
- Reply in `user_requests/` for user-facing questions.
- Start a `msgs/` thread for internal team alignment if needed.

2. Clarify mission
- `PM`, `Ambiguity Analyst`, `Senior Agent Dev`, `Senior Dev`, `UX` review.
- Find assumptions, gaps, risks.
- If unclear: `Q? user` + recommendation.
- Repeat until mission is clear.

3. Developer alignment
- Share clarified mission in `msgs/`.
- Confirm no new technical ambiguity.
- If devs have questions: `DEV: Q? <short>` to `PM`.
- `PM` asks user again if needed.

4. Plan and scope
- Define tasks and acceptance.
- Assign `task:` to devs.
- Confirm `DONE` criteria.

5. Build
- `DEV` works, sends `WIP`.
- If blocked: `DEV: BLOCK <reason>`.
- If new question: `DEV: Q? <short>`.
- If requirements change, repeat clarity loop.

6. Review and validate
- `REVIEW` inspects.
- `QA` tests.
- If issue: `REVIEW: PR#<id> changes needed` or `QA: TEST FAIL`.
- Fix and recheck.

7. Delivery
- `QA: TEST PASS`.
- `DEV`: `DONE`.
- `PM`/`OPS` release / handoff.
- `FYI: delivered`.

8. Archive
- Move closed thread or task to `archive/`.
- Keep active folders clean.
