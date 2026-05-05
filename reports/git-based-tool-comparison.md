# Git-Based Tool Comparison

This report compares repository-centric collaboration tools against the current repo's documentation-driven, in-repo workflow.

| tool_name | diff_from_my_repo | tool_advanteges | tool_disadvanteges | gap_can_be_answered |
| --- | --- | --- | --- | --- |
| GitHub Issues + Projects | External issue tracking and kanban boards built into GitHub. Provides rich integration with pull requests, milestones, and GitHub Actions. | Native GitHub integration, easy issue linking, built-in notifications, standard for open-source projects. | Less customizable than a dedicated process book; conversations live outside the repo docs; depends on GitHub UI. | Partially — this repo can complement GitHub Issues with a self-documenting process, but cannot replace GitHub's interactive issue management. |
| GitLab Issues + Boards | GitLab provides issue tracking, boards, and CI/CD in one platform. Designed for a full git workflow inside a single product. | Integrated merge requests and pipelines, configurable boards, and built-in project planning. | Requires GitLab hosting or account; not part of the repo itself; may be overkill for lightweight documentation-driven repo governance. | Partially — the repo's internal docs can align with GitLab workflows, but GitLab's issue board is an external coordination layer. |
| Gitea / Gogs Issue Tracking | Lightweight self-hosted git service with issue tracking and simple boards. | Minimal setup, self-hosted control, good for small teams or private instances. | Limited feature set compared to GitHub/GitLab, less polished user experience, and separate from repo content. | Partially — the repo can document how to use Gitea issues, but does not itself provide the hosted UI or workflow automation. |
| ZenHub / GitHub Projects (classic) | Layered project management add-on on top of GitHub issues. Adds roadmap, reports, and story points. | Adds agile planning and burndown charts directly to GitHub issues. | Paid extension for some features; still external to repo content; increases tool complexity. | No — the repo cannot fully answer the need for visual agile planning features, but it can document how to use them in context. |

## Summary

The current repo is a self-documenting process tool rather than an external issue/project tracker. Similar git-based tools focus on interactive, UI-driven issue management, while this repo is designed to keep workflow rules and coordination inside the repository itself. The main gap is that the repo does not provide live issue tracking or kanban boards, which external tools address.
