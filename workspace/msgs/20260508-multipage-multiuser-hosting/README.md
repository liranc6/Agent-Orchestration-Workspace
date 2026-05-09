# Internal Coordination: Multipage Multi-user Hosting

**Date:** 2026-05-08

## EXPERT AMBIGUITY ANALYST
- **Ambiguity:** How are "users" identified? If it's a browser-based Streamlit app on the web, do we need Authentication (Google Auth?) or just a dropdown selector?
- **Ambiguity:** "Joint summary" - how is "joint" defined? Is it "all users" or "specific pairs of users"?
- **Ambiguity:** "Phone app" - user asked if it's easier. A phone app (native/capacitor) requires a backend. A hosted web app (Streamlit) is easier for a data tool.

## EXPERT PRODUCT MANAGER
- **Decision:** We will switch the recommendation to **Streamlit Community Cloud** to fulfill the "Free Only" requirement.
- **Architectural Review:** Evaluated alternates (FastAPI + React, Google Apps Script, Glide).
    - *FastAPI/React:* Too complex to host for free 24/7 without a credit card (needs Heroku/Render which now cost money or limited free tiers).
    - *Google Apps Script:* 100% free, but UI is very "Spreadsheet-like" and development is slow.
    - *Streamlit:* Best balance of "Python-only" logic, mobile responsiveness, and 100% free hosting (Streamlit Cloud).
- **Final Decision:** Stick with Streamlit but improve Mobile UX.
- **Decision:** Data persistence will be moved to **Google Sheets** (free) instead of local CSV or GCS (which can incur costs).
- **Decision:** For multi-user, we will start with a **Dropdown Selector** for the "Active User" to keep it simple unless Auth is requested. We will support a "Shared" category or group for the joint summary.
- **Decision:** Multi-page layout will use Streamlit's native `pages/` support.

## ORCHESTRATOR
- Revised plan:
  1. Refactor `app.py` for Streamlit Community Cloud.
  2. Implement Google Sheets as the free database.
  3. Update deployment docs to reflect the free path.

## CONSULT: EXPERT DEVOPS / INFRASTRUCTURE ENGINEER
- **Security Check:** NEVER upload `.env` files to GitHub.
- **Issue:** User encountered "Invalid format: please enter valid TOML" in Streamlit Secrets.
- **Root Cause:** Streamlit Secrets requires TOML format (e.g., `KEY = "value"`), but the user likely pasted shell-style `.env` format.
- **Special Case:** The Google Service Account JSON needs to be nested or passed as a string/dict.
- **Action:** Formatted the specific TOML block for the user including Google Credentials.

## CONSULT: EXPERT UX / PRODUCT DESIGNER
- Multi-page: Home (Overview), My Wallet, Joint Wallet, Settings.
- Avoid cluttering the home page.
