# Message Frequency: Operational Urgency

- Purpose: Maximize operational tempo while minimizing token footprint.

## Rule: Military Brevity
- **Dense Notation**: Only use symbols and acronyms defined in `format.md` and `acronyms.md`.
- **Zero Filler**: Delete all articles (a, an, the) and conjugation (is, are, was).
- **Snapshot Logic**: Messages should read like a medical chart or radio Sitrep.
- **Link-Heavy**: If an explanation takes >1 line, move it to `specs/` or `notes/`.

## Snapshot Update Rule
- Updates only at `HVT` (High Value Task) milestones.
- Batch multiple role outputs into a single SITREP to save file-header tokens.
- Add a new message for each meaningful progress step, decision, question, or block.
- Update the thread when work changes state: `WIP`, `BLOCK`, `ACK`, or `DONE`.
- Do not leave the thread idle as a single summary at the end.

## How often
- Post updates at natural checkpoints, such as:
  - when a task starts
  - when a question is asked or answered
  - when a request is clarified
  - when a decision is made
  - when work is completed
- For short tasks, keep updates brief and frequent.
- For longer tasks, add regular status notes instead of batching everything into one message.

## When to create a dedicated doc
- If a thread grows beyond 2–3 messages of detailed discussion, create a dedicated doc and link it from the thread.
- Use dedicated docs for complex design notes, long decision rationale, or process guidelines.
- Keep the `msgs/` thread as the navigation point and summary of what happened.

## Single-agent note
- When one person is simulating multiple roles, follow the same update frequency.
- Use role-prefixed messages and maintain a live internal chat cadence.
