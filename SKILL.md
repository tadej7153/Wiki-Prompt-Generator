---
name: wiki-prompt-generator
description: Generate project-specific LLM Wiki initialization prompts based on Karpathy's LLM Wiki method. Use when an LLM agent needs to design, create, adapt, or generate prompts for Obsidian or Markdown project memory systems, agent-maintained knowledge bases, AGENTS.md wiki schemas, raw/wiki/schema workflows, persistent project wikis, or token-saving wiki protocols.
---

# Wiki Prompt Generator

Use this skill to generate a project-specific initialization prompt for an agent-maintained LLM Wiki.

## Workflow

1. Read `references/wiki-prompt-generator.md` fully before generating the prompt.
2. Use the user's project description as the source of project intent.
3. If the description is too vague, ask up to 5 high-impact questions; if the user asks to proceed directly, make reasonable assumptions and label them.
4. Generate a complete prompt that another agent can use to create the project wiki structure.

## Output Requirements

The generated prompt must include:

- Karpathy-style `raw sources / wiki / schema` mapping.
- `AGENTS.md`, `index.md`, `log.md`, and `.gitignore` requirements.
- A project-specific directory structure built around the project's core object.
- `memory.md` and `state.md` or equivalent long-term memory/current-state separation.
- Ingest, query, lint, read-before-acting, and write-back workflows.
- Natural-language short command behavior.
- Token-saving rules.
- Sensitivity handling that distinguishes secrets from project-sensitive data.
- Template and example object requirements.

Keep the final answer directly usable: the user should be able to copy the generated initialization prompt into another agent without additional editing.
