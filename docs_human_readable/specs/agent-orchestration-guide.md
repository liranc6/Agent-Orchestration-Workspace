# Agent Orchestration Guide

This document explains how to use the repository as a developer-facing agent orchestration workspace.

## Purpose
- The repo is built to let a developer add it to their environment and direct an AI team.
- It is a workspace to intake requests, coordinate agents, manage state, and validate results.

## Key components
- `user_requests/` for request intake and user-facing requirements.
- `msgs/` for internal coordination, questions, and role alignment.
- `tasks/` for active work tracking and execution status.
- `dev_team/` for role definitions and team responsibilities.
- `specs/` for process and internal guidance.
- `archive/` for closed requests and completed tasks.

## Workflow
1. Create a request under `user_requests/`.
2. Open a message thread under `msgs/` to align the team.
3. Break the work into a task under `tasks/`.
4. Track state with `State Tracker` and `State Manager`.
5. Validate outputs with `Validator`.
6. Evaluate outcomes with `Evaluator`.
7. Archive completed work.

## How to use the repo
- Use `templates/` to create consistent request, task, msg, and evaluation documents.
- Keep the internal thread updated as work progresses.
- Capture decision rationale and intermediate artifacts in `msgs/` or `specs/`.
- Use `QUICKSTART.md` for initial setup.

## What this repo is not
- It is not an autonomous execution engine.
- It does not replace live issue or project tracking platforms.
- It is a documentation-first orchestration layer for developer-directed agents.
