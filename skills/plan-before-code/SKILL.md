---
name: plan-before-code
description: Survey the repository and produce a bounded, evidence-based implementation plan before changing code.
---

# Plan Before Code

## Procedure

1. Read project instructions and source-of-truth documents.
2. Inspect Git status and relevant files.
3. Trace the current behavior through entry points, dependencies, and tests.
4. Identify the minimum change surface.
5. List assumptions and risks.
6. Divide work into independently verifiable waves.
7. Define verification for each wave.

## Plan format

- Current behavior and evidence
- Root area or component involved
- Files likely to change
- Files explicitly protected
- Wave sequence
- Verification commands and runtime checks
- Rollback point

Do not present a plan based only on filenames or user assumptions. Verify assertions in the repository first.
