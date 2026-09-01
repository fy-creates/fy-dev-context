# Groq Adapter

## Purpose

Use FY Dev Context with a Groq-backed coding agent or application.

## Loading contract

The model/provider layer is not the source of project rules. Load the portable context before task execution:

1. `GLOBAL.md`
2. project `AGENTS.md`
3. project requirements and architecture documents
4. task-relevant skills
5. task-specific instructions

## Provider boundary

Keep Groq configuration, model names, API keys, retries, and provider-specific behavior outside the canonical skills. The skills describe engineering behavior, not a particular model.

## Portability rule

A project should be able to switch its model provider without rewriting its FY skills.
