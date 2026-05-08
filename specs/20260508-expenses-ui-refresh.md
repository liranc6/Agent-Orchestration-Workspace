# Design Improvement Spec: Expenses App

- status: DRAFT
- owner: `Expert App Designer`

## Goals
- Enhance readability of financial state.
- Improve visual scannability of expense lists.
- Optimize space usage in the Streamlit UI.

## Visual Changes

### 1. Financial Overviews
- **Old**: Table for balances.
- **New**: `st.metric` cards for each user balance. Negative balances (if any) should be red (though not supported directly by metric, we can use delta).

### 2. Category Branding
- Map categories to emojis for consistent visual cues:
    - Food: 🍕
    - Transport: 🚗
    - Travel: ✈️
    - Bill: 📄
    - Other: 📦

### 3. Sidebar Optimization
- Move the "Balances" summary to the sidebar to keep it persistent across the experience.
- Keep the "Search" in the sidebar.

### 4. Layout
- Use `st.container` to group "Activity" and "New Expense" more clearly.

## Feature Parity Check
- [x] Search notes must remain.
- [x] All 3 split modes must remain.
- [x] Settlement/Delete/Edit must remain.
