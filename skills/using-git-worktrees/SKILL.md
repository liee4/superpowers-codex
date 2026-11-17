---
name: using-git-worktrees
description: Use when the user requests Git worktree isolation or when the current checkout contains work that must be isolated from the requested changes.
---

# Using Git Worktrees

1. Inspect the current checkout, branch, and pending changes with read-only commands. Reuse a suitable existing worktree or checkout when possible.
2. If isolation is needed and authorized, use the host's native worktree tool so the app tracks it. In a Git-only environment, use `git worktree add` with a verified destination and appropriate branch or commit. Follow repository rules for where worktrees live.
3. Check the resulting checkout and run the setup needed for the task. Protect existing edits and preserve pre-existing failures when reporting verification results.
4. If isolation is unavailable, continue only where the requested changes can be made independently. Report any actual blocker. Use the owning host's cleanup tool for worktrees it created when appropriate.
