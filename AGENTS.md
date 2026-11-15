# Workspace Instructions

This directory coordinates independent repositories and worktrees.

- Treat each repository and worktree as independent.
- Read the target repository's local instructions before editing.
- Edit only repositories explicitly in scope.
- Preserve existing uncommitted changes.
- Worktrees may be created or updated as needed, following the layout below.
- Start new work in a fresh worktree from the repository's default branch.
- Fetch the remote default branch before starting new work, unless the task explicitly specifies another base or branch.
- For cross-repository tasks, keep changes and verification isolated per repository.
- Put local agent-managed indexes and records under `.agent-state/`; do not commit them.

## Layout

Group repositories by origin so same-named repositories never share a path.

- A github.com repository lives at `<org>/<repo>`.
- A repository on another host lives at `<host>/<org>/<repo>`.
- A repository without an org lives at `local/<repo>`.
- Lowercase `<org>` and `<host>`; keep `<repo>` as named upstream.
- A worktree is a sibling of its repository, named `<repo>--<branch-or-pr>`, for example `playrix/playrix-server-claude-plugins--pr-66`.
- Only `AGENTS.md` and `.gitignore` are tracked here. Everything else is ignored.
