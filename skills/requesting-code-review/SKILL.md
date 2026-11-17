---
name: requesting-code-review
description: Use when the user or repository requires independent code review, or when an authorized independent review would address a specific high-risk change.
---

# Requesting Code Review

1. Identify the exact diff, intended behavior, and relevant repository standards. Provide test evidence and the files or interfaces with the greatest review risk.
2. When delegation is authorized and available, use a reviewer separate from the implementer. Ask for actionable correctness, compatibility, security, or verification findings with file and line references. Set the review scope to the risk at hand.
3. Verify each finding against the current code and requirements. Fix in-scope issues and rerun relevant checks. Request follow-up review if the correction materially changes what the reviewer assessed.
4. If an independent reviewer is unavailable, perform the review you can and report which review actually occurred.
