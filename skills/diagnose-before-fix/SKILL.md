---
name: diagnose-before-fix
description: Diagnose bugs and regressions through reproduction, minimization, hypotheses, instrumentation, and proof before applying a fix.
---

# Diagnose Before Fix

## Loop

1. Reproduce the failure reliably.
2. Capture exact evidence: command, route, environment, log, response, or screenshot.
3. Minimize the failing path.
4. Generate a small set of falsifiable hypotheses.
5. Test the cheapest discriminating hypothesis first.
6. Identify root cause, not merely the visible symptom.
7. Apply the smallest fix.
8. Add a regression check.
9. Re-run the original reproduction and nearby critical paths.

## Stop conditions

Do not edit when the failure cannot yet be reproduced unless the task explicitly authorizes a defensive change. Mark uncertainty clearly.

Do not claim root cause merely because a change makes the symptom disappear.
