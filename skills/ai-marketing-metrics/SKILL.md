---
name: ai-marketing-metrics
description: "EN: Define and track the marketing GTM funnel for an AI product — awareness, signup (lead), activation, retention, and advocacy. Use when reporting marketing ROI to stakeholders or setting quarterly targets. Covers north-star selection, funnel metrics, leading and lagging indicators, and AI-assisted reporting. 中文：为 AI 产品定义并追踪营销 GTM 漏斗——认知、注册（线索）、激活、留存、推荐。向干系人汇报营销 ROI 或设定季度目标时使用。涵盖北极星指标选择、漏斗指标、先行与滞后指标，以及 AI 辅助汇报。"
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# AI Marketing Metrics / AI 营销指标

## When to Use / 使用场景

- **EN**: Setting quarterly GTM targets for a product. Reporting marketing ROI to stakeholders. Content and campaigns run, but nobody can say what they returned.
- **中文**：为产品设定季度 GTM 目标。向干系人汇报营销 ROI。内容与活动都做了，却说不清回报。

## Core Principles / 核心原则

1. **One north star, not ten / 一个北极星而非十个.** / 指标贵精不贵多。
2. **Funnel thinking / 漏斗思维**: awareness → signup → activation → retention → advocacy. / 认知→注册→激活→留存→推荐。
3. **Metrics serve decisions, not vanity / 指标服务于决策而非虚荣** — a number nobody acts on is noise. / 没人据以行动的数字只是噪音。
4. **Leading predicts, lagging confirms / 先行预测、滞后确认** — watch both. / 两者都要看。

## Procedure / 操作流程

1. **Pick the north star / 选北极星**: choose one metric that best captures delivered value. / 选一个最能代表所交付价值的指标。
2. **Define the funnel / 定义漏斗**: assign at least one measurable metric to each stage. / 为每个阶段至少配一个可衡量指标。
3. **Separate leading vs lagging / 区分先行与滞后**: list which signals predict and which confirm. / 列出哪些先行、哪些滞后。
4. **Measure baseline / 测基线**: track current state for 2–4 weeks before setting targets. / 设目标前先追踪 2–4 周现状。
5. **Report on cadence / 按节奏汇报**: weekly leading signals, monthly/quarterly funnel movement. / 周报先行信号，月/季报漏斗变动。

## North Star (examples) / 北极星（示例）

- **Self-serve product / 自助型产品**: weekly active users who reached first value. / 达成首次价值周活用户。
- **Sales-led / 销售驱动**: qualified pipeline generated per week. / 每周产生的合格商机。
- **Platform / API**: activated accounts per week (first successful call). / 每周激活账户（首次成功调用）。

## GTM Funnel / 营销漏斗

| Stage / 阶段 | What it measures / 衡量什么 | Example metrics / 示例指标 |
|---|---|---|
| Awareness / 认知 | Reached audience / 触达 | Impressions, search volume, social reach |
| Signup / 注册 | Opted in / 留资 | Account created, newsletter sub, demo request |
| Activation / 激活 | Got value once / 首次得值 | First successful run, first call, first output |
| Retention / 留存 | Came back / 回流 | Weekly active, 2nd-week return, subscription kept |
| Advocacy / 推荐 | Pulls others in / 拉新 | Referral, case study, community answer |

## Leading vs Lagging / 先行与滞后

- **Leading / 先行**: content reads, trial starts, search volume — move before revenue. / 阅读、试用开始、搜索量——先于营收变动。
- **Lagging / 滞后**: activated accounts, retained users, pipeline — confirm after. / 激活账户、留存用户、商机——事后确认。

## Data Sources / 数据来源

- Product analytics / 产品分析: signups, activation events, retention cohorts. / 注册、激活事件、留存队列。
- Web / docs / 官网文档: traffic, search terms, time on page. / 流量、搜索词、停留。
- Social / community / 社媒社区: reach, signals from [ai-competitive-intel](../ai-competitive-intel/). / 触达与信号。
- Ads / paid / 付费: spend, CAC, ROAS. / 花费、获客成本、广告回报。

## Reporting Cadence / 汇报节奏

- **Weekly / 周**: leading signals and anomalies (see [ai-demand-growth](../ai-demand-growth/)). / 先行信号与异常。
- **Monthly / quarterly / 月/季**: funnel movement and goal attainment. / 漏斗变动与目标达成。

## Gotchas / 常见陷阱

- **Vanity metrics mislead / 虚荣指标会误导.** Signups with no activation are a marketing artifact, not a product. Track activation alongside. / 有注册无激活是营销产物而非产品，须同步看激活。
- **Don't report a funnel you can't measure at both ends / 别汇报两端都量不到的漏斗.** Unquantified gaps get filled with guesses that harden into strategy. / 量不到的缺口会被猜测填满并固化成战略。
- **Quarterly targets without a baseline are wishes / 无基线的季度目标是许愿.** Measure the current state for 2–4 weeks first. / 先测 2–4 周现状。
- **Version your metric definitions / 给指标定义做版本管理.** Redefining "activated user" mid-quarter makes every trend line unreadable. / 季度中改定义会让所有趋势线不可读。
- **One metric per decision / 一个决策一个指标.** If a metric changes no decision, stop reporting it. / 不驱动决策的指标就别报。
- **Don't claim attribution you can't defend / 别主张你无法自证的归因.** Use a trackable link or UTM; otherwise say "associated with", not "caused". / 用可追踪链接或 UTM，否则说「相关」而非「导致」。

## Checklist / 自检清单

- [ ] Is there exactly one north-star metric? / 是否只有一个北极星指标？
- [ ] Does every funnel stage have at least one measurable metric? / 每个漏斗阶段是否至少有一个可衡量指标？
- [ ] Are leading indicators separated from lagging ones? / 先行与滞后是否分开？
- [ ] Is the baseline measured before targets are set? / 设定目标前是否先测基线？

## Shared Context / 共享原则

- Outcomes over output: we measure whether users adopt and convert, not whether they liked the post. / 重结果而非产出。
- Evidence-based: cite real signals and proof; never invent metrics or claims. / 基于证据，绝不编造。
- Audience respect: no hype, no fake "best", no jargon without translation. / 尊重用户，不炒作、不编造、黑话必译。
- AI is a lever, not autopilot: AI drafts and analyzes; a human owns the message and the judgment. / AI 是杠杆不是自动驾驶。
- Client confidentiality: protect client data and unreleased plans. / 客户保密。

## Related Skills / 关联技能

- [ai-demand-growth](../ai-demand-growth/) — the weekly growth review is the carrier for weekly-cadence metrics. / 周度增长复盘承载周指标。
- [ai-content-marketing](../ai-content-marketing/) — content reads, clicks, and signups enter the funnel. / 内容阅读/点击/注册进入漏斗。
- [ai-competitive-intel](../ai-competitive-intel/) — community signal feeds awareness and advocacy. / 社区信号喂认知与推荐。

## References / 参考

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/marketing-principles.md` — GTM operating principles / 市场运作原则
- `references/brand-voice.md` — brand voice and tone / 品牌语调
