# Contributing

Thanks for considering a contribution to the **ai-gtm** skill library — AI-powered DevRel marketing / GTM skills for developer tools. This repo welcomes any skill, template, or fix that helps devtool teams and agencies do positioning, content, campaigns, listening, metrics, and reporting with AI.

## What You Can Contribute

- **New skills**: create a directory under `skills/` containing a `SKILL.md` (format below).
- **Skill enhancements**: add templates, checklists, or gotchas to existing skills.
- **Fixes**: terminology, links, wording errors.

## Skill File Format (SKILL.md)

Every skill directory must contain a `SKILL.md`. Frontmatter follows the [Agent Skills spec](https://agentskills.io/specification):

```yaml
---
name: your-skill-name        # kebab-case, must match the directory name
description: What the skill does and when to use it. Use when [triggers].
license: CC-BY-4.0
metadata:                    # optional but recommended
  author: your-github-id
  version: "1.0.0"
---
```

Recommended body structure:

1. **When to Use** — trigger scenarios.
2. **Core Principles** — the non-negotiables.
3. **Procedure / Steps** — actions a practitioner can follow directly.
4. **Templates** — copy-paste ready copy / checklists / briefs.
5. **Gotchas** — concrete, non-obvious mistakes to avoid (often the highest-value section).
6. **Checklist** — pre-completion self-check.
7. **Shared Context** — inline the shared principles / voice the skill needs.
8. **Related Skills** — cross-references.
9. **References** — canonical sources.

## Writing Guidelines

- **English only.** The major skill directories (skills.sh, agentskill.sh) render SKILL.md as the listing page and have international audiences; a Chinese-only skill is undiscoverable there.
- **Descriptions are the discovery surface.** Write them imperatively ("Use when…"), focused on user intent rather than implementation, keyword-rich, and under 1024 characters. This is the only thing an agent sees when deciding whether to load your skill.
- **Skills must be self-contained.** Users can install a single skill (`npx skills add zzoeyliu/ai-gtm --skill your-skill`), and the repo-root `references/` directory is **not** bundled with it. Inline any shared context your skill needs (principles, voice) as a compact "Shared Context" section, and point to the canonical `references/` files for repo readers only.
- **Concise over exhaustive.** Keep SKILL.md under 500 lines; split genuinely large material into per-skill `references/` files with explicit "load this when…" triggers.
- **GTM-first, AI as a lever.** Every skill should help move developers down a funnel stage (awareness → signup → activation → retention → advocacy) and show where AI drafts, analyzes, or scales — while a human owns the message and the judgment.
- **Evidence over adjectives.** No "best-in-class", no unverified numbers, no fake users. Cite real signals and proof.

## How to Submit

1. Fork this repo → create a branch → commit your changes.
2. In the PR, explain: which skill was added/changed and what GTM scenario it solves.
3. Merge after review.

You can also open an Issue describing your idea for the maintainer to follow up.

## Distribution Notes

- **Install**: `npx skills add zzoeyliu/ai-gtm [--skill <name>]` works immediately from GitHub — no publishing step needed.
- **skills.sh listing**: triggered by install telemetry from the `skills` CLI; a repo-root `skills.sh.json` can control grouping once listed.
- **agentskill.sh listing**: submit the repo URL at https://agentskill.sh/submit (web form).

## Code of Conduct

Be fact-based, respect developers, and cite information sources. Never speak in a client's official voice without authorization, and never invent metrics or testimonials.
