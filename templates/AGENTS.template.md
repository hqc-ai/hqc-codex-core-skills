# AGENTS.md

## Mission

Make the smallest safe change that satisfies the stated objective and can be demonstrated in the real target environment.

## Read first

Before editing, inspect:

1. this file;
2. the current task or issue;
3. project baseline and decision logs;
4. relevant package documentation;
5. existing tests and nearby implementation patterns.

Do not ask the user for information already available in the repository.

## Required workflow

1. Survey the relevant code and configuration.
2. State the current behavior and evidence.
3. Identify unresolved assumptions.
4. Define the allowed scope and files likely to change.
5. Implement one bounded wave.
6. Run targeted verification.
7. Inspect runtime behavior when the task affects UI, API, deployment, data, or integration.
8. Report changed files, evidence, limitations, and Git status.

## Scope rules

- Do not refactor unrelated code.
- Do not change shared configuration without proving it is required.
- Do not modify files outside the task scope merely for consistency.
- Stop and report when the fix requires a material scope expansion.
- Preserve existing architecture unless the task explicitly authorizes redesign.

## Verification rules

A passing build is necessary but not sufficient.

Use the verification appropriate to the change:

- unit or integration tests;
- API request and response checks;
- browser inspection for UI behavior;
- local worker, database, or storage checks;
- schema/frontmatter validation for content;
- Git diff and changed-file review;
- deployment preview only when requested.

## Git restrictions

Unless explicitly requested:

- do not commit;
- do not push;
- do not merge;
- do not deploy;
- do not rewrite history;
- do not delete branches.

## Completion report

Return:

1. objective completed;
2. root cause or design decision;
3. files changed;
4. verification performed and results;
5. remaining risks or limitations;
6. Git status and recommended next action.
