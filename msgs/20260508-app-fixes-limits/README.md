# Internal Thread: App Fixes and Limits

- Purpose: Address performance, styling, names, and budget logic.

## Thread

ORCHESTRATOR: User has 4 specific requests. 
ORCHESTRATOR: CONSULT: `Senior Principal Dev Programmer` for performance and names.
ORCHESTRATOR: CONSULT: `Expert App Designer` for the green button request.
ORCHESTRATOR: CONSULT: `Expert Product Manager` for the limit/warning logic.

SENIOR PRINCIPAL DEV PROGRAMMER: Updated user names to "Liran" and "Vova". I've added a mapping in the balance display to ensure that if the event store contains "You" or "Partner", they are displayed as "Liran" and "Vova" respectively for backward compatibility.
EXPERT APP DESIGNER: I've injected custom CSS to force the `primary` button type to a green color scheme (#28a745). This satisfies the visual request while maintaining Streamlit's structural integrity.
EXPERT PRODUCT MANAGER: Per-user budget limits are now implemented in `BUDGET_TARGETS`. A warning logic is in place that triggers at 85% utilization, showing a warning in the sidebar, and an error if the limit is exceeded.
SENIOR PRINCIPAL DEV PROGRAMMER: Optimized the button interaction logic to only trigger `st.rerun()` if the selection actually changes, which should improve the perceived speed during category switching.
ORCHESTRATOR: All changes applied to `app.py`. Handoff to user.

SENIOR PRINCIPAL DEV PROGRAMMER: Deployment issue identified. Local changes were not committed or pushed to the `deploy` remote (`expenses_app.git`).
ORCHESTRATOR: CONSULT: `Senior Principal Dev Programmer` to finalize deployment.
SENIOR PRINCIPAL DEV PROGRAMMER: Committed `app.py` and `limits.json` and pushed to `deploy main`.
ORCHESTRATOR: The live app at Streamlit Cloud should now be rebuilding with the latest layout and features.

EXPERT PRODUCT MANAGER: The user requested that only the logged-in user see their own limits. 
SENIOR PRINCIPAL DEV PROGRAMMER: Implemented a new "Your Budget Utilization" section in the dashboard that dynamically filters limits and spending based on the `active_user`.
EXPERT APP DESIGNER: Added progress bars and color-coded statuses (Blue/Yellow/Red) to provide immediate visual feedback on spending levels.
ORCHESTRATOR: Pushed to `deploy main`. Live app update in progress.

SENIOR PRINCIPAL DEV PROGRAMMER: Bug identified in budget utilization. The logic was looking for "Liran" in the splits, but the historical data (and current events based on the user's view) uses "You".
EXPERT AMBIGUITY ANALYST: Confirmed that "You" and "Partner" are the keys stored in the event store.
SENIOR PRINCIPAL DEV PROGRAMMER: Implemented a key-mapping shim in the budget calculation. It now checks both the display name ("Liran") and the internal key ("You") to aggregate spending correctly. 
ORCHESTRATOR: Pushed the fix. Utilization bars should now reflect existing data.
