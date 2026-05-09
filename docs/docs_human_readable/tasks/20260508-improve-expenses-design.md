# Task: Improve Expenses App Design

- task: improve-expenses-design
- status: WIP
- owner: ORCHESTRATOR

## Work
- [x] Create user request entry.
- [x] Create internal message thread.
- [x] Audit existing app UI structure.
- [x] Create design improvement spec.
- [x] Implement UI changes:
    - [x] Upgrade balances to `st.metric`.
    - [x] Add emojis to categories in lists and charts.
    - [x] Improve layout of "Quick Summary" using Streamlit containers.
    - [x] Style the sidebar for better accessibility.
- [x] Verify features are intact.

## Expert Consultation Log
- Expert: `Expert App Designer` | Value: Provided visual hierarchy audit and identified Streamlit-specific improvements (metrics, emojis).
- Expert: `Senior Principal Dev Programmer` | Value: Identified `app.py` as the layout engine.
- Expert: `Supervisor` | Value: Verified functional parity after UI changes.

## Notes
- Focus on `expenses_app/` folder and root `app.py`.

## Next steps
- Run `list_dir` on `expenses_app/` and read `app.py`.
