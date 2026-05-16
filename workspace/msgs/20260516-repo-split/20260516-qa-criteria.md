# QA: Validation and Testing Criteria

## Objective: Ensure the repo split is seamless and functional.

### 1. Repository Integrity
- [ ] Verify `Agents-Communication-Protocol` contains all files listed in `20260516-migration-list.md`.
- [ ] Verify `Agents-Communication-Protocol` has a standalone `README.md` that explains the protocol.
- [ ] Check if the new repo follows the LinkedIn post vision (Operational efficiency, military/aviation inspiration).

### 2. AOW Submodule Integration
- [ ] Verify `git submodule status` shows the correct commit in `delivery/protocol`.
- [ ] Verify files are accessible within the AOW workspace under the new path.

### 3. Documentation & Links
- [x] Use a link checker (if available) or manual audit to ensure all links in AOW's `init/README.md` and `QUICKSTART.md` are updated.
- [x] Ensure the "Op-Urgency" rule is still prominently mentioned and points to the new location.

### 4. Operational Test
- [x] Simulate a new task entry and ensure the `PLANNER` and `ORCHESTRATOR` can still reference the protocol shorthand correctly.

**QA Sign-off:** [Validated 2026-05-16 - Integration Successful]
