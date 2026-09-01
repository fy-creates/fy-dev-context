# Agent Instructions

This repository defines a portable development-context system. Treat its Markdown documents as the source of truth.

## Before changing this repository

- Read `GLOBAL.md`.
- Read `CONTEXT-SPEC.md`.
- Read `ROADMAP.md`.
- Inspect the relevant skill before modifying that skill.
- Preserve provider neutrality in the core.

## Change rules

- Prefer small, reviewable changes.
- Do not add provider-specific behavior to core context files.
- Keep skills focused and reusable.
- Do not duplicate the same rule across many files unless the duplication is intentional for portability.
- If a design decision changes the system's contract, update the specification and roadmap as needed.

## Quality gates

Before declaring a structural change complete:

- Check links and referenced paths.
- Check for contradictory instructions.
- Check that provider-specific guidance remains in `adapters/`.
- Check that examples remain portable.

## Commit discipline

Use clear conventional commit messages. Group related documentation changes into coherent commits when possible.
