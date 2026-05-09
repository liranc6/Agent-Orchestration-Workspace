# Request: App Performance, Colors, User Names, and Per-User Limits

- request: Fix slow category selection, change button color to green, update user names to Liran/Vova, and implement per-user category limits with 85% warnings.
- user: liranc6

## Acceptance criteria
- [x] Category selection is faster (optimize fragments/reruns).
- [x] Selected button color is green (custom CSS injection).
- [x] "You" and "Partner" replaced with "Liran" and "Vova" (with backward compatibility).
- [x] Per-user category limits can be set.
- [x] Warning shows when 85% of limit is reached.

## Status
- `task: app-fixes-limits`
- `COMPLETED`

## Progress
- Initiated intake.
- Updated `app.py` constants and UI logic.
- Injected custom CSS for branding.
- Implemented per-user budget monitoring in the sidebar.

## Next steps
- Archive task records.
