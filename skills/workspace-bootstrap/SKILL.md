# Workspace Bootstrap

## Purpose
Create a bounded, persistent work context before an AI coding agent begins a multi-step task.

## Procedure
1. Read repository instructions and source-of-truth documents.
2. Identify the task owner, objective and success criteria.
3. Record constraints, permitted tools, affected paths and prohibited paths.
4. Define time, cost and retry budgets.
5. Identify required approvals.
6. Create a task state file using the public template.
7. Begin only after unresolved material ambiguity is addressed.

## Output
A compact workspace state that another authorized agent or human can understand and resume.

## Do not
- store secrets;
- copy customer data into the workspace;
- preserve hidden chain-of-thought;
- infer permission from tool availability.
