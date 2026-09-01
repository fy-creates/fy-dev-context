# FY Dev Context Specification

Version: 0.1

## 1. Context layers

FY Dev Context uses four conceptual layers:

1. **Global context** — stable FY-wide engineering principles.
2. **Skill context** — reusable instructions for a specific kind of work.
3. **Project context** — the project's goals, architecture, constraints, and decisions.
4. **Task context** — the immediate request and acceptance criteria.

The narrower layer wins when it intentionally and explicitly defines project-specific behavior.

## 2. Portable format

The canonical format is plain Markdown plus predictable directories. No provider-specific syntax is required for the core context.

A skill should live at:

`skills/<skill-name>/SKILL.md`

## 3. Skill contract

Every skill should contain:

- `Purpose`
- `When to use`
- `Inputs/context to inspect`
- `Workflow`
- `Rules`
- `Quality gates`
- `Expected output`

Skills should be focused. Avoid turning one skill into a giant universal prompt.

## 4. Project contract

A project adopting FY Dev Context should expose, where relevant:

- `AGENTS.md` — how agents should operate in this repository.
- `PRD.md` — what is being built and why.
- `ARCHITECTURE.md` — how the system is structured.
- `EDGE-CASES.md` — important failure modes and unusual scenarios.

## 5. Provider neutrality

Core files must not assume Kimi, Groq, Gemini, OpenAI, or another provider. Provider adapters only explain how an agent should discover and load the canonical context.

## 6. Context loading priority

Recommended order:

1. Global rules
2. Project agent instructions
3. Project requirements and architecture
4. Relevant skills
5. Task-specific instructions
6. Existing implementation and tests as runtime evidence

## 7. Future automation

A future CLI may discover relevant skills automatically, bootstrap project documents, validate context completeness, and generate provider-specific entry points. Automation must remain a convenience layer; Markdown remains the portable source of truth.
