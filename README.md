# DevRel Skills for AI Agents · 开发者生态运营技能库

![Skills](https://img.shields.io/badge/skills-6-blue)

![Agent Skills Spec](https://img.shields.io/badge/Agent%20Skills-spec-brightgreen)

![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-blue.svg)

一套面向 **开发者生态运营（Developer Relations / DevRel）** 从业者的 AI agent 技能集合，帮助运营者用 AI 这个杠杆，为开源社区（如 AI / LLM 类项目）做生态运营与品牌营销。

本库覆盖社区引导、问题分流、发布运营、技术内容、运营指标与社区周报。每个技能既能交给 AI 智能体直接执行，也能作为运营人员照着做的标准作业手册。兼容任何支持 [Agent Skills 规范](https://agentskills.io) 的智能体（Claude Code、Codex、Cursor、Windsurf 等）。

> **独立声明**：本仓库为开发者生态运营的实践沉淀，**与任何特定开源项目（如 vLLM semantic-router）无隶属或背书关系**。基于这些技能生产的内容，可在实战中服务于具体社区，但项目本身不在本仓库中；引用项目信息时以官方仓库与文档为权威源。

> **本仓库也是 GitHub 运营能力的实践样本**：Releases 版本化、Issues / Labels 管理待办、Discussions 答疑、Projects 看板排期、CONTRIBUTING / LICENSE 规范协作——这些能力都在本仓库中被实际运用，作为「精通 GitHub 场景」的佐证。版本化记录见 [Releases](releases)。

---

## 目录（Contents）

- [为谁打造](#为谁打造who-is-this-for)
- [什么是 Skills](#什么是-skillswhat-are-skills)
- [技能如何协同](#技能如何协同how-skills-work-together)
- [可用技能](#可用技能available-skills)
- [安装](#安装installation)
- [使用](#使用usage)
- [技能分类](#技能分类skill-categories)
- [路线图](#路线图roadmap)
- [贡献](#贡献contributing)
- [许可证](#许可证license)

---

## 为谁打造（Who is this for?）

- **开发者生态运营者（DevRel）**：负责开源社区的增长、引导与内容，需要可复用、可版本化的方法论与框架。
- **为开源项目做品牌与社区的人**：用这些技能生产的话术、上手指南、发布节奏、技术文章，直接服务于你支持的项目，在实战中为它创造影响力。
- **把 AI 当执行杠杆的运营者**：技能内嵌框架与清单，你用自然语言驱动 AI 把它跑出来——从"想做"到"产出"的距离被大幅压缩。

---

## 什么是 Skills（What are Skills?）

Skills 是赋予 AI agents 特定任务与最佳实践的 **Markdown 文件**。当被加入项目后，agent 能识别对应的运营任务，并应用正确的框架与清单——你既可以把它们交给 agent 自动执行，也可以由运营人员照着做。对运营者而言，它等于把一位资深 DevRel 的方法论，固化成可复用、可安装、可版本化的文件。

---

## 技能如何协同（How Skills Work Together）

技能之间通过**共享上下文**相互引用，避免每次重复解释业务背景。本库的共享上下文是 `references/` 下的两个基础文件：

- `references/community-principles.md` —— 社区运营的**基本原则**（单一事实来源，是所有技能的前提）。
- `references/voice-and-tone.md` —— **语气与品牌声音**，保证对外内容口径一致——无论你是写自己品牌的推文，还是为支持的开源项目写公告。

```
references/                     ← 共享上下文（被所有技能首先读取）
├── community-principles.md
└── voice-and-tone.md
        │
        ├── community-onboarding/      新人引导（欢迎语 + 上手清单 + FAQ）
        ├── issue-discussion-triage/   Issue/Discussion 分类、标签与标准回复
        ├── launch-runbook/            发布节奏手册（T-14 → T+7）
        ├── dev-content-writing/       开发者技术内容写作（AI 辅助产出）
        ├── community-weekly-report/   社区周报与信号分级
        └── devrel-metrics/            生态运营指标与漏斗
```

各技能内的 **Related Skills** 一节标注了完整的交叉引用关系。

---

## 可用技能（Available Skills）

| 技能                                                         | 说明                                                                            |
| ---------------------------------------------------------- | ----------------------------------------------------------------------------- |
| [community-onboarding](skills/community-onboarding/)       | 当用户需要为一个开源社区（如 AI / LLM 类项目）设计新人欢迎流程、上手清单与 FAQ，让新成员也能在 5 分钟内看懂"我在哪、该干嘛"时。     |
| [issue-discussion-triage](skills/issue-discussion-triage/) | 当用户要管理一个技术社区的 Issue / Discussion——分类、打标签、写标准回复、建立分流规范，把"问题堆积"变成"有序响应"时。       |
| [launch-runbook](skills/launch-runbook/)                   | 当用户要为开源项目执行一次发布（版本 / 功能 / 活动），需要一份从 T-14 到 T+7 的标准动作清单与节奏，且能直接转成对社区与对外的发布内容时。 |
| [dev-content-writing](skills/dev-content-writing/)         | 当用户要用 AI 辅助产出开发者真正会读的技术内容——项目博客、上手教程、版本公告、社媒文案——既为自己的品牌营销，也为所支持的开源项目做传播时。     |
| [community-weekly-report](skills/community-weekly-report/) | 当用户要定期汇总社区动态、分级信号（风险 / 机会 / 待办），产出对内周报或向上汇报，让"我在认真运营"可被看见时。                   |
| [devrel-metrics](skills/devrel-metrics/)                   | 当用户要定义与追踪生态运营关键指标、搭建漏斗（认知 → 采用 → 贡献 → 留存），用数据证明运营价值、做季度复盘时。                   |

> 当前为初始 6 个核心技能，后续按实战需要持续扩充。

---

## 安装（Installation）

**方式一 · CLI 安装（推荐）**

```bash
npx skills add zzoeyliu/ai-gtm
```

可只安装指定技能：

```bash
npx skills add zzoeyliu/ai-gtm --skill community-onboarding issue-discussion-triage
```

**方式二 · 克隆并复制**

```bash
git clone https://github.com/zzoeyliu/ai-gtm.git
cp -r ai-gtm/skills/* .agents/skills/
```

**方式三 · Git 子模块**

```bash
git submodule add https://github.com/zzoeyliu/ai-gtm.git .agents/skills/ai-gtm
```

**方式四 · Fork 后自定义**  
Fork 本仓库 → 按你支持的具体社区语境修改 `references/` 与各个技能 → 克隆到本地使用。

---

## 使用（Usage）

安装后，用自然语言描述需求，agent 会自动匹配对应技能。例如：

- *"帮我把这个开源项目的新人欢迎流程搭出来，写成新人一看就懂的版本"* → 调用 `community-onboarding`
- *"社区 Issue 又堆了 20 个，给我一套分流规则和标准回复"* → 调用 `issue-discussion-triage`
- *"下周要发一个新版本，给我发布清单，顺带产出一篇对外公告"* → 调用 `launch-runbook` + `dev-content-writing`
- *"用 AI 帮我写一条介绍这个项目的社媒文案，语气要专业但不端着"* → 调用 `dev-content-writing`

也可直接调用技能命令：`/community-onboarding`、`/issue-discussion-triage`、`/launch-runbook`、`/dev-content-writing`、`/community-weekly-report`、`/devrel-metrics`。

---

## 技能分类（Skill Categories）

- **社区引导**：`community-onboarding` —— 欢迎流程、上手清单、新人 FAQ
- **问题响应**：`issue-discussion-triage` —— 分类、标签、标准回复
- **发布运营**：`launch-runbook` —— 发布节奏与动作清单
- **内容生产（AI 杠杆）**：`dev-content-writing` —— 开发者技术写作与品牌传播
- **度量与复盘**：`devrel-metrics` —— 指标、漏斗、季度复盘
- **汇报同步**：`community-weekly-report` —— 周报与信号分级

---

## 路线图（Roadmap）

当前为初始 6 个核心技能。后续按实战反馈持续扩充，以下为「规划中」方向（尚未上线，欢迎在 Issue 提议）：

- `community-advocacy` —— KOL / 布道者计划与激励。
- `event-runbook` —— 线上 / 线下活动（Meetup、黑客松）运营手册。
- `docs-audit` —— 文档可用性体检与改进清单。
- `onboarding-metrics` —— 新人转化漏斗与留存追踪。

---

## 贡献（Contributing）

欢迎通过 Issue 或 Pull Request 改进现有技能、补充新技能或修正术语。协作规范详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

---

## 许可证（License）

本仓库内容基于 [CC BY 4.0](LICENSE) 授权——使用时请注明出处。
