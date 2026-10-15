---
name: launch-runbook
description: 当需要在开发者社区执行一次产品/功能/版本发布时使用。提供从 T-14 到 T+7 的标准动作清单、渠道分工、角色职责与发布后复盘模板。
license: CC-BY-4.0
---

# 发布节奏手册（Launch Runbook）

## 何时使用
- 准备发布新版本、新功能或一次社区活动。
- 希望发布过程可复制、不靠临场发挥。

## 核心原则
1. 开发者发布靠「文档 + Demo + 可上手」三件套，不靠口号。
2. 渠道分工明确：公告、社媒、社区各司其职。
3. 发布后 48h 是答疑黄金期，必须有人在。
4. **先小测再放量**：发布是大投入，先用预热帖 / 核心贡献者预览验证信息点，再全量推。
5. **经验回流**：把本次有效的渠道组合与信息口径记回本手册，下轮直接复用。

## 时间线
| 时间 | 动作 |
|---|---|
| T-14 | 定发布目标与口径；起草公告 / Release Note 初稿 |
| T-10 | 准备 Demo / 最小可运行示例；内部评审文档 |
| T-7 | 定稿 Release Note；准备社媒文案（多版本） |
| T-3 | 通知核心贡献者 / 提前预览；布置「发布日」监控 |
| T-0 | 发布：打 Tag/Release + 公告 + 社媒；社区同步 |
| T+1~2 | 黄金答疑期：蹲守 Issue / Discussion / 评论 |
| T+7 | 复盘：数据、反馈、待跟进项 |

## 渠道分工（RACI 简表）
| 渠道 | 负责 | 内容 |
|---|---|---|
| GitHub Release | 维护者 | Release Note、升级指引 |
| Discussion / 博客 | DevRel | 技术解读、使用场景 |
| 社媒（X / 领英） | DevRel | 亮点、链接、@相关方 |
| 社区群 | 社区运营 | 同步、答疑引流 |

## 发布前清单
- [ ] Release Note 含：变更点 / 升级方式 / 破坏性变更 / 致谢
- [ ] Demo 或示例可一键复现
- [ ] 监控与值班安排就位

## 复盘模板
- 目标达成情况（安装量 / Star / 讨论量 / 新问题数）
- 哪些动作有效 / 哪些浪费
- 待跟进的 issue 与文档缺口

## 相关技能（Related Skills）
- [dev-content-writing](../dev-content-writing/) — 公告、Release Note、社媒文案由内容写作技能产出；本手册提供时间线与口径，内容技能负责落地。
- [community-weekly-report](../community-weekly-report/) — 发布后 7 天的数据与反馈，进入周报的复盘与信号分级。
- [community-onboarding](../community-onboarding/) — 新功能发布要配套更新上手文档与 `good first issue`，承接新涌入的用户。

## 参考
- `dev-content-writing`
- `community-weekly-report`
