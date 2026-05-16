# TASK: Split Repo and Integrate Protocol Submodule

## Status
- [ ] Phase 1: Preparation (Identify and move files)
- [ ] Phase 2: Create Submodule Repo Structure
- [ ] Phase 3: Update Orchestration Repo to use Submodule
- [ ] Phase 4: Validation and QA

## Items
1. **PLANNER:** Finalize file list for migration. [ID: 001]
2. **DEV:** Extract protocol-related files to a temporary directory. [ID: 002]
3. **DEV:** Initialize submodule in orchestration repo. [ID: 003]
4. **DEV:** Update internal path references across all AOW docs. [ID: 004]
5. **QA:** Verify submodule connectivity and documentation link integrity. [ID: 005]
6. **REVIEW:** Final sign-off on repository structure. [ID: 006]

## Notes
- Ensure no loss of history if possible (though for this task, clean-copy is acceptable if history is maintained in the new repo independently).
- Submodule target: `git@github.com:liranc6/Agents-Communication-Protocol.git`
