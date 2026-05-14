# Spec: st.page_link Path Fix

## Issue
Streamlit `st.page_link` throws `KeyError: 'url_pathname'` when it cannot find the specified page in its internal page registry. This often happens if the path provided doesn't exactly match how Streamlit has indexed the multi-page app.

## Proposed Changes
1. Update `app.py` to use relative paths that Streamlit expects.
2. If `"pages/1_Dashboard.py"` fails, try `"pages/1_Dashboard.py"` (current) vs relative to root.
3. Check if `Streamlit` version in the environment is too old (though `KeyError` suggests the function exists but data is missing).

## Verification Plan
- Run Streamlit locally if possible.
- Check logs for "Page not found" warnings which precede the KeyError.
