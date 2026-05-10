# Agent Orchestration Workspace (AOW)

> A structured workflow system that turns any LLM (Claude, ChatGPT, etc.) into a **controlled, role-based engineering team operating inside your repository**.

---

## 🧭 Navigation for Quick Skimming

| For Executives (The "Why")            | For Developers (The "How")         | For Operators (The "System")                 |
| :------------------------------------ | :--------------------------------- | :------------------------------------------- |
| 📊 [Value Proposition](#-what-is-aow) | 🛠️ [Installation](#-installation) | ⚙️ [Workflow Engine](#-how-it-works-5-steps) |
| 💡 [Why It Matters](#-why-aow-exists) | 🚀 [Quick Start](#-how-to-use)     | 🤖 [Agent Model](#-what-multi-agent-means)   |
| ⚖️ [Comparison](#-how-aow-differs)    | 🧪 [Example](#-example)            | 🧩 [Workspace Structure](#-core-idea)        |

---

## 🚀 What is AOW?

AOW is a **workflow layer on top of LLMs**.

It replaces unstructured prompting with a controlled engineering process:

> request → plan → assign roles → execute → audit in files

Instead of chatting with an AI, you run a **structured engineering workflow inside your repo**.

---

## 🧠 Core Idea

AOW enforces discipline inside LLM execution:

* every request is planned before coding
* work is split into roles (Dev, QA, DevOps)
* execution follows a strict lifecycle
* all outputs are written into repository files

Nothing is ephemeral. Everything is traceable.

---

## ⚙️ How It Works (5 Steps)

| Step | Phase      | What Happens             | Output                                 |
| ---- | ---------- | ------------------------ | -------------------------------------- |
| 1    | Intake     | Capture request          | `workspace/user_requests/`             |
| 2    | Planning   | Break into specs + tasks | `workspace/specs/`, `workspace/tasks/` |
| 3    | Team Setup | Select required roles    | Active agent roles                     |
| 4    | Execution  | Agents implement work    | `workspace/tasks/`, `workspace/msgs/`  |
| 5    | Validation | QA verifies results      | Completed + archived tasks             |

---

## 🧪 Example

**Input:**

> “New task: Add login system”

**AOW produces:**

* authentication specification
* task breakdown
* backend API implementation
* frontend login UI
* QA test suite
* full execution log in workspace

---

## ⚖️ How AOW Differs

| Feature         | Prompting        | Agent Frameworks (CrewAI / AutoGen) | AI Coding Tools (Cursor / Devin) | **AOW**                             |
| --------------- | ---------------- | ----------------------------------- | -------------------------------- | ----------------------------------- |
| Control         | Low              | Medium                              | Medium                           | **High (user-led workflow)**        |
| Structure       | None             | User-defined                        | Hidden                           | **Built-in workflow system**        |
| Traceability    | None             | Partial                             | Limited                          | **Full file-based audit trail**     |
| Execution Model | One-shot prompts | Custom agents                       | Autonomous coding                | **Role-based structured execution** |
| Persistence     | None             | Partial                             | Partial                          | **Repo-native state (workspace/)**  |

---

## 📦 Installation

AOW is designed as a **Git submodule** inside your project:

```bash id="aow-install"
git submodule add https://github.com/liranc6/Agent-Orchestration-Workspace.git
```

---

## 🤖 How to Use

1. Open Claude / ChatGPT
2. Paste the bootstrap prompt
3. Provide a task
4. AOW executes full workflow inside your repo

No additional infrastructure required.

---

## 🧪 Example Workflow Output

When you request a feature, AOW generates:

* structured specs
* task breakdown
* assigned roles
* execution logs
* QA validation output

All stored inside `workspace/`.

---

## 🧠 What “Multi-Agent” Means

Not multiple independent bots.

It means:

> One LLM running a structured workflow where different roles handle different parts of a single engineering pipeline.

### Traditional AI:

* single model does everything
* no structure
* no persistent state

### AOW:

* role separation (like a real engineering team)
* explicit planning phase
* structured execution pipeline
* shared file-based memory

---

## 🧩 Why AOW Exists

Modern AI tools fail at:

* structure (outputs are inconsistent)
* traceability (no durable history)
* governance (no enforced workflow)

AOW introduces:

> A repeatable engineering workflow layer on top of LLMs

---

## 🧭 Workspace Structure

AOW uses a simple, persistent file system:

* `workspace/user_requests/` → incoming requests
* `workspace/specs/` → system design
* `workspace/tasks/` → execution plan + status
* `workspace/msgs/` → agent communication logs

Everything is stored and auditable.

---

## 💡 Why It Matters

Instead of:

> “Ask AI → get code → lose context”

You get:

> “Define request → structured plan → role execution → full audit trail”

This turns AI from a chat tool into a **managed engineering system**.

---

## 💎 Core Principle

> “If you cannot trace it, you cannot trust it.”

Every action is:

* planned
* assigned
* executed
* recorded

Nothing disappears into chat history.

---

## 🚀 Summary

AOW turns any LLM into:

> a structured engineering organization operating inside your repository with enforced planning, role separation, and full execution traceability.

---

## 🧭 One-line takeaway

AOW is not a prompt system.

It is a **workflow operating system for AI-assisted engineering**.