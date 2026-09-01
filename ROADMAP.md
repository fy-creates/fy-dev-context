# FY Dev Context Roadmap

## Vision

Create a portable development-context layer that lets FY move between AI coding agents and model providers without repeatedly explaining how projects should be understood, designed, implemented, tested, and reviewed.

## Phase 0 — Foundation

- [x] Create provider-agnostic repository
- [x] Define global development context
- [x] Define portable context specification
- [x] Define project agent contract
- [x] Create initial reusable skills
- [x] Create project-document templates
- [x] Define provider adapter pattern

## Phase 1 — Practical adoption

- [ ] Test the context with a real existing project
- [ ] Install the context into FY Intelligence
- [ ] Install it into AI Opportunity Agent
- [ ] Test with Kimi
- [ ] Test with Groq-backed coding workflow
- [ ] Test with Gemini CLI
- [ ] Test with OpenCode
- [ ] Record friction and revise the specification

## Phase 2 — Bootstrap tooling

- [ ] Create `fydev init`
- [ ] Generate project context files from templates
- [ ] Add a context validator
- [ ] Add skill listing and discovery
- [ ] Add project context status command

## Phase 3 — Intelligent skill selection

- [ ] Define skill metadata
- [ ] Build deterministic skill matching
- [ ] Add optional semantic skill discovery
- [ ] Prevent irrelevant skills from bloating agent context

## Phase 4 — Provider adapters

- [ ] Standardize Kimi entry point
- [ ] Standardize Groq entry point
- [ ] Standardize Gemini entry point
- [ ] Standardize OpenCode entry point
- [ ] Add additional agents only when they prove useful

## Phase 5 — FY Intelligence integration

- [ ] Allow FY Intelligence to read the same context
- [ ] Allow it to select relevant skills
- [ ] Allow it to bootstrap project documentation
- [ ] Keep provider/model selection independent from the context layer

## Non-goals for early versions

- Building a new LLM framework
- Replacing existing coding agents
- Forcing one model provider
- Creating a complex vector database before needed
- Automatically modifying projects without an explicit task

## Success criteria

The system succeeds when FY can start a new project, give an agent access to the FY context and project documents, and receive materially more consistent work with fewer repeated explanations.
