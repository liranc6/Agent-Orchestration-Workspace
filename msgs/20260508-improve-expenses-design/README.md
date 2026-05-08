# Internal Thread: Improve Expenses App Design

- Purpose: Coordination for visual enhancements.

## Thread

ORCHESTRATOR: User wants to improve the expenses app design using the new `Expert App Designer`.
ORCHESTRATOR: CONSULT: `Expert App Designer` for initial audit of the app.
ORCHESTRATOR: CONSULT: `Senior Principal Dev Programmer` to find where the UI is defined.

SENIOR PRINCIPAL DEV PROGRAMMER: The UI is defined in `app.py` using Streamlit. It's a single-page application with a sidebar, top-level charts, and an expander for input.

EXPERT APP DESIGNER: I've audited the Streamlit implementation. It's functional but can be improved for better visual hierarchy and clarity.
- **Visual Hierarchy**: Use `st.metric` for balances to make them pop compared to a simple table.
- **Layout**: The charts are currently in columns with the balance table. We should unify the "Summary" view.
- **Color & Style**: Use consistent emojis for categories to improve scannability.
- **Interactive Feedback**: Improve the grouping of the "Create a new expense" form.
- **Responsive Navigation**: Use the sidebar effectively for global stats.

EXPERT PRODUCT MANAGER: Ensure we don't remove the "Search" and "Filter" capabilities. The "More Controls" tab is a bit hidden, maybe move "Settlement" to a more prominent place if balances are high.

ORCHESTRATOR: PLANNER, let's draft the implementation steps in `tasks/`.

MEMBER CREATOR: Creating the design spec and applying changes to `app.py`.
EXPERT APP DESIGNER: UI Refresh complete. 
- Integrated `st.metric` for live balances in the sidebar.
- Added emoji mappings for categories (Food 🍕, Transport 🚗, etc.).
- Improved layout with columns and containers.
- Switched static tables to `st.dataframe` for interactive sorting.
- Maintained all existing features (splits, search, settlement).
SUPERVISOR: Visual validation complete. The app now has a modern, dashboard-like feel while retaining all core logic.
ORCHESTRATOR: Task complete.
