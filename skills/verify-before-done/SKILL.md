---
name: verify-before-done
description: Require evidence that the changed behavior works in its real execution path before declaring completion.
---

# Verify Before Done

## Principle

Build success proves that code can be built. It does not prove that the requested behavior works.

## Verification ladder

Use the highest applicable levels:

1. Static checks: format, lint, typecheck, schema validation.
2. Focused tests: unit and regression tests for changed logic.
3. Integration checks: API, database, worker, queue, or storage path.
4. Runtime checks: browser, local preview, actual route, or real component interaction.
5. Diff audit: changed files match the authorized scope.
6. Deployment check: preview or production only when explicitly authorized.

## Evidence report

For every check, report:

- command or action;
- expected result;
- actual result;
- pass, fail, or not run;
- reason when not run.

Never write “tested successfully” without identifying what was tested.
