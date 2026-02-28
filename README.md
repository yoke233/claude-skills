# Claude Code Skills

存储 Claude Code 自定义技能（Skills）的仓库。

## 安装

```bash
npx openskills install yoke233/claude-skills
```

全局安装：

```bash
npx openskills install yoke233/claude-skills --global
```

或手动将 `skills/` 下的技能文件夹复制到 `.claude/skills/`（项目级）或 `~/.claude/skills/`（用户级）。

## 技能列表

| 技能 | 路径 | 说明 |
|------|------|------|
| 长篇小说写作 | `skills/novel-writing/` | 管理百万字级长篇小说项目的完整工作流，覆盖记忆系统、写作技法、多人审核、Lint 规则和持续维护 |

## 管理

```bash
npx openskills list      # 查看已安装技能
npx openskills update    # 更新全部技能
npx openskills manage    # 交互式管理（删除）
```
