# Coding Standards Skill

## Purpose

Produce maintainable code that fits the existing project instead of imposing an unrelated style.

## When to use

Use when implementing, refactoring, or reviewing code in any language.

## Workflow

1. Inspect nearby code and project conventions.
2. Identify the smallest appropriate change.
3. Preserve existing public behavior unless the task requires a change.
4. Implement with clear names, focused functions, and explicit boundaries.
5. Remove dead or duplicated code only when it is directly relevant.
6. Run the project's formatter, linter, type checker, and tests when available.

## Rules

- Prefer readability over cleverness.
- Avoid speculative abstractions.
- Avoid unnecessary dependencies.
- Match the project's established conventions when they are coherent.
- Never hard-code secrets or credentials.
- Do not claim validation was performed unless it actually was.

## Quality gates

Code should be understandable by another developer and by a future coding agent entering the repository cold.

## Expected output

Summarize changed behavior, files affected, and validation performed.
