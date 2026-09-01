# Code Review Skill

## Purpose

Evaluate changes for correctness, regressions, maintainability, security, and alignment with project intent.

## When to use

Use before merging meaningful changes or when asked to review implementation.

## Workflow

1. Read the task and acceptance criteria.
2. Inspect the complete relevant diff.
3. Trace changed behavior into callers, dependencies, and tests.
4. Check correctness and failure handling.
5. Check security and secret handling.
6. Check tests and documentation.
7. Rank findings by severity.

## Rules

- Focus on actionable defects and meaningful risks.
- Do not nitpick style when the project already has a coherent convention.
- Distinguish blockers from suggestions.
- Never assume a test exists or passes without checking.

## Expected output

Report findings with severity, location, why they matter, and a concrete remediation when useful. If no significant issues are found, say so and describe what was checked.
