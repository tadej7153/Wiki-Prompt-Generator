# Wiki Prompt Generator

一个用于生成“项目专属 LLM Wiki 初始化提示词”的 LLM agent skill，方法论参考 Karpathy 的 LLM Wiki。

当你希望让 agent 为某个项目设计 Obsidian / Markdown 项目记忆库时，可以使用这个 skill。它会根据项目描述生成一份可交给另一个 agent 执行的初始化提示词。

生成的 Wiki 方案会包含：

- `raw sources / wiki / schema` 三层结构
- 使用 `AGENTS.md` 作为 agent 协议
- 根目录 `index.md` 和 `log.md`
- `memory.md` 与 `state.md` 的长期记忆/当前状态分离
- ingest / query / lint 工作流
- 自然语言短命令触发规则
- 节省 token 的读取和写回规则
- secrets 与项目敏感资料的分级处理

## 安装

把这个仓库放到你的 agent skills 目录中，例如：

```text
~/.agent/skills/wiki-prompt-generator
```

## 使用

对你的 agent 说：

```md
使用 $wiki-prompt-generator，根据下面的项目描述，生成一份项目专属 LLM Wiki 初始化提示词。

项目描述：
[在这里描述你的项目]
```

完整生成规则见 [`references/wiki-prompt-generator.md`](references/wiki-prompt-generator.md)。
