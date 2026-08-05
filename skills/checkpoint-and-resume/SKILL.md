# Checkpoint and Resume

## Purpose
Preserve verifiable progress for long-running work without claiming completion prematurely.

## Checkpoint content
- completed steps;
- changed files;
- commands or tests run;
- observed results;
- unresolved risks;
- next bounded action;
- evidence references;
- remaining budget.

## Resume procedure
1. Validate that the checkpoint belongs to the current repository and task.
2. Re-read changed source-of-truth documents.
3. Verify that prior evidence is still valid.
4. Continue from the next bounded action.
5. Do not repeat completed work unless validation fails.

## Stop conditions
Stop and request human direction when scope, authority, risk or required evidence changes materially.
