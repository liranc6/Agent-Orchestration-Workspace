# Tech Spec: Repository Delivery & Portability (Submodule Model)

**Status:** Draft
**Date:** 2026-05-08
**Author:** ORCHESTRATOR / PLANNER

## 1. Goal
Optimize `Agent-Orchestration-Workspace` to be used as a Git Submodule within any application repository, while maintaining its ability to function as a standalone template.

## 2. Usage Models
- **Model A: Git Submodule (Recommended for existing apps)**
  - User runs: `git submodule add https://github.com/liranc6/Agent-Orchestration-Workspace.git`
  - The team exists in a sub-folder but operates on the parent repo's files.
- **Model B: Standalone/Template (Recommended for new projects)**
  - User clicks "Use this template" or clones directly.

## 3. Required Modifications
1. **Root Verification:** Check if `.gitmodules` exists in `expenses-app`.
2. **Documentation Update:** Update `README.md` and `QUICKSTART.md` to explain how to "Recruit/Install" the workspace.
3. **Portability Check:** Ensure that references to "the app" are generic.

## 4. Portability Principles
- All internal links in the workspace must be relative.
- The workspace should not hardcode its own folder name (e.g., use `Agent-Orchestration-Workspace/` only when referring to itself, but use `../` to refer to the host app).
