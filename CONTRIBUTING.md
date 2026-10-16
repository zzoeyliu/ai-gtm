# Contributing / 贡献

Thanks for considering a contribution to the **ai-gtm** skill library — AI-powered marketing & GTM skills for AI products. This repo welcomes any skill, template, or fix that helps teams do positioning, content, launch, intelligence, growth, and metrics with AI.
感谢你考虑为 **ai-gtm** 技能库做贡献——这是面向 AI 产品的 AI 驱动营销与 GTM 技能库。我们欢迎任何能帮助团队用 AI 做定位、内容、发布、情报、增长与指标的 skill、模板或修正。

## What You Can Contribute / 可以贡献什么

- **New skills / 新技能**: create a directory under `skills/` containing a `SKILL.md` (format below). / 在 `skills/` 下建目录并放入 `SKILL.md`（格式见下）。
- **Skill enhancements / 技能增强**: add templates, checklists, or gotchas to existing skills. / 为现有 skill 增补模板、清单或陷阱。
- **Fixes / 修正**: terminology, links, wording errors. / 术语、链接、措辞错误。

## Skill File Format (SKILL.md) / Skill 文件格式（SKILL.md）

Every skill directory must contain a `SKILL.md`. Frontmatter follows the [Agent Skills spec](https://agentskills.io/specification):
每个 skill 目录必须含 `SKILL.md`，前置元数据遵循 [Agent Skills spec](https://agentskills.io/specification)：

```yaml
---
name: your-skill-name        # kebab-case, must match the directory name / 短横线命名，须与目录名一致
description: What the skill does and when to use it. Use when [triggers]. / 技能做什么、何时用，用「Use when…」句式。
license: CC-BY-4.0
metadata:                    # optional but recommended / 可选但建议
  author: your-github-id
  version: "1.0.0"
---
```

Recommended body structure / 建议的正文结构：

1. **When to Use / 使用场景** — trigger scenarios. / 触发场景。
2. **Core Principles / 核心原则** — the non-negotiables. / 不可妥协项。
3. **Procedure / 操作流程** — actions a practitioner can follow directly. / 可直接照做。
4. **Templates / 模板** — copy-paste ready copy / checklists / briefs. / 可直接复制的文案/清单/简报。
5. **Gotchas / 常见陷阱** — concrete, non-obvious mistakes to avoid (often the highest-value section). / 具体、反直觉的避坑点（常是价值最高的一段）。
6. **Checklist / 自检清单** — pre-completion self-check. / 完成前自查。
7. **Shared Context / 共享原则** — inline the shared principles / voice the skill needs. / 内联本技能所需共享原则/语调。
8. **Related Skills / 关联技能** — cross-references. / 交叉引用。
9. **References / 参考** — canonical sources. / 规范来源。

## Writing Guidelines / 写作规范

- **Bilingual (中文 / English) / 双语**: this library is written bilingually so it serves both English and Chinese marketing teams. Keep the two languages aligned in meaning; you may present English first then 中文, or interleave per item. / 本库以双语撰写，服务中英文市场团队。两种语言含义需一致；可英文在前中文在后，或逐条并列。
- **Descriptions are the discovery surface / 描述是发现入口**: write them imperatively ("Use when…"), focused on user intent, keyword-rich, and under 1024 characters. This is the only thing an agent sees when deciding whether to load your skill. / 用祈使句式（「Use when…」），聚焦用户意图，关键词丰富，且不超过 1024 字符。这是 agent 决定是否加载你 skill 时唯一看到的内容。
- **Skills must be self-contained / 技能须自包含**: users can install a single skill (`npx skills add zzoeyliu/ai-gtm --skill your-skill`), and the repo-root `references/` directory is **not** bundled with it. Inline any shared context your skill needs as a compact "Shared Context" section, and point to the canonical `references/` files for repo readers only. / 用户可只装单个 skill（`npx skills add zzoeyliu/ai-gtm --skill your-skill`），而仓库根的 `references/` 目录**不会**随之打包。请把所需共享上下文内联为精简的「Shared Context」段，仅向读库者指向规范 `references/` 文件。
- **Concise over exhaustive / 精简胜过穷尽**: keep SKILL.md focused; split genuinely large material into per-skill `references/` files with explicit "load this when…" triggers. / 保持精炼；超大材料拆到 per-skill `references/` 文件，并写明「何时加载」。
- **GTM-first, AI as a lever / 以 GTM 为先，AI 为杠杆**: every skill should help move users down a funnel stage (awareness → signup → activation → retention → advocacy) and show where AI drafts, analyzes, or scales — while a human owns the message and the judgment. / 每个 skill 都应推动用户沿漏斗阶段前进（认知→注册→激活→留存→推荐），并标明 AI 在何处起草、分析或放大——而人掌握信息与判断。
- **Evidence over adjectives / 证据胜过形容词**: no "best-in-class", no unverified numbers, no fake users. Cite real signals and proof. / 不用「行业领先」，不写未验证数字，不造假用户。引用真实信号与证据。

## How to Submit / 如何提交

1. Fork this repo → create a branch → commit your changes. / Fork 本库 → 建分支 → 提交改动。
2. In the PR, explain: which skill was added/changed and what GTM scenario it solves. / 在 PR 中说明：新增/修改了哪个 skill，解决了什么 GTM 场景。
3. Merge after review. / 评审通过后合并。

You can also open an Issue describing your idea for the maintainer to follow up. / 也可开 Issue 描述想法，由维护者跟进。

## Distribution Notes / 分发说明

- **Install / 安装**: `npx skills add zzoeyliu/ai-gtm [--skill <name>]` works immediately from GitHub — no publishing step needed. / 从 GitHub 直接可用，无需发布步骤。
- **skills.sh listing / skills.sh 收录**: triggered by install telemetry from the `skills` CLI; a repo-root `skills.sh.json` can control grouping once listed. / 由 `skills` CLI 安装遥测触发；收录后可用仓库根 `skills.sh.json` 控制分组。
- **agentskill.sh listing / agentskill.sh 收录**: submit the repo URL at https://agentskill.sh/submit (web form). / 在 https://agentskill.sh/submit 提交仓库 URL（网页表单）。

## Code of Conduct / 行为准则

Be fact-based, respect the audience, and cite information sources. Never speak in a client's official voice without authorization, and never invent metrics or testimonials.
基于事实、尊重用户、标注信息来源。未经授权不冒充客户官方口吻，绝不编造数据或证言。
