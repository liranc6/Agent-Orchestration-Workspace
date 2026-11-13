# Spec: 20260516-protocol-sync-audit

- **Topic:** Audit and Synchronize AOW with updated Protocol Submodule.
- **Date:** 2026-05-16
- **Status:** DRAFT

## 1. Objective
Ensure all Op-Urgency codes and communication formats in the Agent-Orchestration-Workspace (AOW) remain compliant with the latest updates in the `protocol/` submodule.

## 2. Background
The user recently updated the protocol submodule with "LLM-optimized" clarity and potentially modified "Expert Codes" or "Action Logic". AOW references these in `process/` and `docs/`.

## 3. Analysis
- **Expert Codes:** Protocol now uses `ORCH`, `PLAN`, `SPDP`, `JDP`, `XPM`, `XAD`, `XAA`, `XDM`, `XQA`.
- **AOW Codes:** Currently uses mixed names like `Senior Principal Dev Programmer` and shorthand `SPDP`.
- **Action Logic:** New symbols like `->`, `=>`, `^` need to be reflected in onboarding docs if missing.

## 4. Proposed Changes
1. **Update `process/dev_team/INTERACTION_PROTOCOL.md`** to strictly use the new shorthand codes for experts.
2. **Update `process/init/README.md`** and `QUICKSTART.md` if they contain outdated examples.
3. **Audit `msgs/` and `tasks/` templates** to ensure they prompt the correct syntax.

## 5. Success Criteria
- [ ] No mismatch between `protocol/protocol/format.md` and AOW documentation.
- [ ] Internal comms in `msgs/` use the latest shorthand.
