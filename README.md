# agent_docs Framework

This repository provides a standardized, AI-readable framework for documenting software projects. By adopting this structure, you enable AI agents to quickly understand, navigate, and contribute to your repository using [**Continuous Alignment**](https://contalign.jefflunt.com/) and [**Progressive Disclosure**](https://docs.claude-mem.ai/progressive-disclosure).

## Core Philosophy
This framework is built on the principles of **Continuous Alignment**:
1. **Iterative Alignment**: Align on the approach (the "Plan") *before* implementation.
2. **Documentation-First**: Treat documentation as the contract/ground truth for development.
3. **Context Management**: Use Progressive Disclosure to avoid context bloat.
4. **Structured Work Breakdown**: Use plans as state-tracking mechanisms.

## Structure
- `01_orientation/`: High-level context & alignment goals.
- `02_patterns/`: Implementation standards & documentation-first practices.
- `03_deep_dives/`: Subsystem analysis & progressive disclosure targets.
- `04_plans/`: Actionable work & state tracking (using breakdown conventions).
- `templates/`: Boilerplates for agents to generate new documentation files.

## How to use

### As a Documentation Framework
AI agents should start at `01_orientation/README.md` to establish the alignment loop, then move to `02_patterns/` to understand conventions, reference `03_deep_dives/` for complex subsystem knowledge, and finally use `04_plans/` to track work progress.

### As a Project Bootstrap
To use this framework to initialize a new project, provide your AI agent with this prompt:

```plaintext
I want to build a new project that <project goals description, which can be a few lines of text, or mutiple paragraphs>. Please start implementation using the patterns laid out in https://github.com/jefflunt/agent_docs and then let's plan a series of features together.
```

When initialized this way, an AI agent should:
1. Create an `agent_docs/` folder that follows this structure (you do not need to directly clone this repo).
2. Populate `01_orientation/` with the specific project goals and architectural context.
3. Fill in `02_patterns/` as the foundational standards for the project evolve.
4. Begin the [Continuous Alignment](https://contalign.jefflunt.com/) loop by proposing the first epic plan in `04_plans/`.
