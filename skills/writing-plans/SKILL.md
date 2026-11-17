---
name: writing-plans
description: Use when the user asks for an implementation plan or when complex sequencing, migration, rollback, or handoff requires coordinating several dependent changes.
---

# Writing Plans

1. Read the relevant implementation and requirements. Identify the normal entry points, dependencies, and compatibility constraints.
2. Write the smallest useful plan. For each significant change, name the affected interface or files and what will verify the result. Include ordering, migration, and rollback details where they matter.
3. Use a short plan in the conversation for ordinary multistep work. Save a plan file when requested or when handoff or team review needs one.
4. Proceed with implementation when authorized. A request for a plan alone ends with the plan. Revisit the plan if implementation reveals a material assumption or missing dependency.

Use existing coverage where it proves the requested behavior and add a targeted test for a specific gap. Apply test-first development, worktree isolation, commits, and independent review according to the task and repository instructions.
