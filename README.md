# Matt Pocock Skills v1.1.0 – HQC Core

A curated and adapted skill pack for working with AI coding agents such as Codex, Claude Code, and compatible agent environments.

This repository is maintained by **Nguyễn Đăng Quang / HQC**. It translates the central engineering lessons of Matt Pocock's public `skills` repository into a smaller operating core for real project work: clarify before coding, investigate before fixing, control scope, verify actual behavior, and hand off with evidence.

> This is an independent HQC adaptation. It is not an official Matt Pocock distribution and is not affiliated with Matt Pocock, Total TypeScript, or AI Hero.

## Why this repository exists

AI coding agents can write code quickly, but speed without control creates familiar failures:

- the agent solves the wrong problem;
- it modifies more files than necessary;
- it treats a successful build as proof that the feature works;
- it guesses at root causes;
- it reports completion without usable evidence;
- it consumes excessive tokens because the project lacks a shared operating method.

HQC Core introduces a small, composable workflow:

```text
Clarify → Survey → Plan → Implement → Verify → Review → Handoff
```

## Included skills

| Skill | Purpose |
|---|---|
| `grill-first` | Resolve material ambiguity before a large implementation begins. |
| `plan-before-code` | Survey the repository and define a bounded implementation plan. |
| `diagnose-before-fix` | Reproduce, isolate, and prove root cause before changing code. |
| `scope-control` | Prevent unrelated edits, opportunistic refactors, and scope drift. |
| `verify-before-done` | Require runtime evidence instead of relying only on build success. |
| `handoff` | Produce a compact, auditable completion report for the next person or agent. |

## Recommended Codex setup

Copy these files into a target repository:

```text
AGENTS.md
.agent-skills/
  grill-first/SKILL.md
  plan-before-code/SKILL.md
  diagnose-before-fix/SKILL.md
  scope-control/SKILL.md
  verify-before-done/SKILL.md
  handoff/SKILL.md
```

Start from [`templates/AGENTS.template.md`](templates/AGENTS.template.md), then add project-specific constraints, commands, and source-of-truth documents.

## Operating rule

The skills do not replace engineering judgment. They create deliberate friction at the points where coding agents most often fail.

The agent should not ask questions that the repository already answers. It should inspect first, ask only about unresolved product decisions, and make the smallest safe change that can be verified.

## About the maintainer

**Nguyễn Đăng Quang** is an information-technology graduate, management-system auditor, and consultant with more than ten years of experience in ISO auditing and organizational improvement. His work includes ISO/IEC 27001, information security, business continuity, IT service management, AI management systems, and practical digital transformation for SMEs.

He is not positioning himself as a full-time software developer. His focus is the governance and operating layer between business owners and AI coding agents: defining requirements, controlling implementation scope, validating evidence, managing risk, and turning AI-assisted development into a repeatable process.

Through HQC, he is developing practical methods for using AI agents in real business systems while preserving human oversight, auditability, security, and management control.

More: [ABOUT.md](ABOUT.md)

## Upstream inspiration and attribution

This repository is inspired by Matt Pocock's open-source repository **Skills for Real Engineers**, especially its emphasis on alignment, small feedback loops, diagnosis, testing, architecture, and reusable agent skills.

Upstream project: `mattpocock/skills`

See [NOTICE.md](NOTICE.md) for attribution details.

## Version

Current HQC Core release: **v1.1.0-hqc.1**

## License

MIT. See [LICENSE](LICENSE).
