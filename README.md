# DevRel Skills for AI Agents

![Skills](https://img.shields.io/badge/skills-6-blue)

![Agent Skills Spec](https://img.shields.io/badge/Agent%20Skills-spec-brightgreen)

![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-blue.svg)

A collection of AI agent skills for **Developer Relations (DevRel)** practitioners — a skill library for running open-source ecosystem operations (e.g. AI / LLM projects) and brand marketing with AI as the lever.

This repo covers community onboarding, issue triage, launch operations, technical content, community metrics, and weekly reporting. Each skill can be handed to an AI agent for direct execution, or used as a standard playbook by operators. Compatible with any agent that supports the [Agent Skills spec](https://agentskills.io) (Claude Code, Codex, Cursor, Windsurf, etc.). All skills are written in English and are **self-contained** — each one works standalone when installed on its own.

> **Independence statement**: This repo is a distillation of developer-ecosystem operations practice and has **no affiliation with, or endorsement from, any specific open-source project (e.g. the vLLM semantic-router)**. Content produced with these skills can serve specific communities in real-world work, but the projects themselves are not part of this repo; when citing project information, the official repos and docs are the authoritative source.

> **This repo is also a working sample of GitHub operations in practice**: versioned Releases, Issues / Labels for tracking work, Discussions for Q&A, Projects boards for planning, CONTRIBUTING / LICENSE for collaboration norms — all of these capabilities are actually in use here, as evidence of hands-on GitHub proficiency. See the versioned history in [Releases](releases).

---

## Table of Contents

- [Who is this for?](#who-is-this-for)
- [What are Skills?](#what-are-skills)
- [How Skills work together](#how-skills-work-together)
- [Available Skills](#available-skills)
- [Installation](#installation)
- [Usage](#usage)
- [Skill Categories](#skill-categories)
- [Roadmap](#roadmap)
- [Discovery & Distribution](#discovery--distribution)
- [Contributing](#contributing)
- [License](#license)

---

## Who is this for?

- **DevRel practitioners**: responsible for growth, onboarding, and content for open-source communities, and in need of reusable, versioned methodologies and frameworks.
- **People running brand and community work for open-source projects**: the messaging, getting-started guides, launch cadence, and technical articles produced with these skills directly serve the projects you support, creating real-world impact for them.
- **Operators who use AI as an execution lever**: the skills embed frameworks and checklists — you drive AI with natural language to run them, compressing the distance from "want to do it" to "delivered output" dramatically.

---

## What are Skills?

Skills are **Markdown files** that give AI agents a specific task plus the best practices for doing it. Once added to a project, the agent recognizes the corresponding operations task and applies the right framework and checklist — you can either hand them to the agent for automatic execution, or have operators follow them manually. For operators, it is a senior DevRel's methodology frozen into reusable, installable, versioned files.

---

## How Skills work together

Skills cross-reference one another through **shared context**, so the business background does not have to be re-explained every time. The canonical shared context lives in two foundation files under `references/`:

- `references/community-principles.md` — the **basic principles** of community operations (single source of truth, a prerequisite for all skills).
- `references/voice-and-tone.md` — **voice and tone**, keeping external messaging consistent — whether you are writing social copy for your own brand or announcements for an open-source project you support.

Because the `skills` CLI installs one skill directory at a time, each SKILL.md **inlines the shared context it needs** (as a "Shared Context" section) so every skill works standalone. The `references/` files remain the canonical, extended versions for repo readers and for the "fork and customize" workflow.

```
references/                     ← canonical shared context (extended versions)
├── community-principles.md
└── voice-and-tone.md
        │
        ├── community-onboarding/      newcomer welcome (greeting + checklist + FAQ)
        ├── issue-discussion-triage/   Issue/Discussion classification, labels, standard replies
        ├── launch-runbook/            launch playbook (T-14 → T+7)
        ├── dev-content-writing/       developer technical content writing (AI-assisted)
        ├── community-weekly-report/   community weekly report & signal grading
        └── devrel-metrics/            ecosystem operations metrics & funnel
```

The **Related Skills** section inside each skill documents the full cross-reference map.

---

## Available Skills

| Skill | Description |
| --- | --- |
| [community-onboarding](skills/community-onboarding/) | Use when you need to design a newcomer welcome flow, onboarding checklist, and FAQ for an open-source community (e.g. an AI / LLM project), so new members can figure out "where am I and what should I do" within 5 minutes. |
| [issue-discussion-triage](skills/issue-discussion-triage/) | Use when you need to manage a technical community's Issues / Discussions — classification, labels, standard replies, triage norms — turning "piled-up questions" into "orderly responses". |
| [launch-runbook](skills/launch-runbook/) | Use when you need to run a launch (version / feature / campaign) for an open-source project and want a standard checklist and cadence from T-14 to T+7 that converts directly into community-facing and external launch content. |
| [dev-content-writing](skills/dev-content-writing/) | Use when you want AI-assisted technical content that developers actually read — project blogs, getting-started tutorials, release notes, social copy — both for your own brand marketing and for amplifying the open-source projects you support. |
| [community-weekly-report](skills/community-weekly-report/) | Use when you need to regularly summarize community activity, grade signals (risk / opportunity / to-do), and produce internal weekly reports or upward reports, making "I am operating seriously" visible. |
| [devrel-metrics](skills/devrel-metrics/) | Use when you need to define and track key ecosystem operations metrics, build funnels (awareness → adoption → contribution → retention), prove operations value with data, and run quarterly reviews. |

> The current set is the initial 6 core skills; more will be added as real-world needs emerge.

---

## Installation

**Option 1 · CLI install (recommended)**

```bash
npx skills add zzoeyliu/ai-gtm
```

To install specific skills only:

```bash
npx skills add zzoeyliu/ai-gtm --skill community-onboarding issue-discussion-triage
```

**Option 2 · Clone and copy**

```bash
git clone https://github.com/zzoeyliu/ai-gtm.git
cp -r ai-gtm/skills/* .agents/skills/
```

**Option 3 · Git submodule**

```bash
git submodule add https://github.com/zzoeyliu/ai-gtm.git .agents/skills/ai-gtm
```

**Option 4 · Fork and customize**
Fork this repo → adapt `references/` and each skill to the specific community context you support → clone locally and use.

---

## Usage

After installation, describe your needs in natural language and the agent will match the right skill. For example:

- *"Build me a newcomer welcome flow for this open-source project, in a version newcomers can understand at a glance"* → invokes `community-onboarding`
- *"20 more issues piled up in the community again; give me a triage rule set and standard replies"* → invokes `issue-discussion-triage`
- *"We are shipping a new version next week; give me the launch checklist plus an external announcement"* → invokes `launch-runbook` + `dev-content-writing`
- *"Use AI to write a social post introducing this project — professional but not stiff"* → invokes `dev-content-writing`

You can also invoke the skills directly with slash commands: `/community-onboarding`, `/issue-discussion-triage`, `/launch-runbook`, `/dev-content-writing`, `/community-weekly-report`, `/devrel-metrics`.

---

## Skill Categories

- **Onboarding**: `community-onboarding` — welcome flow, onboarding checklist, newcomer FAQ
- **Issue response**: `issue-discussion-triage` — classification, labels, standard replies
- **Launch operations**: `launch-runbook` — launch cadence and checklists
- **Content production (AI lever)**: `dev-content-writing` — developer technical writing and brand amplification
- **Measurement & review**: `devrel-metrics` — metrics, funnels, quarterly reviews
- **Reporting & sync**: `community-weekly-report` — weekly reports and signal grading

---

## Roadmap

The current set is the initial 6 core skills. More will be added based on real-world feedback. The following directions are **planned** (not yet shipped — proposals via Issues are welcome):

- `community-advocacy` — KOL / advocate programs and incentives.
- `event-runbook` — operations playbook for online / offline events (meetups, hackathons).
- `docs-audit` — documentation usability review and improvement checklist.
- `onboarding-metrics` — newcomer conversion funnel and retention tracking.

---

## Discovery & Distribution

- **Install works out of the box**: `npx skills add zzoeyliu/ai-gtm` clones directly from GitHub — no publishing step needed. This repo follows the [Agent Skills spec](https://agentskills.io/specification), so any spec-compatible agent can discover and load the skills.
- **skills.sh listing**: the [skills.sh](https://skills.sh) registry (the "npm for agent skills", by Vercel Labs) indexes skills via install telemetry from the `skills` CLI. The first `npx skills add zzoeyliu/ai-gtm` registers the repo; installs then drive its ranking.
- **agentskill.sh listing**: an independent directory with a web submission flow — paste the repo URL at [agentskill.sh/submit](https://agentskill.sh/submit) to list and get a security score.
- **Discovery hygiene**: skill `name` / `description` frontmatter is the entire discovery surface for agents, so descriptions are written to be keyword-rich and trigger-accurate (see [CONTRIBUTING.md](CONTRIBUTING.md) for the writing guidelines).

---

## Contributing

Improving existing skills, adding new ones, or fixing terminology via Issues or Pull Requests is welcome. Collaboration norms are detailed in [CONTRIBUTING.md](CONTRIBUTING.md).

---

## License

The content of this repo is licensed under [CC BY 4.0](LICENSE) — please credit the source when using it.
