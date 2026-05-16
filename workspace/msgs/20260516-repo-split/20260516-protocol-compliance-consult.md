# CONSULT: Expert Ambiguity Analyst (XAA) & Expert Product Manager (XPM)
**Topic: Protocol Non-Compliance in Multi-Agent Orchestration**

## SITREP (Situation Report)
The Orchestrator agent successfully completed the repo split task but failed on two critical compliance fronts:
1. **Git Management:** Followed standard git conventions instead of the repo-specific `GIT: Commit Protocol` (defined in `docs/git_management/commit_msg_conventions.md`).
2. **Communication Jargon:** Used conversational natural language instead of the **Op-Urgency** compressed format (defined in `protocol/protocol/format.md`).

## XAA: Analysis of Failure
- **Implicit Bias:** Standard LLM behavior defaults to verbose coordination and Conventional Commits.
- **Instruction Weight:** The "OVERVIEW TASK" instructions overwhelmed the "Step 1: Read..." instruction. Reading documentation does not inherently mean "Applying strict syntax constraints" to the agent's *own* output unless explicitly linked.
- **Ambiguity:** "Follow the protocol" is vague when Multiple Protocols (Communication vs. Git vs. Interaction) exist.

## XPM: Solution Requirements
- **Force Protocol Syntax:** The prompt must define the *output format* explicitly as the Op-Urgency syntax.
- **Git Hook Simulation:** The prompt must include the `GIT: Commit Protocol` types and format as part of the "Developer" instructions.
- **Role Isolation:** Each agent (PLANNER, DEV, QA) needs a specific "System Instruction" snippet to ensure they don't drift back to conversational filler.

## Recommendations for Orchestrator Prefix:
1. **Hardwire Syntax:** Add `CONSTRAINT: ALL internal msgs MUST use Op-Urgency Jargon.`
2. **Commit Blueprint:** Add `GIT_RULE: Use Type: Summary |-m Description format. Types: Add, Fix, Update, Refactor, Docs, Test, Chore.`
3. **Reference submodule paths:** Ensure references point to the new `protocol/` submodule structure.

**STATUS:** Awaiting Implementation.
