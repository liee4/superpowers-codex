---
name: subagent-driven-development
description: Use when the user or repository instructions request delegated implementation and the plan has substantial tasks with clear ownership.
---

# Subagent-Driven Development

1. Read the plan and identify work that can be delegated without overlapping changes. The main agent retains responsibility for shared design, integration, and final verification.
2. Assign each delegate a bounded objective, files or interfaces, relevant project guidance, tests, and reporting expectations. Use the current checkout or an existing isolated workspace when suitable. Create a worktree when needed and authorized.
3. Give each delegate substantial work. Review returned diffs and evidence. Follow up with the same delegate when it needs to revise its work.
4. Use an independent reviewer when requested or when the risk justifies it and delegation is authorized. Group related changes so the reviewer can assess the resulting behavior across files.
5. Reconcile changes, run the integrated verification, and report the outcome. Apply repository requirements for tests, commits, and branch integration.
