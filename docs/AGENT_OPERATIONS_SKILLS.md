# Agent Operations Skills

This public extension adds five composable skills:

| Skill | Use |
|---|---|
| `workspace-bootstrap` | Establish identity, boundaries and success criteria |
| `checkpoint-and-resume` | Continue long-running tasks from evidence-backed state |
| `approval-gate` | Pause consequential actions for human decision |
| `memory-curation` | Turn verified lessons into governed memory |
| `evidence-handoff` | Close work with observable evidence |

Recommended flow:

```text
workspace-bootstrap
        ↓
plan-before-code
        ↓
implement
        ↓
checkpoint-and-resume
        ↓
verify-before-done
        ↓
approval-gate (when required)
        ↓
evidence-handoff
```

These skills are intentionally generic and exclude private project workflows.
