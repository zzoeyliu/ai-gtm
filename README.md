# AI-GTM — DevRel Marketing Skills for DevTools

![Skills](https://img.shields.io/badge/skills-6-blue)

![Agent Skills Spec](https://img.shields.io/badge/Agent%20Skills-spec-brightgreen)

![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-blue.svg)

A collection of AI agent skills for running **Developer Relations (DevRel) as AI-powered marketing / go-to-market (GTM)** for developer tools (devtools). The library helps DevRel practitioners, agencies, and in-house teams use AI as a lever to do devtool positioning, content, channel campaigns, community listening, growth metrics, and client reporting.

Each skill can be handed to an AI agent for direct execution, or used as a standard playbook by a human. Compatible with any agent that supports the [Agent Skills spec](https://agentskills.io) (Claude Code, Codex, Cursor, Windsurf, etc.). All skills are written in English and are **self-contained** — each one works standalone when installed on its own.

> **What changed**: the library was restructured from "developer-ecosystem operations" playbooks into a unified "AI marketing for DevRel" skill set, oriented to devtools GTM and client / team use.

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

- **DevRel / GTM teams at devtool companies**: who need repeatable, versioned playbooks for positioning, content, and campaigns.
- **Agencies serving devtool clients**: who run DevRel marketing on behalf of clients and need consistent methodology across accounts.
- **Operators who use AI as an execution lever**: the skills embed frameworks, templates, and gotchas — you drive AI with natural language to run them, compressing the distance from "want to do it" to "delivered output".

---

## What are Skills?

Skills are **Markdown files** that give AI agents a specific task plus the best practices for doing it. Once added to a project, the agent recognizes the corresponding GTM task and applies the right framework and checklist — you can either hand them to the agent for automatic execution, or follow them manually. For practitioners, it is a senior DevRel marketer's methodology frozen into reusable, installable, versioned files.

---

## How Skills work together

Skills cross-reference one another through **shared context**, so the GTM background does not have to be re-explained every time. The canonical shared context lives in two foundation files under `references/`:

- `references/gtm-principles.md` — the **operating principles** behind every GTM action (outcomes over output, evidence-based, AI as a lever).
- `references/brand-voice.md` — **voice and tone**, keeping client-facing messaging consistent across docs, social, announcements, and reports.

Because the `skills` CLI installs one skill directory at a time, each SKILL.md **inlines the shared context it needs** (as a "Shared Context" section) so every skill works standalone. The `references/` files remain the canonical, extended versions for repo readers and for the "fork and customize" workflow.

```
references/                     ← canonical shared context (extended versions)
├── gtm-principles.md
└── brand-voice.md
        │
        ├── devtool-positioning/        positioning, persona, messaging hierarchy
        ├── dev-content-engine/         AI topic mine → draft → multi-channel adapt → measure
        ├── dev-channel-campaign/       GTM campaigns across X / HN / Reddit / communities
        ├── dev-community-listening/    listen → triage signal → insight-to-content
        ├── devrel-gtm-metrics/         awareness → signup → activation → retention → advocacy
        └── client-gtm-report/          weekly client-ready GTM report & signal grading
```

The **Related Skills** section inside each skill documents the full cross-reference map.

---

## Available Skills

| Skill | Description |
| --- | --- |
| [devtool-positioning](skills/devtool-positioning/) | Define or refine positioning, target developer persona, and core messaging for a devtool before any GTM motion. |
| [dev-content-engine](skills/dev-content-engine/) | Run an AI-powered developer content engine: mine topics from signal, draft with AI, adapt across blog / docs / X / LinkedIn / HN, and measure what converts. |
| [dev-channel-campaign](skills/dev-channel-campaign/) | Plan and run GTM campaigns for a devtool across developer channels, with launch cadence and AI-assisted A/B. |
| [dev-community-listening](skills/dev-community-listening/) | Monitor communities, social, and issues to triage signals and turn them into marketing intelligence and content ideas. |
| [devrel-gtm-metrics](skills/devrel-gtm-metrics/) | Define and track the DevRel GTM funnel — awareness, signup, activation, retention, advocacy — for client reporting. |
| [client-gtm-report](skills/client-gtm-report/) | Produce a weekly, client-ready GTM report with signal grading and recommended next actions. |

> The current set is the initial 6 core skills for AI marketing-style DevRel; more will be added as real-world client work surfaces new needs.

---

## Installation

**Option 1 · CLI install (recommended)**

```bash
npx skills add zzoeyliu/ai-gtm
```

To install specific skills only:

```bash
npx skills add zzoeyliu/ai-gtm --skill devtool-positioning dev-content-engine
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
Fork this repo → adapt `references/` and each skill to the specific devtool client you serve → clone locally and use.

---

## Usage

After installation, describe your needs in natural language and the agent will match the right skill. For example:

- *"Our devtool client can't explain what they do — help me write a positioning statement and a persona"* → invokes `devtool-positioning`
- *"We keep writing blog posts nobody signs up from — build us a content engine that starts from real developer questions"* → invokes `dev-content-engine`
- *"We're shipping v2 next month; give me a launch cadence and a channel plan"* → invokes `dev-channel-campaign`
- *"What are developers saying about us vs the competitor? Turn it into content ideas"* → invokes `dev-community-listening`

You can also invoke the skills directly with slash commands: `/devtool-positioning`, `/dev-content-engine`, `/dev-channel-campaign`, `/dev-community-listening`, `/devrel-gtm-metrics`, `/client-gtm-report`.

---

## Skill Categories

- **Positioning**: `devtool-positioning` — who it's for, the job it wins, messaging hierarchy.
- **Content (AI engine)**: `dev-content-engine` — topic mine, draft, multi-channel adapt, measure.
- **Channels & Campaigns**: `dev-channel-campaign` — launch cadence, channel mix, A/B.
- **Listening & Intelligence**: `dev-community-listening` — signal triage, insight-to-content.
- **Metrics**: `devrel-gtm-metrics` — GTM funnel, north-star, leading/lagging.
- **Reporting**: `client-gtm-report` — weekly client-ready report, signal grading.

---

## Roadmap

The current set is the initial 6 core skills. More will be added based on real client work. The following directions are **planned** (not yet shipped — proposals via Issues are welcome):

- `devtool-competitor-battlecard` — build comparison and objection-handling cards per competitor.
- `dev-paid-growth` — paid dev-channel experiments (ads, sponsored content) with AI-optimized creative.
- `dev-event-gtm` — GTM playbook for conferences, meetups, and hackathons.
- `devlifecycle-email` — lifecycle email / in-product nudges driving activation and retention.

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
