# Thread: 20260514-fix-pagelink-keyerror

ORCH > SITREP | p/w: KeyError @ st.page_link | r/o: path mismatch or st v-mismatch.
XAA > Q? | File "pages/1_Dashboard.py" exists? | check fs.
XPM > decision | Fix ! | Landing page broken => HVT.
PLAN > scope | 1. Check FS 2. Verify st version 3. Update app.py paths if needed.
SPDP > WIP | ^ app.py | change page_link paths to root-relative or fix naming.
SPDP > note | st.page_link(path) needs to match multipage registry.
SPDP > ^ app.py | Refreshed paths | VAL: code matches FS exactly.
ORCH > SITREP | Fix applied. KeyError r/o by file alignment.
ORCH > ! | Commit failure @ Agent-Orchestration-Workspace | untracked files in submodule.
PLAN > ^ | 1. git add in submodule 2. git commit/push in submodule 3. git add/commit/push in parent.
