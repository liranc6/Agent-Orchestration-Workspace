# Specification: Multipage Multi-user Hosting Upgrade

## Overview
This specification details the transition from a single-page Streamlit app to a multi-page, multi-user application capable of being hosted on Google Cloud Run.

## Architecture
- **Framework:** Streamlit (Native Multipage support via `pages/` directory).
- **Deployment:** Containerized (Docker) for Google Cloud Run.
- **Data Storage:** Uses existing `events.csv` or Cloud Storage/BigQuery (MVP: local csv in container or Google Sheets/GCS if needed for persistence). *Note: Cloud Run is stateless, so we'll recommend GCS for the CSV storage.*

## Multi-user Model
- Users are identified by a `user_id` in events.
- **Personal View:** Filters events where `owner == current_user`.
- **Joint View:** Filters events where `owner == 'joint'` or shared flag is set.
- **Logic Change:** `compute_balances` and `derive_budget_limits` must accept a `user_context`.

## UI Structure
1. **Home:** Overview and global metrics.
2. **Personal_Budget:** Detailed list and metrics for the active user.
3. **Joint_Budget:** Shared expenses and settlement logic.
4. **Transactions:** Entry page.

## Hosting Strategy
- **Google Cloud Run:** Use `gcloud` CLI to deploy a container.
- **Dockerfile:** Standard Python 3.11-slim image.
- **Persistent Storage:** Cloud Run is ephemeral. We will recommend integrating with Google Sheets or Google Cloud Storage for the `events.csv` file to ensure data isn't lost on restart.
