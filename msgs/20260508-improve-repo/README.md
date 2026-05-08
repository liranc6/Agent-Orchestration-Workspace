# Thread: Improve Workspace for Better Results

- Purpose: Internal coordination on improving the repo to better leverage AI experts.

## Thread

ORCHESTRATOR: Task: Improve the repo results by better utilizing experts. I've initiated [user_requests/20260508-improve-repo/README.md](user_requests/20260508-improve-repo/README.md).

PLANNER: We should focus on the gap between user requests and agent execution. Often the agents don't know *which* expert to consult for specific phases. I suggest improving the `dev_team/README.md` and adding a "Consultancy Map".

PRODUCT MANAGER: Agreed. We also need to make sure the user can easily see *why* an expert was used. Let's add an `expert_contributions` section to the `tasks/` template.

SENIOR AGENT DEVELOPER: I'll review the existing expert role files. Some might be redundant or lacking specific "Interaction Protocols". I'll propose updates to `dev_team/expert-*.md`.

ORCHESTRATOR: Sounds solid. PLANNER, please draft the [specs/20260508-improve-repo-spec.md](specs/20260508-improve-repo-spec.md). SENIOR AGENT DEVELOPER, start auditing the `dev_team` folder.

QA: I'll verify that the new structure doesn't break current workflows and that the new templates are discoverable.

DONE: The improvements are live.
- Interaction Protocol: [dev_team/INTERACTION_PROTOCOL.md](dev_team/INTERACTION_PROTOCOL.md)
- Consultancy Map: [dev_team/CONSULTANCY_MAP.md](dev_team/CONSULTANCY_MAP.md)
- Standardized Experts: Updated Ambiguity Analyst, PM, UX Designer, DevOps, Planner, QA, Reviewer.
- Logic improvements in README and templates.

ORCHESTRATOR: The user asked if the "Single-agent prefix prompt" in the main README needs improvement. 

PLANNER: Absolutely. It currently mentions `user_requests`, `msgs`, etc., but it doesn't mention our new [INTERACTION_PROTOCOL.md](dev_team/INTERACTION_PROTOCOL.md) or the [CONSULTANCY_MAP.md](dev_team/CONSULTANCY_MAP.md). It should explicitly tell the agent to consult experts during specific phases.

AMBIGUITY ANALYST: It also lacks instruction on *how* to log those consultations in the `tasks/` file using the new template section. We should make it more robust.

ORCHESTRATOR: Agreed. I'll draft the update.

SENIOR AGENT DEVELOPER: I've updated `planner.md`, `expert-qa.md`, and `expert-code-reviewer.md`. The new protocol in `INTERACTION_PROTOCOL.md` is clear.

QA: DONE: All files created and updated. Templates are now more helpful for tracking expert value.

ORCHESTRATOR: FINAL REVIEW:
- **What was done:** Improved expert discoverability and utilization through a new Interaction Protocol, categorized roles, and enhanced templates.
- **Why it was done:** To ensure the user gets better results by knowing exactly when and how to engage specific AI experts.
- **Improvements:** Future iterations could automate the "Expert Consultation Log" generation.

DONE: Task 20260508-improve-repo complete.
