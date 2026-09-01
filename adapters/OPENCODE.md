# OpenCode Adapter

## Purpose

Use FY Dev Context with OpenCode or another agent that supports repository-level instructions and reusable skills.

## Loading contract

1. Load `GLOBAL.md` as the general FY context.
2. Load the project's `AGENTS.md`.
3. Read `PRD.md`, `ARCHITECTURE.md`, and `EDGE-CASES.md` when present.
4. Discover the skills relevant to the current task.
5. Inspect existing source and tests before modification.

## Portability rule

Provider- and agent-specific configuration belongs in this adapter or generated project files, not in the canonical skills.
