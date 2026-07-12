# Read-only Implementation Review

Audit the current implementation without modifying files.

Compare the change against:

- the stated objective;
- the allowed and protected scope;
- acceptance criteria;
- repository conventions;
- required runtime verification;
- Git and deployment restrictions.

Report:

1. exact changed files;
2. whether each change is necessary;
3. scope violations;
4. functional or security risks;
5. missing tests or runtime checks;
6. rollback concerns;
7. recommendation: keep, revise, or rollback.

Do not treat build success as proof of correct behavior.
