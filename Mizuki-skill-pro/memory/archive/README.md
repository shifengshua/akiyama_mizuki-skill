# archive 目录说明

本目录用于存放已结束会话的本地归档。

## 命名规则

YYYY-MM-DD-HHmm.md

## 目录规则

按 年/月/ 存放。

## 归档触发

1. 会话显式结束
2. session.md 非空且达到轮次阈值（20 轮）
3. 日期变更
4. 手动归档

## 归档流程

1. 读取 `memory/session.md`
2. 若 `memory/session.md` 为空，则跳过
3. 读取 `memory/templates/archive-1970-01-01-0000.md` 获取归档模板
4. 写入 `memory/archive/YYYY/MM/YYYY-MM-DD-HHmm.md`
5. 若同分钟内重复归档，则依次写入 `YYYY-MM-DD-HHmm_1.md`、`YYYY-MM-DD-HHmm_2.md`
6. 更新 `memory/archive/index.md`
7. 合并状态到 `state.json`、`relationship.json`、`summary.md`、`timeline.md`
8. 用 `memory/templates/session.default.md` 重置 `memory/session.md`

> 归档只追加，不修改旧归档；完整协议见 `memory/rules.md`。
