---
name: test-driven-development
description: Use when the user explicitly requests test-first development, red-green-refactor, or a repository rule requires TDD for the change.
---

# Test-Driven Development (TDD)

1. **Red.** Find or write the smallest automated test that captures the required behavior through its normal entry point. Run it and confirm it fails for the expected reason. A syntax error, unrelated failure, or misconfigured test is not evidence of a behavioral regression.
2. **Green.** Make the smallest production change that satisfies the test. Rerun it and the related tests. Check that the behavior and callers' contracts hold.
3. **Refactor.** Improve clarity when useful. Keep the behavior and rerun the affected tests after refactoring.

Prefer observable results and existing test patterns. Reuse a failing test that captures the requirement. Assert one behavior clearly and use real dependencies where practical. See [writing good tests](writing-good-tests.md) for pitfalls.

When a fix is already present, test the old behavior in a safe baseline when feasible and rerun against the fix. Preserve existing work and state any evidence gap if a safe baseline is unavailable.

For ordinary implementation, reuse existing checks and add focused coverage for a specific regression or requirement that existing tests would miss.
