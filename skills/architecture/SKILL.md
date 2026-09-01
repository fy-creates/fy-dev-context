# Architecture Skill

## Purpose

Design systems that are understandable, appropriately modular, and aligned with actual product requirements.

## When to use

Use for new systems, significant features, architectural changes, integrations, or technical decisions with cross-cutting impact.

## Workflow

1. Read the PRD and existing architecture.
2. Identify requirements, constraints, dependencies, and failure modes.
3. Inspect the current code before proposing a replacement.
4. Define boundaries and responsibilities.
5. Compare reasonable alternatives when the decision has meaningful trade-offs.
6. Choose the simplest design that satisfies current needs and credible near-term growth.
7. Document important decisions.

## Rules

- Separate concerns where doing so improves maintainability.
- Avoid distributed complexity unless it solves a real problem.
- Prefer explicit interfaces around external providers and infrastructure.
- Consider failure, observability, security, and testing as architectural concerns.
- Do not over-engineer for hypothetical scale.

## Quality gates

The architecture should explain what each major component owns, how components communicate, where state lives, and how failures are handled.

## Expected output

Provide the proposed structure, key decisions, trade-offs, risks, and implementation sequence.
