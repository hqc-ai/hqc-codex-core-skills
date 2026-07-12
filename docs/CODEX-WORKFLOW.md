# HQC Codex Workflow

## Standard flow

```text
Survey → Clarify → Bound Scope → Plan Wave → Implement → Verify → Review → Handoff
```

## Wave definition

A wave is a bounded implementation unit that can be completed and verified independently. A wave is larger than a single checkbox but smaller than an entire project phase.

A good wave:

- has one coherent outcome;
- changes a controlled set of files;
- has explicit acceptance criteria;
- produces evidence before the next wave starts;
- can be rolled back without dismantling unrelated work.

## Task versus wave

A task is a unit of work. A wave is a controlled execution batch that may contain several related tasks.

Use tasks to describe what must be done. Use waves to control when and how much Codex implements before review.

## Recommended sequence for Codex

1. Read project context.
2. Inspect current code and Git status.
3. Reproduce the issue or establish the baseline.
4. Present the smallest credible implementation plan.
5. Execute only the approved/current wave.
6. Run focused tests and runtime checks.
7. Audit the diff.
8. Stop before commit, push, merge, or deploy unless authorized.
