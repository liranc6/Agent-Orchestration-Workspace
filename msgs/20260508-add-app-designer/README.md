# Internal Thread: Add App Designer

- Purpose: Coordination for adding/verifying the App Designer role.

## Thread

ORCHESTRATOR: Task initiated to check for "app designer" role and add if missing.
ORCHESTRATOR: CONSULT: `Expert Ambiguity Analyst` and `Expert Product Manager` for intake.

EXPERT AMBIGUITY ANALYST: The user asks for an "app designer". We have `Expert UX/Product Designer`. Is there a distinction for the user?
EXPERT PRODUCT MANAGER: Often "App Designer" is used synonymously with UX/UI Designer. However, to ensure full alignment with the user's mental model, we can either alias the existing role or refine it to explicitly include "App Design".
EXPERT AMBIGUITY ANALYST: User's phrasing "do you have a teem member for app designe?" suggests they might be looking for a specific label.
EXPERT PRODUCT MANAGER: Recommendation: We have `Expert UX/Product Designer` which covers the functional area. We should clarify to the user that this role exists, OR create a dedicated `Expert App Designer` if the user wants a more holistic "Application Architect/Designer" hybrid.
PLANNER: Let's create `Expert App Designer` as a specialized role for mobile/web layout and interaction specific to "apps" to complement the broader UX/Product role, or simply clarify if they are meant to be one and the same.
ORCHESTRATOR: Given the instruction "if not, add", we will add a dedicated `Expert App Designer` to satisfy the explicit request, focusing on technical app layout and design systems.

MEMBER CREATOR: Creating `dev_team/expert-app-designer.md` and updating the roles registry.
ORCHESTRATOR: Done. The `Expert App Designer` is now part of the team.
SUPERVISOR: Verified. The role is correctly integrated into `roles-matrix.md` and `CONSULTANCY_MAP.md`. Ready for handoff.
