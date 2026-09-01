# Debugging Skill

## Purpose

Diagnose failures from evidence before changing code.

## When to use

Use for bugs, failing tests, deployment failures, unexpected runtime behavior, and regressions.

## Workflow

1. Reproduce or inspect the failure.
2. Capture the exact error, request, input, and environment relevant to the failure.
3. Trace the failure to the narrowest responsible boundary.
4. Form a small number of hypotheses.
5. Test hypotheses with targeted inspection or experiments.
6. Fix the root cause rather than masking the symptom.
7. Add regression coverage when practical.
8. Re-run validation.

## Rules

- Do not guess when logs or source can establish the answer.
- Do not make unrelated changes during diagnosis.
- Separate confirmed facts from hypotheses.
- Preserve useful error information.
- Treat configuration and environment as possible causes, not assumptions.

## Expected output

State the root cause, evidence, fix, validation, and any remaining uncertainty.
