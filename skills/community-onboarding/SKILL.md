---
name: community-onboarding
description: Design newcomer welcome flows, onboarding checklists, and FAQs for open-source developer communities (including AI / LLM projects). Use when a new member joins your community or user group, when writing or rewriting "how to get started" docs, or when members report "I don't know where to start" or "the barrier is too high". Covers welcome message templates, environment prep checklists, first-contribution suggestions, and replies to common hesitations.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Community Onboarding

## When to Use

- A new member joins your open-source community or user group.
- You need to write or redo "how to get started" documentation.
- Community feedback says "I don't know where to begin" or "the barrier is too high".

## Core Principles

1. **The first 5 minutes decide stay-or-leave**: let newcomers complete one small thing before asking anything deeper.
2. **Compress environment prep to the minimum**: use a ready-made environment instead of forcing a local setup.
3. **Lower the first-contribution barrier with `good first issue`.**
4. **Be specific in welcomes**: name the person and point to one clear path — never a generic broadcast "welcome aboard".

## Procedure (4 steps)

1. **Welcome**: reply point-to-point in the newcomer's thread within 24 hours.
2. **Direct**: hand them a "start here" checklist (see Templates).
3. **First contribution**: recommend 1–3 `good first issue` or documentation tasks.
4. **Follow up**: after the first contribution merges, thank them publicly and point to the next step.

## Templates

### Welcome message (copy-paste ready)

> Welcome @user! Glad you're interested in this project. To get started, check out [getting-started doc], then pick a task labeled `good first issue` — if you get stuck, ping me anytime in Discussions.

### Newcomer checklist

- [ ] Read the README section "what problem this project solves"
- [ ] Run the minimal example once (use a hosted environment / online demo link)
- [ ] Introduce yourself in one line in Discussions (who you are, what you want to solve)
- [ ] Claim one `good first issue`

### First-contribution recommendation

> The 3 issues below are good first contributions, each estimated under 30 minutes: [link1] [link2] [link3]. I'll help review once you're done.

## Gotchas

- **Never make a full local dev setup the first step.** A newcomer who spends two hours fighting dependencies before seeing the project work is usually gone. Hosted notebooks, online demos, or a single docker command first; local setup later, for people who came back.
- **A generic broadcast welcome is worse than nothing.** "Welcome to our community!" posted in a channel reads as automated noise. Name the person, reference something specific they said or did, and give exactly one next action.
- **A first question left unanswered for 24h+ is read as "this project is dead".** Speed beats completeness for first contact — a short "good question, looking into it, back to you today" preserves the newcomer.
- **The `good first issue` pool goes stale.** If the label has no open issues, the entire flow stalls at step 3. Replenish it weekly and retire issues that grew too complex.
- **Don't promise review turnaround you can't keep.** "I'll review immediately" on a PR you'll see in three days burns more trust than an honest "I review PRs on weekends".

## Checklist

- [ ] Is there a working "5-minute quick start" entry point?
- [ ] Is the `good first issue` label continuously stocked?
- [ ] Does every newcomer get a human reply within 24h?

## Shared Context

- Newcomers get extra patience; a confusing first experience is usually a docs problem, not a person problem.
- Decisions and changes stay public and traceable.
- Credit contributions publicly — visibility is the main currency of open-source communities.

## Related Skills

- [issue-discussion-triage](../issue-discussion-triage/) — repeated newcomer questions are the raw material for labels and standard replies; onboarding FAQs feed back into the triage system.
- [dev-content-writing](../dev-content-writing/) — welcome messages and checklists are external content; onboarding is the first class of content output.
- [community-weekly-report](../community-weekly-report/) — welcome → first contribution → follow-up conversion is a "health" signal source for the weekly report.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/community-principles.md` — community operating principles
- `references/voice-and-tone.md` — voice and tone
