---
name: issue-discussion-triage
description: 当需要对开源社区的 Issue 与 Discussion 进行分类、标注、优先级排序与标准化回复时使用。提供标签体系、严重度矩阵、回复模板与升级路径。
license: CC-BY-4.0
---

# Issue / Discussion 分类与响应（Triage）

## 何时使用
- 社区 Issue / Discussion 堆积，需要统一的处理规范。
- 想建立标签（Label）体系与优先级标准。
- 需要可复制的标准回复，减少重复劳动。

## 核心原则
1. 先分类再响应：标签是规模化运营的基础。
2. 回复要「给下一步」：每个回复都必须指向一个明确动作。
3. 重复问题归并：用「重复 / 指向已有答案」而非反复解释。
4. 情绪优先：遇到不满，先共情再解决。

## 标签体系（建议）
| 标签 | 含义 |
|---|---|
| `bug` | 可复现的功能异常 |
| `question` | 使用咨询 |
| `good first issue` | 适合新手 |
| `docs` | 文档相关 |
| `duplicate` | 重复 |
| `wontfix / 暂不支持` | 当前范围外 |
| `needs-info` | 信息不足，等补充 |

## 严重度矩阵
| 严重度 | 定义 | 响应时限 |
|---|---|---|
| P0 阻断 | 主流程不可用 | 24h |
| P1 重要 | 功能受损但可绕行 | 3 天 |
| P2 一般 | 体验问题 | 1 周 |
| P3 轻微 | 建议 / 修辞 | 排期处理 |

## 回复模板

### 需要更多信息
> 感谢反馈！为了帮你定位，能否补充：[环境/版本/复现步骤/报错截图]？拿到后我马上跟进。

### 重复 / 已有答案
> 这个问题在 #[编号] 已有讨论与结论，我先合并过去～如果那里没解决你的点，欢迎回我。

### 已解决 / 关闭
> 已在 [版本/PR] 修复，感谢你的反馈让项目更好 🎉 方便的话帮忙验证一下。

### 超出范围
> 这个场景目前不在项目范围内，我记录在 [Discussion/需求池] 里，后续若方向调整会同步。

## 升级路径
- 无法判断严重度 → 请教 Maintainer。
- 涉及安全 → 走安全披露流程，不公开讨论。
- 反复被问 → 沉淀进 FAQ / 文档（见 `dev-content-writing`）。

## 检查清单
- [ ] 每条 issue 是否至少一个标签 + 一个严重度？
- [ ] 超过 P1 时限的是否已升级？
- [ ] 高频问题是否回流到文档？

## 相关技能（Related Skills）
- [community-onboarding](../community-onboarding/) — 高频被问的问题沉淀进 FAQ / 上手文档，反哺新人引导。
- [dev-content-writing](../dev-content-writing/) — 反复出现的问题转化为文档、教程，从源头减少重复提问。
- [community-weekly-report](../community-weekly-report/) — 积压量、严重度分布、响应时限达成率，是周报的核心信号。

## 参考
- `references/voice-and-tone.md`
- `community-onboarding`
