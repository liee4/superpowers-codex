# Codex Tools

## Skills

Codex selects applicable skills using their descriptions. An explicit invocation loads the selected skill. In `agents/openai.yaml`, `policy.allow_implicit_invocation: false` reserves a skill for explicit use.

## Delegation

Use the tools exposed by the current session. Delegate when the user or applicable project or skill instructions call for it. Give the delegate a bounded task and relevant context, and use the existing agent for follow-up corrections. Inherit the session's model and reasoning defaults unless applicable instructions call for an override.

## Worktrees

In the desktop app, reuse a suitable attached worktree. Use the native worktree tool to create one when isolation is needed and authorized. For a host with Git only, inspect the checkout and Git state before using `git worktree add`. Perform only the integration operations the user has authorized.
