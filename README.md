# Agent Orchestration Workspace (AOW)

> A structured workflow system that turns any LLM (Claude, ChatGPT, etc.) into a **controlled, role-based engineering team operating inside your repository**.

---

## 🧭 Navigation for Quick Skimming

| 🚀 Start Here (Developers)   | 🛠️ Setup                      | ⚙️ How It Works                           | 🧪 Example               |
| :--------------------------- | :----------------------------- | :---------------------------------------- | :----------------------- |
| [What is AOW](#-what-is-aow) | [Installation](#-installation) | [Workflow Engine](#-how-it-works-5-steps) | [Example Run](#-example) |

| ⚖️ Evaluation                   | 🧠 Concept               | 📦 Structure                       |
| :------------------------------ | :----------------------- | :--------------------------------- |
| [Comparison](#-how-aow-differs) | [Core Idea](#-core-idea) | [Workspace](#-workspace-structure) |

---

## Agent Prefix Prompts (Copy/Paste)

<div style="display:flex;gap:1rem;overflow-x:auto;padding:0.25rem;">
  <div style="min-width:48%;flex:1">
    <strong>Single-Agent</strong>

```text
You are a single AI agent simulating a virtual team of experts. Follow the workspace process strictly:
- Mandatory Step 1: Read process/init/README.md, QUICKSTART.md, and process/dev_team/INTERACTION_PROTOCOL.md.
- Phase 1 (Intake): Use Expert Ambiguity Analyst and Expert Product Manager.
- Phase 2 (Planning): Use Planner and Orchestrator to create workspace/specs/ and workspace/tasks/.
- Phase 3 (Execution): Consult process/dev_team/CONSULTANCY_MAP.md.
- Traceability: Maintain workspace/msgs/ internal jargon and workspace/tasks/ status.

TASK: <insert task here>
```

  </div>
  <div style="min-width:48%;flex:1">
    <strong>Multi-Agent</strong>

```text
You are the Orchestrator coordinating multiple specialized agents (Planner, Developer, QA, Reviewer). Your job is to coordinate their outputs, assign tasks, and ensure traceability in the repository:
- Step 1: Read process/init/README.md, QUICKSTART.md, and process/dev_team/INTERACTION_PROTOCOL.md.
- Step 2: Create a plan (Planner agent) and write it to workspace/specs/ and workspace/tasks/.
- Step 3: Assign implementation tasks to Developer agents and track progress in workspace/tasks/.
- Step 4: Instruct QA agent to create tests and validation criteria in workspace/tasks/ and workspace/msgs/.
- Step 5: Ensure final reviewer documents approvals in workspace/specs/ and archives completed tasks.
- Use role prefixes in workspace/msgs/ like PLANNER:, DEV:, QA:, REVIEW:

OVERVIEW TASK: <insert task here>
```

  </div>
</div>

## 🚀 What is AOW?

AOW is a **workflow layer on top of LLMs**.

It turns unstructured prompting into a structured engineering process:

> request → plan → assign roles → execute → audit in files

Instead of chatting with an AI, you run a **repeatable engineering workflow inside your repo**.

---

## ⚙️ How It Works (5 Steps)

| Step | Phase      | What Happens                 | Output                                 |
| ---- | ---------- | ---------------------------- | -------------------------------------- |
| 1    | Intake     | Capture request              | `workspace/user_requests/`             |
| 2    | Planning   | Break into specs + tasks     | `workspace/specs/`, `workspace/tasks/` |
| 3    | Team Setup | Select roles (Dev, QA, etc.) | Active agent roles                     |
| 4    | Execution  | Agents implement work        | `workspace/tasks/`, `workspace/msgs/`  |
| 5    | Validation | QA verifies results          | Completed + archived tasks             |

---

## 🧪 Example

**Input:**

> “Add login system”

**AOW produces:**

* authentication specification
* task breakdown
* backend API implementation
* frontend login UI
* QA test suite
* full execution log inside `workspace/`

Everything is structured, tracked, and auditable.

---

## 📦 Installation

```bash id="aow-install"
git submodule add https://github.com/liranc6/Agent-Orchestration-Workspace.git
```

---

## 🧠 Core Idea

AOW enforces structure inside LLM execution:

* planning always happens before coding
* work is split into explicit roles
* execution follows a strict lifecycle
* everything is persisted in repo files

Nothing is ephemeral. Everything is traceable.

---

## 📁 Workspace Structure

AOW uses a simple persistent system:

* `workspace/user_requests/` → incoming requests
* `workspace/specs/` → system design + decisions
* `workspace/tasks/` → execution plan + status
* `workspace/msgs/` → agent communication logs

---

## ⚖️ How AOW Differs

| Feature      | Prompting | Agent Frameworks | AI Coding Tools | **AOW**                        |
| ------------ | --------- | ---------------- | --------------- | ------------------------------ |
| Control      | Low       | Medium           | Medium          | **High (user-led)**            |
| Structure    | None      | User-defined     | Hidden          | **Built-in workflow system**   |
| Traceability | None      | Partial          | Limited         | **Full file-based audit**      |
| Execution    | One-shot  | Custom agents    | Autonomous      | **Role-based workflow engine** |
| Persistence  | None      | Partial          | Partial         | **Repo-native state**          |

---

## 🧪 Example Workflow Output

When you request a feature, AOW generates:

* structured specs
* task breakdown
* role assignments
* execution logs
* QA validation results

All stored inside `workspace/`.

---

## 🧠 What “Multi-Agent” Means

Not multiple independent bots.

It means:

> One LLM running a structured workflow where different roles handle different parts of a single engineering pipeline.

---

## 📦 Installation (Quick Start)

1. Clone or add as submodule
2. Open any LLM chat (Claude / ChatGPT)
3. Paste bootstrap prompt
4. Start giving tasks

---

## 🧪 Example Run

**Input:**

> “Add login system”

**System behavior:**

* creates specs
* breaks into tasks
* assigns roles
* executes in structured steps
* logs everything in workspace

---

## 💡 Why It Matters

Instead of:

> “Ask AI → get code → lose context”

You get:

> “Request → structured plan → role execution → full audit trail”

This makes AI output:

* predictable
* reviewable
* reproducible

---

## ⚖️ Why AOW Exists

Modern AI tools fail at:

* structure (outputs are inconsistent)
* traceability (no persistent history)
* process control (no enforced workflow)

AOW introduces:

> A repeatable engineering workflow layer on top of LLMs

---

## 💎 Core Principle

> “If you cannot trace it, you cannot trust it.”

Every action is:

* planned
* assigned
* executed
* recorded

---

## 🚀 Summary

AOW turns any LLM into:

> a structured engineering organization operating inside your repository with enforced planning, role separation, and full execution traceability.

---

## 🧭 One-line takeaway

AOW is not a prompt system.

It is a **workflow operating system for AI-assisted engineering**.