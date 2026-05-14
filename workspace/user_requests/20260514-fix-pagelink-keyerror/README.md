# Request: Fix st.page_link KeyError

## Context
User reported a `KeyError` when using `st.page_link` in `app.py`.

## Error Traceback
```
KeyError: This app has encountered an error.
Traceback:
File "/mount/src/expenses_app/app.py", line 98, in <module>
    main()
File "/mount/src/expenses_app/app.py", line 92, in main
    st.page_link("pages/1_Dashboard.py", label="Dashboard", icon="📊")
...
File "/home/adminuser/.conda/lib/python3.10/site-packages/streamlit/elements/widgets/button.py", line 1588, in _page_link
    url_pathname = page_data["url_pathname"]
```

## Acceptance Criteria
- [ ] Investigate cause of `KeyError` (pylint/conda/streamlit version?).
- [ ] Fix `st.page_link` implementation or environment.
- [ ] Verify landing page navigation.
