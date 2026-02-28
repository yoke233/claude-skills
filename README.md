# Claude Code Skills

存储 Claude Code 自定义技能（Skills）的仓库。可通过 [openskills](https://github.com/numman-ali/openskills) 一键安装到任何 AI 编辑器。

## 安装

### Claude Code

直接安装，开箱即用：

```bash
npx openskills install yoke233/claude-skills
```

全局安装（所有项目可用）：

```bash
npx openskills install yoke233/claude-skills --global
```

### Cursor / Windsurf / Aider / Codex 等

这些编辑器通过 `AGENTS.md` 加载技能，安装后需额外执行 `sync`：

```bash
npx openskills install yoke233/claude-skills
npx openskills sync
```

如果同时使用 Claude Code 和其他编辑器，用 `--universal` 避免冲突：

```bash
npx openskills install yoke233/claude-skills --universal
npx openskills sync
```

### 手动安装

直接复制 `skills/` 下的技能文件夹到对应位置：

| 场景 | 目标路径 |
|------|----------|
| Claude Code（项目级） | `.claude/skills/` |
| Claude Code（用户级） | `~/.claude/skills/` |
| 多编辑器共存 | `.agent/skills/` + 运行 `npx openskills sync` |

## 技能列表

| 技能 | 路径 | 说明 |
|------|------|------|
| 长篇小说写作 | `skills/novel-writing/` | 管理百万字级长篇小说项目的完整工作流，覆盖记忆系统、写作技法、多人审核、Lint 规则和持续维护 |

## 管理

```bash
npx openskills list              # 查看已安装技能
npx openskills update            # 更新全部技能
npx openskills remove <name>     # 删除指定技能
npx openskills manage            # 交互式管理
```
