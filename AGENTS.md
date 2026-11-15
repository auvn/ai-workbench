# Workspace Instructions

This directory coordinates independent repositories and worktrees.

- Treat each repository and worktree as independent.
- Read the target repository's local instructions before editing.
- Edit only repositories explicitly in scope.
- Preserve existing uncommitted changes.
- Worktrees may be created or updated as needed.
- Start new work in a fresh worktree from the repository's default branch.
- Fetch the remote default branch before starting new work, unless the task explicitly specifies another base or branch.
- For cross-repository tasks, keep changes and verification isolated per repository.
- Put local agent-managed indexes and records under `.agent-state/`; do not commit them.
