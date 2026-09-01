# FY Dev Context

A portable, provider-agnostic development context system for FY's AI-assisted software workflow.

## Purpose

FY Dev Context separates reusable development knowledge from any particular AI model or coding agent. It gives agents a consistent understanding of:

- how FY approaches software development
- project goals and constraints
- engineering and quality standards
- reusable workflows and skills
- project documentation conventions

The system is designed to work with different agents and model providers, including Kimi, Groq-backed agents, Gemini CLI, OpenCode, and eventually FY Intelligence.

## Core principle

> The model is replaceable. The development context is not.

## Repository layers

- `GLOBAL.md` — global FY development philosophy and agent behavior.
- `skills/` — reusable task-specific development skills.
- `templates/` — standardized project documents.
- `adapters/` — instructions for making the context consumable by different agent environments.
- `project/` — future project bootstrap/runtime metadata when automation is introduced.

## Status

Version: `0.1.0` — foundation and portable documentation layer.

The first release intentionally avoids coupling the core system to a specific model provider, SDK, CLI, or agent framework.

## Roadmap

1. Establish FY's development philosophy.
2. Define a portable skill format.
3. Create reusable project-document templates.
4. Add agent adapters.
5. Add a lightweight project bootstrap CLI.
6. Add context discovery and skill selection.
7. Add validation and quality checks.
8. Integrate with FY Intelligence as an optional orchestrator.
