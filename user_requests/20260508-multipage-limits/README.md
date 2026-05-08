# Request: Separate Limits Configuration Page

- request: Create a separate page in the app to view and change category limits per user.
- user: liranc6

## Acceptance criteria
- [x] Navigation between "Dashboard" and "Limits" pages.
- [x] Limits page allows editing `BUDGET_TARGETS` for Liran and Vova.
- [x] Changes to limits persist for the session (saved to `limits.json`).
- [x] Limits are respected by the dashboard warnings.

## Status
- `task: multipage-limits`
- `COMPLETED`

## Progress
- Initiated intake.
- Implemented `render_limits_page()` in `app.py`.
- Added `limits.json` for persistent storage.
- Integrated sidebar navigation.

## Next steps
- Archive task records.
