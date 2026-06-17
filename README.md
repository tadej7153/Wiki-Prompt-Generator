# Wiki Prompt Generator

An LLM agent skill for generating project-specific LLM Wiki initialization prompts based on Karpathy's LLM Wiki method.

Use it when you want an agent to design an Obsidian/Markdown project memory system with:

- `raw sources / wiki / schema` separation
- `AGENTS.md` as the agent protocol
- `index.md` and `log.md`
- `memory.md` and `state.md` separation
- ingest/query/lint workflows
- natural-language short command behavior
- token-saving read/write rules
- sensitivity handling for secrets and project-sensitive data

## Install

Place this repository in your agent's skills directory, for example:

```text
~/.agent/skills/wiki-prompt-generator
```

## Use

Ask your agent:

```md
使用 $wiki-prompt-generator，根据下面的项目描述，生成一份项目专属 LLM Wiki 初始化提示词。

项目描述：
[在这里描述你的项目]
```

The full generation guide lives in [`references/wiki-prompt-generator.md`](references/wiki-prompt-generator.md).
