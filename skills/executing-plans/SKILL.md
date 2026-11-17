---
name: executing-plans
description: Use when the user asks to execute an existing implementation plan or resume a partially completed plan.
---

# Executing Plans

1. Read the plan, current changes, repository instructions, and relevant code. Use the current checkout or attached worktree by default. Select isolation according to the user's request and the needs of the task.
2. Execute tasks in dependency order through the feature's normal entry points. Track progress in the plan or conversation as useful. The main agent implements and integrates the work unless the user or repository instructions request delegation.
3. Reuse existing tests when they cover the affected behavior. Add targeted regression coverage where needed. Use test-first development when requested or required by the repository.
4. If the plan drifts from the code, make a scoped, reversible adjustment and keep working. Ask when a missing decision materially changes the result or an action requires authorization.
5. Run the checks that support the expected result and inspect their output. Report the outcome, significant deviations, and any pending verification. Use independent review when requested or warranted and authorized.
