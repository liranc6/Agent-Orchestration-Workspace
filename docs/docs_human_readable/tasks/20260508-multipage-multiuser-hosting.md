# Task List: Multipage Multi-user Hosting

**Related Spec:** [specs/20260508-multipage-multiuser-hosting.md](specs/20260508-multipage-multiuser-hosting.md)

## Tasks

### T1: Refactor UI into Multipage Structure
- Create `pages/` directory.
- Move components from `app.py` into separate page files (Home, Personal, Joint, History).
- Update `app.py` to be the entry point (Sidebar/Navigation).
- **Status:** not-started
- **Expert:** `Expert UX / Product Designer` / `Senior Principal Dev Programmer`

### T2: Support User-Specific Summaries & Joint Summary
- Update `model.py` and `replay.py` to filter events by user.
- Add user selection to global state or sidebar.
- Implement classification summary per user.
- **Status:** not-started
- **Expert:** `Senior Principal Dev Programmer`

### T3: Cloud Hosting Prep (DevOps)
- Create `Dockerfile`.
- Create `.dockerignore`.
- Draft deployment guide for Google Cloud Run.
- Mention data persistence caveats for Cloud Run (GCS/Sheets).
- **Status:** not-started
- **Expert:** `Expert DevOps / Infrastructure Engineer`

### T4: Validation & QA
- Test multi-user isolation.
- Test joint summary calculation.
- **Status:** not-started
- **Expert:** `Expert QA`
