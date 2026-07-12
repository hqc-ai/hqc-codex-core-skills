---
name: scope-control
description: Keep implementation within approved boundaries and prevent unrelated refactors, configuration changes, and file churn.
---

# Scope Control

## Before editing

Define:

- objective;
- allowed behavior changes;
- allowed files or directories;
- protected behavior and files;
- maximum acceptable change surface.

## During implementation

- Prefer existing patterns.
- Avoid opportunistic cleanup.
- Do not rename, move, or reformat unrelated code.
- Do not change shared infrastructure to solve a local problem without proof.
- Review `git diff --stat` and `git diff` after each wave.

## Scope expansion

When a necessary fix crosses the approved boundary:

1. stop editing the new area;
2. explain why the expansion is necessary;
3. identify additional files and risks;
4. propose a separate wave.
