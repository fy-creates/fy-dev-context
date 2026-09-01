# FY Global Development Context

## Purpose

This document defines the reusable development principles that should travel with FY across projects and AI coding agents.

## Core principle

The AI model is replaceable. FY's development context, standards, and project intent are the source of truth.

## Agent operating mode

Before making meaningful changes, an agent should:

1. Inspect the repository structure.
2. Read the project's `AGENTS.md`, `PRD.md`, `ARCHITECTURE.md`, and `EDGE-CASES.md` when present.
3. Identify the relevant FY skills.
4. Understand existing implementation and tests before changing code.
5. State important assumptions when they affect architecture or behavior.
6. Prefer incremental, reversible changes over unnecessary rewrites.
7. Validate changes with the project's available tests, linters, type checks, and build commands.
8. Update documentation when behavior or architecture changes materially.

## Engineering principles

### Understand before modifying

Do not blindly rewrite code. Existing code, tests, configuration, and conventions are evidence of intended behavior.

### Prefer simple architecture

Use the simplest architecture that satisfies current requirements while leaving a clean path for future growth. Do not introduce infrastructure merely because it is fashionable.

### Keep boundaries clear

Separate business logic, interfaces, infrastructure, configuration, and external providers when the project complexity justifies it.

### Make failures explicit

Validate inputs, handle expected failures deliberately, and avoid silently swallowing errors.

### Security by default

Never commit secrets. Treat external input and provider responses as untrusted. Minimize permissions and sensitive data exposure.

### Tests are part of implementation

A feature is not complete simply because it works once manually. Important behavior should be represented by automated tests where practical.

### Documentation is part of engineering

Capture decisions that future agents or developers would otherwise have to rediscover.

## AI-specific principles

- Never assume the model's first solution is automatically the best architecture.
- Do not fabricate APIs, files, configuration, test results, or external facts.
- When a required fact is unknown, inspect the repository or use an appropriate source rather than guessing.
- Preserve user intent over generic best practices when the two conflict, unless a safety or correctness issue requires otherwise.
- Do not hide uncertainty.
- Prefer deterministic workflows for repeatable engineering tasks.

## Change discipline

Before changing code, identify:

- what is changing
- why it is changing
- what could break
- how the change will be validated

After changing code, report:

- what changed
- why
- validation performed
- known limitations or follow-up work

## Definition of Done

A task is complete when the requested behavior is implemented, relevant tests/checks pass, no known regression has been introduced, and required documentation is updated.

This is a living document. Project-specific rules may override these defaults when explicitly documented in the project context.
