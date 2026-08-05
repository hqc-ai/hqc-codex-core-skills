# Phase 1 Public Update — Agent Operations Skills

Copy all included paths into `hqc-codex-core-skills`.

## Recommended README insertion

Add these rows to the Included skills table:

```markdown
| `workspace-bootstrap` | Establish a bounded persistent task workspace. |
| `checkpoint-and-resume` | Preserve and resume evidence-backed progress. |
| `approval-gate` | Pause consequential actions for human approval. |
| `memory-curation` | Maintain reviewable operational memory. |
| `evidence-handoff` | Close tasks with observable evidence. |
```

Add `templates/AGENT_WORKSPACE.template.md` to the recommended setup.

## Suggested version

`v1.2.0-hqc.1`

## Suggested commit

```bash
git add .
git commit -m "feat: add governed agent operations skills"
git push
```
