# Kimi Adapter

## Purpose

Use FY Dev Context with a Kimi-powered coding agent.

## Loading contract

At the beginning of a project or task:

1. Locate the FY Dev Context repository or its copied/synchronized context.
2. Read `GLOBAL.md`.
3. Read the target project's `AGENTS.md`.
4. Read the target project's `PRD.md`, `ARCHITECTURE.md`, and `EDGE-CASES.md` when present.
5. Select only skills relevant to the task.
6. Treat repository source code and tests as implementation evidence.

## Portability rule

Do not modify the canonical FY context to satisfy Kimi-specific prompt syntax. Any Kimi-specific entry-point instructions belong in this adapter.

## Recommended invocation behavior

The agent should acknowledge context discovery internally or in its task plan, then proceed without requiring FY to repeat rules already documented.
