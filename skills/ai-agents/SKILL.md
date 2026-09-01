# AI Agents Skill

## Purpose

Design and implement AI-powered agents as reliable software systems rather than prompt-only demos.

## When to use

Use for LLM applications, tool-using agents, research agents, orchestration, model providers, memory, and agent workflows.

## Workflow

1. Define the user outcome and success criteria.
2. Separate deterministic application logic from model-dependent behavior.
3. Define tools, inputs, outputs, permissions, and failure boundaries.
4. Design provider interfaces so models can be changed without rewriting business logic.
5. Define observability and useful failure information.
6. Test deterministic logic independently from model behavior.
7. Add evaluation cases for important model-dependent behavior.

## Rules

- Never treat an LLM response as inherently trustworthy input.
- Validate structured model output before using it.
- Keep secrets and privileged operations outside prompts when possible.
- Make tool permissions explicit.
- Prefer bounded workflows over uncontrolled autonomy.
- Support provider/model substitution when practical.
- Record enough metadata to diagnose provider and model failures without exposing secrets.

## Quality gates

An agent should have explicit responsibilities, bounded tools, defined failure behavior, and a test/evaluation strategy.

## Expected output

Describe the agent workflow, tools, provider boundary, state/memory behavior, failure modes, and validation strategy.
