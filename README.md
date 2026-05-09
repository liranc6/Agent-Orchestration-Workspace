# Agent Orchestration Workspace (AOW)
> **Recruit a disciplined AI delivery team into your repo** — phased planning, explicit protocols, and file-based traceability.

## 🚀 TL;DR: "The Virtual Team in a Box"
Most AI tools sell **agents or autonomy**. AOW sells **control**. Instead of fighting with opaque chat histories, AOW provides a repeatable **Engineering Operating System** that transforms high-level intent into auditable engineering artifacts.

---

## 🧭 Navigation for Quick Skimming

| For Executives (The "Why") | For Developers (The "How") | For Agents (The "Engine") |
| :--- | :--- | :--- |
| [Value Proposition](#-value-proposition) | [Quick Installation](#-installation) | [Mandatory Onboarding](init/README.md) |
| [Workflow Lifecycle](#-how-it-works) | [Start Here](#-start-here) | [Op-Urgency Protocol](communication_protocol/README.md) |

---

## 💎 Value Proposition
- **Chat-First Paradigm**: Tell the AI "Add a feature" and watch it update `tasks/`, `specs/`, and `msgs/` automatically.
- **Total Traceability**: Real-time SITREPs and audit logs in `tasks/`.
- **Zero Cleanup**: AI manages its own "hygiene" (pruning logs, archiving closed work).

---

## 🎯 Positioning: Why AOW?
AOW isn't just another agent framework; it's a **Managed Delivery Ecosystem** designed for developers who lead AI teams rather than just using AI assistants.

### How We Differentiate
| Feature | Agent Frameworks (CrewAI/AutoGen) | AI Coder Apps (Devin/Cursor) | **AOW Workspace** |
| :--- | :--- | :--- | :--- |
| **Focus** | "Build your own system" | "Let the agent drive" | **"You drive; the team executes"** |
| **Integration** | External library API | Standalone app / IDE | **Repo-Native (Git Submodule)** |
| **Traceability** | Transient logs | Opaque chat history | **File-based persistent memory** |
| **Governance** | None (Ad-hoc) | Model-driven | **Protocol-driven (Explicit Rules)** |

### The "Five Pillars" of AOW
1. **Repo-Native & Portable**: Lives inside your target project as a version-pinned Git submodule. Standardize workflows across many repos without rewriting prompts.
2. **Process > Prompts > Code**: A structured intake → planning → execution pipeline that makes outcomes consistent and repeatable.
3. **First-Class Governance**: "Mandatory Step 1" + Interaction Protocols create an explicit behavioral contract, reducing "rogue AI" drift.
4. **Auditable Traceability**: `user_requests/`, `specs/`, and `tasks/` create a durable trail. Executives and engineers can review *what* was decided and *why*.
5. **Human-Managed Team**: Designed for a human leader driving expert agents, fitting perfectly into real-org constraints like review and compliance.

### The "Sell" for Developers
- **Stop Prompt Spaghetti**: Use phases, roles, and functional artifacts instead of one-shot prayers.
- **Portable Infrastructure**: Recruit the same high-performing team into any project via `git submodule`.
- **Context-Density**: Save up to 40% on token costs using our proprietary **Op-Urgency AI Jargon**.

---

## 🛠 Installation: "Recruit Your Team" (30 Seconds)
AOW is designed as a **Git Submodule** to live inside your existing app.

```bash
# Add the team to your project
git submodule add https://github.com/liranc6/Agent-Orchestration-Workspace.git
```

*Alternatively, click **"Use this template"** on GitHub to start a new project from scratch.*

---

## ⚙️ How it Works (The Workflow)
1. **INTAKE**: You provide intent in chat. AI refines requirements in [user_requests/](Agent-Orchestration-Workspace/user_requests/).
2. **PLAN**: AI creates [tasks/](Agent-Orchestration-Workspace/tasks/) and technical [specs/](Agent-Orchestration-Workspace/specs/).
3. **BUILD**: Virtual experts (Dev, DevOps) execute implementation.
4. **VAL**: Reviewers and QA validate against acceptance criteria.

---

## 🧠 The Dual-Language Engine
- **Human Jargon**: [docs_human_readable/](docs_human_readable/README.md) — Full-prose docs for your onboarding.
- **AI Jargon**: [communication_protocol/](communication_protocol/README.md) — "Op-Urgency" compressed symbols to maximize AI memory and speed.

---

## 📍 Start Here
- [init/README.md](init/README.md) — **Step-by-step onboarding.**
- [QUICKSTART.md](QUICKSTART.md) — Fast workspace setup.
- [dev_team/INTERACTION_PROTOCOL.md](dev_team/INTERACTION_PROTOCOL.md) — How the experts work.

---

## 🤝 Join the Mission: Open Source Contribution
We are building the future of **AI-Mediated Software Engineering**, and the **Agent Orchestration Workspace (AOW)** is a 100% Open Source community project. Whether you are a programmer, an AI researcher, or a process enthusiast, we want your help.

### Why contribute to AOW?
*   **Pioneer the Paradigm**: Help us refine the patterns of how humans and AI teams collaborate.
*   **Build the "Engine"**: Contribute to the [Op-Urgency Protocol](communication_protocol/README.md) and internal workflows.
*   **Expand the Experts**: Develop and share new [Agent Roles](dev_team/README.md) for specialized tasks.

**Ready to jump in?** Check out [CONTRIBUTING.md](CONTRIBUTING.md) and help us build the "Virtual Team" that scales everyone's productivity.

---

## �🤖 Single-Agent Prefix Prompt (Copy/Paste)
```text
You are a single AI agent simulating a virtual team of experts. Follow the workspace process strictly:
- Mandatory Step 1: Read init/README.md, QUICKSTART.md, and dev_team/INTERACTION_PROTOCOL.md.
- Phase 1 (Intake): Use Expert Ambiguity Analyst and Expert Product Manager.
- Phase 2 (Planning): Use Planner and Orchestrator to create specs/ and tasks/.
- Phase 3 (Execution): Consult dev_team/CONSULTANCY_MAP.md.
- Traceability: Maintain msgs/ internal jargon and tasks/ status.

TASK: <insert task here>
```
