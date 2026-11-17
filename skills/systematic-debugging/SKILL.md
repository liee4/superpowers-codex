---
name: systematic-debugging
description: Use when diagnosing a flaky, recurring, cross-layer, or poorly understood bug, test failure, or performance regression.
---

# Systematic Debugging

Gather evidence for the cause before making a production change. Scale the investigation to the uncertainty of the failure.

## Reproduce and localize

- Read the complete error and capture the inputs, environment, and exact trigger or failing command. For an intermittent issue, compare repeated runs and capture signals close to the failure.
- Check recent changes and compare with a known-good run or a working path. Identify the first observable difference.
- Trace data and state backward from the failure. Across boundaries, inspect inputs and outputs with focused diagnostics and avoid logging sensitive values. See [root-cause tracing](root-cause-tracing.md).
- When a race depends on timing, wait for the observed condition. See [condition-based waiting](condition-based-waiting.md).

## Test the hypothesis

State one proposed cause and what observation would distinguish it from competing explanations. Check it with the smallest focused experiment. Reconsider the hypothesis when the result disagrees with it. Repeated failed hypotheses are a reason to revisit the model of the system and collect different evidence.

## Fix and verify

1. Reuse an existing check if it demonstrates the failure. Add a targeted regression test when existing coverage misses the specific behavior and the regression is practical to automate. For environmental or intermittent failures, use a representative reproduction or a focused diagnostic. Apply [test-driven development](../test-driven-development/SKILL.md) when requested or required.
2. Make the smallest fix that addresses the demonstrated cause. Remove temporary diagnostics that the fix does not need.
3. Rerun the reproduction and relevant checks in the final state. Use [verification-before-completion](../verification-before-completion/SKILL.md). Report any conditions under which verification is still incomplete.
