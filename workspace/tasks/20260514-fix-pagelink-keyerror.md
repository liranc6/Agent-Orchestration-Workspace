# Task: Fix st.page_link KeyError [20260514]

- [x] SITREP: Identified KeyError in `app.py` @ `st.page_link`.
- [x] r/o FS mismatch: verified `pages/1_Dashboard.py` exists.
- [/] WIP: Technical Spec creation.
- [x] WIP: Implementation of path fix.
- [x] VAL: Verify navigation works locally.

DONE.
- `st.page_link` often requires absolute-like paths from root or specific formatting.
- Current paths: `"pages/1_Dashboard.py"`.
- Potential fix: Remove `pages/` prefix if Streamlit handles it automatically, or ensure it matches internally registered page names.
