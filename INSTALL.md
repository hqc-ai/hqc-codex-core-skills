# Installation

## Repository-local installation

1. Copy `templates/AGENTS.template.md` to the target repository root as `AGENTS.md`.
2. Copy selected folders from `skills/` into `.agent-skills/`.
3. Edit `AGENTS.md` with project commands, source-of-truth documents, protected files, and deployment restrictions.
4. Commit the instruction files with the project so future Codex sessions inherit the same operating rules.

Example:

```bash
cp templates/AGENTS.template.md /path/to/project/AGENTS.md
mkdir -p /path/to/project/.agent-skills
cp -R skills/* /path/to/project/.agent-skills/
```

## Suggested first use

Ask Codex to perform a read-only repository survey using `plan-before-code`, then review the proposed first wave before allowing implementation.
