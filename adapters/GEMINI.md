# Gemini Adapter

## Purpose

Use FY Dev Context with Gemini CLI or another Gemini-powered coding workflow.

## Loading contract

Before meaningful implementation work:

1. Read `GLOBAL.md`.
2. Read the project's `AGENTS.md` if present.
3. Read project requirements, architecture, and edge-case documents.
4. Load only relevant skills.
5. Inspect the repository before changing it.

## Portability rule

Do not put Gemini-specific commands or assumptions into canonical skills. Keep them here or in future generated project entry points.

## Expected behavior

Gemini should use FY context as reusable engineering guidance while respecting the project's own instructions and actual source code.
