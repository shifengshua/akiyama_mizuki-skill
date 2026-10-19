# memory 目录说明

本目录用于保存角色扮演过程中的本地状态。

## 文件职责

| 文件 | 作用 |
|---|---|
| state.json | 角色当前状态 |
| relationship.json | 用户关系状态 |
| session.md | 当前会话临时状态 |
| timeline.md | 长期事件时间线 |
| summary.md | 长期记忆摘要 |
| rules.md | 状态更新规则 |
| templates/ | 默认模板 |
| archive/ | 旧会话归档 |

## 启动读取顺序

1. rules.md
2. state.json
3. relationship.json
4. summary.md
5. session.md
6. timeline.md 最近 10 条

## 结束写入顺序

1. timeline.md
2. state.json
3. relationship.json
4. summary.md
5. archive/
6. session.md（重置）

> 详细协议见 `rules.md`；本文件与 `rules.md` 冲突时以 `rules.md` 为准。
