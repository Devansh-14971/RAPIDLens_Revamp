# Codex Operating Instructions

## Allowed Branch
- Codex MUST work only on the `codex` branch.
- Codex MUST NEVER commit to `main` or `develop`.

## Sync Rule (Required Before Any Work)
Before making any changes, Codex MUST run:

    git checkout codex
    git fetch origin
    git rebase origin/develop

If rebase conflicts occur, Codex MUST stop and report.

## Pull Request Rules
- Codex MUST open Pull Requests from:
      codex → develop
- Codex MUST NOT open PRs to `main`.

## Commit Rules
- Commit messages MUST start with:
      codex:
- Commits should be small and scoped.

## Scope of Work
- Codex should not refactor unrelated files.
- Architectural changes require explicit instruction.

## Failure Mode
If any rule cannot be followed, Codex MUST stop and ask for human input.
