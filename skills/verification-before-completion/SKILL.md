---
name: verification-before-completion
description: Use before reporting that an implementation, bug fix, or other changed deliverable is complete or works.
---

# Verification Before Completion

1. Identify evidence that directly covers the requested result. Inspect the final diff and run relevant tests, validation commands, or the affected user flow as appropriate.
2. Read the output and exit status. Use evidence from the final relevant state. Rerun affected checks after changes that could invalidate them.
3. Report what was verified and its result. If a check cannot run or coverage is partial, state the exact gap. A successful build supports a build claim, and observed behavior supports a behavior claim.

Use the project's required checks and choose verification proportional to the change. Reuse a passing check in the same final state.
