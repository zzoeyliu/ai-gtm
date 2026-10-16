# AI-GTM — AI Marketing & GTM Skills / AI 营销与市场进入技能库

![Skills](https://img.shields.io/badge/skills-6-blue)
![Agent Skills Spec](https://img.shields.io/badge/Agent%20Skills-spec-brightgreen)
![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-blue.svg)
![Language](https://img.shields.io/badge/language-中文%20%2F%20English-blue)

A collection of AI agent skills for running **AI-product marketing and go-to-market (GTM)** — covering positioning, content, launch, competitive intelligence, demand & growth, and metrics. The library helps marketers, growth operators, agencies, and in-house teams use AI as a lever to do the full marketing stack, not just DevRel.
一套用 AI agent 执行的**AI 产品营销与市场进入（GTM）**技能库——覆盖定位、内容、发布、竞争情报、需求增长与指标。帮助市场人、增长运营、代理商与内部团队用 AI 作为杠杆，做完整的营销全栈，而不只是开发者关系（DevRel）。

Each skill can be handed to an AI agent for direct execution, or used as a standard playbook by a human. Compatible with any agent that supports the [Agent Skills spec](https://agentskills.io) (Claude Code, Codex, Cursor, Windsurf, etc.). All skills are **self-contained** — each one works standalone when installed on its own — and **bilingual (中文 / English)**.
每个 skill 既可直接交给 AI agent 执行，也可由人按手册操作。兼容任何支持 [Agent Skills spec](https://agentskills.io) 的 agent（Claude Code、Codex、Cursor、Windsurf 等）。所有 skill 均**自包含**——单独安装也能用——且为**双语（中文 / English）**。

> **What changed / 变更说明**: the library was restructured from a DevRel-only playbook into a **general AI-marketing full stack** (brand + content + launch + intel + growth + metrics), written bilingually for both English and Chinese marketing teams.
> 本库已从「仅 DevRel」手册重构为**通用 AI 营销全栈**（品牌+内容+发布+情报+增长+指标），并以中英双语撰写，面向中英文市场团队。

---

## Table of Contents / 目录

- [Who is this for? / 面向谁](#who-is-this-for-面向谁)
- [What are Skills? / 什么是 Skill](#what-are-skills-什么是-skill)
- [How Skills work together / 技能如何协作](#how-skills-work-together-技能如何协作)
- [Available Skills / 可用技能](#available-skills-可用技能)
- [Installation / 安装](#installation-安装)
- [Usage / 用法](#usage-用法)
- [Skill Categories / 技能分类](#skill-categories-技能分类)
- [Roadmap / 路线图](#roadmap-路线图)
- [Discovery & Distribution / 发现与分发](#discovery--distribution-发现与分发)
- [Contributing / 贡献](#contributing-贡献)
- [License / 许可证](#license-许可证)

---

## Who is this for? / 面向谁

- **Marketing & GTM teams at AI companies / AI 公司的市场与 GTM 团队**: who need repeatable, versioned playbooks for positioning, content, launch, and growth. / 需要可复用、可版本化的定位、内容、发布与增长手册。
- **Agencies serving AI clients / 服务 AI 客户的代理商**: who run marketing on behalf of clients and need consistent methodology across accounts. / 代客户做营销，需要跨账户一致的方法论。
- **Operators who use AI as an execution lever / 把 AI 当执行杠杆的操盘手**: the skills embed frameworks, templates, and gotchas — you drive AI with natural language to run them. / skill 内置框架、模板与陷阱，你用自然语言驱动 AI 执行。

---

## What are Skills? / 什么是 Skill

Skills are **Markdown files** that give AI agents a specific task plus the best practices for doing it. Once added to a project, the agent recognizes the corresponding GTM task and applies the right framework and checklist — you can either hand them to the agent for automatic execution, or follow them manually. For practitioners, it is a senior marketer's methodology frozen into reusable, installable, versioned files.
Skill 是给 AI agent 特定任务与最佳实践的 **Markdown 文件**。加入项目后，agent 能识别对应 GTM 任务并套用正确框架与清单——既可交给 agent 自动执行，也可由人手动遵循。对从业者而言，这是把资深市场人的方法论固化成可复用、可安装、可版本化的文件。

---

## How Skills work together / 技能如何协作

Skills cross-reference one another through **shared context**, so the GTM background does not have to be re-explained every time. The canonical shared context lives in two foundation files under `references/`:
技能通过**共享上下文**互相引用，因此 GTM 背景无需每次重述。规范版共享上下文位于 `references/` 下的两个基础文件：

- `references/marketing-principles.md` — the **operating principles** behind every GTM action. / 每个 GTM 动作背后的**运作原则**。
- `references/brand-voice.md` — **voice and tone**, keeping client-facing messaging consistent. / **语调**，保证对外信息一致。

Because the `skills` CLI installs one skill directory at a time, each SKILL.md **inlines the shared context it needs** (as a "Shared Context" section) so every skill works standalone. The `references/` files remain the canonical, extended versions for repo readers and for the "fork and customize" workflow.
由于 `skills` CLI 一次只装一个 skill 目录，每个 SKILL.md 都**内联所需共享上下文**（「Shared Context」段），因此单独安装也能用。`references/` 文件仍是规范扩展版，供读库者与「fork 后定制」流程使用。

```
references/                     ← canonical shared context (extended versions) / 规范共享上下文（扩展版）
├── marketing-principles.md
└── brand-voice.md
        │
        ├── ai-positioning/          positioning, persona, messaging hierarchy / 定位、人群、信息层级
        ├── ai-content-marketing/    AI topic mine → draft → multi-channel adapt → measure / AI 选题→起草→多渠道改编→衡量
        ├── ai-launch-gtm/           GTM launches across X / LinkedIn / 小红书 / 视频号 / HN / Product Hunt
        ├── ai-competitive-intel/    listen → triage signal → intel & battlecards / 监听→信号分级→情报与打击卡
        ├── ai-demand-growth/        demand-gen mix, channel ROI, weekly growth review / 需求组合、渠道 ROI、周度增长复盘
        └── ai-marketing-metrics/    awareness → signup → activation → retention → advocacy / 认知→注册→激活→留存→推荐
```

The **Related Skills** section inside each skill documents the full cross-reference map.
每个 skill 内的「Related Skills」段记录了完整的交叉引用图。

---

## Available Skills / 可用技能

| Skill | Description / 说明 |
| --- | --- |
| [ai-positioning](skills/ai-positioning/) | Define or refine positioning, target persona, and core messaging before any GTM motion. / 在任何市场动作前定义或打磨定位、目标人群与核心信息。 |
| [ai-content-marketing](skills/ai-content-marketing/) | Run an AI-powered content engine: mine topics from signal, draft with AI, adapt across blog / docs / X / LinkedIn / 小红书 / 视频号, and measure what converts. / 跑 AI 内容引擎：从信号挖选题、AI 起草、跨渠道改编、衡量转化。 |
| [ai-launch-gtm](skills/ai-launch-gtm/) | Plan and run GTM launches across channels, with launch cadence and AI-assisted A/B. / 跨渠道规划并执行 GTM 发布，含发布节奏与 AI 辅助 A/B。 |
| [ai-competitive-intel](skills/ai-competitive-intel/) | Monitor market, social, communities, and competitors to triage signals into intelligence, content ideas, and battlecards. / 监测市场、社媒、社区与竞品，把信号转化为情报、选题与打击卡。 |
| [ai-demand-growth](skills/ai-demand-growth/) | Build a demand-generation and growth system (paid + organic + lifecycle + referral) with a weekly growth review. / 搭建需求生成与增长系统（付费+自然+生命周期+转介绍），含周度增长复盘。 |
| [ai-marketing-metrics](skills/ai-marketing-metrics/) | Define and track the marketing GTM funnel — awareness, signup, activation, retention, advocacy — for ROI reporting. / 定义并追踪营销 GTM 漏斗——认知、注册、激活、留存、推荐——用于 ROI 汇报。 |

> The current set is the initial 6 core skills for the AI-marketing full stack; more will be added as real-world work surfaces new needs.
> 当前为 AI 营销全栈的 6 个核心技能；随着实战涌现新需求，会持续补充。

---

## Installation / 安装

**Option 1 · CLI install (recommended) / 命令行安装（推荐）**

```bash
npx skills add zzoeyliu/ai-gtm
```

To install specific skills only / 仅安装指定技能：

```bash
npx skills add zzoeyliu/ai-gtm --skill ai-positioning ai-content-marketing
```

**Option 2 · Clone and copy / 克隆后复制**

```bash
git clone https://github.com/zzoeyliu/ai-gtm.git
cp -r ai-gtm/skills/* .agents/skills/
```

**Option 3 · Git submodule / Git 子模块**

```bash
git submodule add https://github.com/zzoeyliu/ai-gtm.git .agents/skills/ai-gtm
```

**Option 4 · Fork and customize / Fork 后定制**
Fork this repo → adapt `references/` and each skill to the specific AI product you serve → clone locally and use.
Fork 本库 → 按你所服务的 AI 产品调整 `references/` 与各 skill → 本地克隆使用。

---

## Usage / 用法

After installation, describe your needs in natural language and the agent will match the right skill. For example / 安装后用自然语言描述需求，agent 会匹配对应 skill。例如：

- *"Our AI product can't explain what it does — help me write a positioning statement and a persona"* → invokes `ai-positioning`
  「我们的 AI 产品讲不清自己是什么——帮写一份定位陈述和用户画像」→ 触发 `ai-positioning`
- *"We keep writing posts nobody signs up from — build us a content engine that starts from real user questions"* → invokes `ai-content-marketing`
  「我们总写没人注册的帖子——搭一个从真实用户问题出发的内容引擎」→ 触发 `ai-content-marketing`
- *"We're shipping v2 next month; give me a launch cadence and a channel plan"* → invokes `ai-launch-gtm`
  「下月发 v2；给我一个发布节奏和渠道计划」→ 触发 `ai-launch-gtm`
- *"What is the market saying about us vs the competitor? Turn it into content ideas and a battlecard"* → invokes `ai-competitive-intel`
  「市场和竞品怎么评价我们？转成选题和一个打击卡」→ 触发 `ai-competitive-intel`

You can also invoke the skills directly with slash commands / 也可直接用斜杠命令调用：
`/ai-positioning`, `/ai-content-marketing`, `/ai-launch-gtm`, `/ai-competitive-intel`, `/ai-demand-growth`, `/ai-marketing-metrics`.

---

## Skill Categories / 技能分类

- **Positioning / 定位**: `ai-positioning` — who it's for, the job it wins, messaging hierarchy.
- **Content (AI engine) / 内容（AI 引擎）**: `ai-content-marketing` — topic mine, draft, multi-channel adapt, measure.
- **Launch & Campaigns / 发布与活动**: `ai-launch-gtm` — launch cadence, channel mix, A/B.
- **Listening & Intelligence / 监听与情报**: `ai-competitive-intel` — signal triage, intel, battlecards.
- **Demand & Growth / 需求与增长**: `ai-demand-growth` — demand-gen mix, channel ROI, weekly review.
- **Metrics / 指标**: `ai-marketing-metrics` — GTM funnel, north-star, leading/lagging.

---

## Roadmap / 路线图

The current set is the initial 6 core skills. More will be added based on real client work. The following directions are **planned** (not yet shipped — proposals via Issues are welcome) / 当前为 6 个核心技能，后续按实战补充。以下方向**计划中**（未上线，欢迎通过 Issue 提议）：

- `ai-paid-growth` — paid channel experiments (ads, sponsored content) with AI-optimized creative. / 付费渠道实验（广告、赞助内容）与 AI 优化创意。
- `ai-event-gtm` — GTM playbook for conferences, meetups, and hackathons. / 大会、线下活动与黑客松的 GTM 打法。
- `ai-lifecycle-email` — lifecycle email / in-product nudges driving activation and retention. / 生命周期邮件/产品内触达，驱动激活与留存。
- `ai-marketing-strategy` — quarterly GTM planning and OKR-to-campaign translation. / 季度 GTM 规划与 OKR 到活动的拆解。

---

## Discovery & Distribution / 发现与分发

- **Install works out of the box / 开箱即装**: `npx skills add zzoeyliu/ai-gtm` clones directly from GitHub — no publishing step needed. This repo follows the [Agent Skills spec](https://agentskills.io/specification), so any spec-compatible agent can discover and load the skills.
  `npx skills add zzoeyliu/ai-gtm` 直接从 GitHub 克隆，无需发布步骤。本库遵循 [Agent Skills spec](https://agentskills.io/specification)，任何兼容 agent 都能发现并加载。
- **skills.sh listing / skills.sh 收录**: the [skills.sh](https://skills.sh) registry (the "npm for agent skills", by Vercel Labs) indexes skills via install telemetry from the `skills` CLI. The first `npx skills add zzoeyliu/ai-gtm` registers the repo; installs then drive its ranking.
  [skills.sh](https://skills.sh)（Vercel Labs 出品的「agent skill 的 npm」）通过 `skills` CLI 的安装遥测收录技能。首次 `npx skills add zzoeyliu/ai-gtm` 即注册本库，后续安装推动排名。
- **agentskill.sh listing / agentskill.sh 收录**: an independent directory with a web submission flow — paste the repo URL at [agentskill.sh/submit](https://agentskill.sh/submit) to list and get a security score.
  独立目录，提供网页提交入口——在 [agentskill.sh/submit](https://agentskill.sh/submit) 粘贴仓库 URL 即可收录并获安全评分。
- **Discovery hygiene / 发现卫生**: skill `name` / `description` frontmatter is the entire discovery surface for agents, so descriptions are written to be keyword-rich and trigger-accurate in both languages (see [CONTRIBUTING.md](CONTRIBUTING.md)).
  skill 的 `name`/`description` 是 agent 唯一的发现入口，因此描述在两种语言下都做到关键词丰富、触发精准（见 [CONTRIBUTING.md](CONTRIBUTING.md)）。

---

## Contributing / 贡献

Improving existing skills, adding new ones, or fixing terminology via Issues or Pull Requests is welcome. Collaboration norms are detailed in [CONTRIBUTING.md](CONTRIBUTING.md).
欢迎通过 Issue 或 PR 改进现有技能、新增技能或修正术语。协作规范详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

---

## License / 许可证

The content of this repo is licensed under [CC BY 4.0](LICENSE) — please credit the source when using it.
本库内容以 [CC BY 4.0](LICENSE) 授权——使用时请注明出处。
