---
name: community-weekly-report
description: 当需要向团队或社区定期汇总开源社区动态时使用。提供周报模板、应追踪的指标、信号分级与分发方式。
license: CC-BY-4.0
---

# 社区周报（Community Weekly Report）

## 何时使用
- 每周向团队 / 维护者同步社区状态。
- 需要把分散的社区信号收敛成可决策的信息。

## 核心原则
1. 周报是「决策输入」，不是流水账。
2. 信号分级：什么要立刻处理，什么仅记录。
3. 始终给「下周建议动作」。

## 模板
```
# 社区周报（YYYY-Www）

## 关键指标
- 新增 Star / Fork：
- 新增 Issue / 已关闭：
- 新增 Discussion / 已回复：
- 新增贡献者：

## 本周信号
- 🔴 阻塞：[需立刻处理的事]
- 🟡 关注：[值得留意]
- 🟢 良好：[正向进展]

## 重点讨论
- [Discussion 链接 + 一句话结论]

## 下周建议
- [动作 1]
- [动作 2]
```

## 指标清单
- 增长类：Star / Fork / 新贡献者。
- 健康类：Issue 关闭率、首响应时长。
- 内容类：文档访问、博客阅读。

## 信号分级
- 🔴 阻塞：安全、主流程故障、关键贡献者流失。
- 🟡 关注：重复问题增多、某模块问询集中。
- 🟢 良好：贡献增长、好评。

## 分发
- 内部：团队频道 / 周会。
- 公开：社区 Discussion 置顶（可选）。

## 相关技能（Related Skills）
- [devrel-metrics](../devrel-metrics/) — 周报中的指标与信号，是月度 / 季度漏斗复盘的数据底座。
- [issue-discussion-triage](../issue-discussion-triage/) — 周报里的阻塞 / 关注信号，直接对应 triage 的升级项。
- [launch-runbook](../launch-runbook/) — 发布后的数据回溯，是周报复盘的输入之一。

## 参考
- `devrel-metrics`
