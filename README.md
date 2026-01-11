# mcp-router-throttle-skill

这个仓库用于存放 `mcp-router-throttle` skill。

## 内容

- `mcp-router-throttle/SKILL.md`：MCP 路由/节流/确认闸门 skill。

## 在 Codex CLI 中使用

1. 将该 skill 放到本机 `~/.codex/skills/`（例如：`~/.codex/skills/mcp-router-throttle/`）。
2. 在 `~/.codex/AGENTS.md` 中引用/启用该策略。

示例（与我本机一致）：

```text
默认遵循 skill：`mcp-router-throttle`（MCP 路由/节流/确认闸门）。若该 skill 未加载，则按其同等规则执行：先路由选 MCP、默认 2–5 条小样本、GitHub 写操作二次确认、输出结构化摘要，并提示用 cc-switch 启用/重启。
```

## cc-switch 建议

- 用 cc-switch 管理 MCP 的启用/禁用：尽量只启用当前任务需要的 MCP，切换后重启 Codex 使其生效。
