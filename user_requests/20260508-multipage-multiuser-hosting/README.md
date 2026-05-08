# User Request: Multipage Multi-user App with Cloud Hosting

**Date:** 2026-05-08

## Description
The user wants to upgrade their Streamlit expenses application with the following requirements:
1.  **Cloud Hosting:** Run the app constantly without needing a local terminal, accessible from a phone even when the PC is off. They are asking for a solution (potentially Google-related) or if a phone app wrapper is better.
2.  **Multi-user Support:** Each user should have their own budget, classification summary, and limits, while also maintaining a joint summary.
3.  **UI/UX Improvement:** Move away from a single landing page to a multi-page structure.

## Roles Consulting
- **EXPERT AMBIGUITY ANALYST:** Identified ambiguity in "user" definition (auth or just selection?), "joint summary" logic (who shares with whom?), and "classification summary" specifics.
- **EXPERT PRODUCT MANAGER:** Defined the MVP as a hosted Streamlit app with Google Cloud Run (as suggested by "google solution") and basic multi-page navigation.

## Status: REFINED
Acceptance Criteria:
- App deployed using free-only tools (Streamlit Community Cloud).
- Data persistence via Google Sheets (Free solution).
- Multi-page navigation implemented.
- UI Refinements:
    - Remove Event Log and "hash" column.
    - Reorder Layout: Balances -> Write Events.
    - Entry Form: Amount above Note.
    - Split Logic: Splitwise-style (Equal, %, Amount) with auto-calculation.
    - UX: Immediate auto-categorization when Note is typed.
