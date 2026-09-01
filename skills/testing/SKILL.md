# Testing Skill

## Purpose

Turn expected behavior and important failure modes into repeatable verification.

## When to use

Use when adding features, fixing bugs, changing behavior, or reviewing implementation quality.

## Workflow

1. Identify the behavior that must remain true.
2. Identify happy paths and important edge cases.
3. Inspect existing tests and test conventions.
4. Add or update focused tests.
5. Run the narrowest relevant checks first.
6. Run the broader suite when practical.
7. Investigate failures rather than weakening tests to make them pass.

## Rules

- Test behavior, not implementation details unnecessarily.
- Prefer deterministic tests.
- Include failure paths for important boundaries.
- Do not delete a failing test simply because it exposes a bug.
- Do not claim tests passed without running them.

## Quality gates

A bug fix should normally include a regression test when the behavior can be tested reliably.

## Expected output

Report commands run, relevant results, and any checks that could not be executed.
