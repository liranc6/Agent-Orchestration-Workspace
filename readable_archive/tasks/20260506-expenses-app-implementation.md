# Task: Build Expenses App

status: WIP

## Goal
Create a Streamlit-based event-sourced expenses ledger matching `app_description/`.

## Progress
- [x] Inspect specification files
- [x] Create core Python package for events and replay logic
- [x] Create Streamlit UI with expense creation, edit, delete, settlement, and balance views
- [x] Add local append-only storage and optional Google Sheets support scaffolding
- [ ] Validate app flows with tests
- [ ] Confirm app usability and update docs

## Notes
- The app derives state from sorted events and enforces expense deletion semantics.
- Local CSV storage is the default append-only ledger.
- The user-facing app is in `app.py`.
