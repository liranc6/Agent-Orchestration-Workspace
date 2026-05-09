# Task: App Fixes and Limits

- task: app-fixes-limits
- status: WIP
- owner: ORCHESTRATOR

## Work
- [x] Create user request entry.
- [x] Create internal message thread.
- [ ] Refactor names "You"/"Partner" -> "Liran"/"Vova".
- [x] Optimize `st.rerun()` calls on category selection.
- [x] Implement CSS for green buttons.
- [x] Implement per-user limits and warning system.
- [x] Deploy changes to Streamlit Cloud (push to `deploy` remote).
- [x] Add per-user budget utilization dashboard section.

## Expert Consultation Log
- Expert: `Senior Principal Dev Programmer` | Value: Implemented backward-compatible name mapping and state-check optimizations for buttons.
- Expert: `Expert App Designer` | Value: Provided CSS injection for green branding.
- Expert: `Expert Product Manager` | Value: Specified the 85% threshold logic for user-specific budgets.

## Notes
- Need to ensure backward compatibility for "You" and "Partner" in logs if possible, but user asked for name change.

## Next steps
- Edit `app.py` constants and logic.
