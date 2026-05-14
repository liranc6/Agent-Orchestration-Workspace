# Tech Spec: UI/UX Modernization

## 1. Multi-Page Architecture
- **Objective**: Transition from a single-file application with conditional rendering to a Streamlit native Pages structure.
- **Action**: 
    - Create a `pages/` directory.
    - Split `app.py` logic into:
        - `pages/1_Dashboard.py`
        - `pages/2_Expenses.py`
        - `pages/3_Limits.py`
        - `pages/4_Settlements.py`
- **Main Entry (`app.py`)**: 
    - Set page config.
    - Serve as a landing page or redirect to Dashboard.
    - Universal sidebar navigation.

## 2. Floating Action Button (FAB)
- **Objective**: Provide a quick way to add expenses from any page.
- **Implementation**:
    - Streamlit does not have a native FAB.
    - Use custom CSS injection (`st.markdown` with `unsafe_allow_html=True`) to position a fixed button at the bottom right.
    - Button click will toggle a session state variable `show_add_expense_modal`.
    - If `show_add_expense_modal` is True, use `st.dialog` (if available in current Streamlit version) or a conditional container at the top of the page to simulate a modal.

## 3. Pop-up (Modal) for Add Expense
- **Objective**: Streamline the expense entry process.
- **Fields**: Date, Payer, Amount, Note, Category, Splits (Equal/Custom).

## 4. Consultancy Notes (XAD)
- **XAD > ^ Color Palette**: Use cohesive theme (Money Green / Slate Grey).
- **XAD > ^ Navigation**: Sidebar should be clean. Icons for each page.
- **XAD > ^ Feedback**: Show success toast message on expense added.
