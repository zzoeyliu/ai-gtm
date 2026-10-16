---
name: dev-channel-campaign
description: Plan and run GTM campaigns for a devtool across developer channels — X, Hacker News, Reddit, dev communities, and launch platforms. Use when a client is shipping a version or feature, or wants always-on growth. Covers launch cadence (T-14 to T+7), channel mix, demo-driven growth, and AI-assisted A/B experimentation.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Dev Channel & Campaign

## When to Use

- A devtool client is shipping a version, feature, or campaign and needs a repeatable GTM playbook.
- Growth depends on one-off posts instead of a planned channel mix.
- You want to test messages across channels without burning the whole audience.

## Core Principles

1. **Developer GTM runs on docs + demo + hands-on**, not slogans.
2. **Each channel owns a job**: HN for technical credibility, X for reach, Reddit for community trust, docs for activation.
3. **The first 48h after a launch are the golden window — someone must be present.**
4. **Small test before full push**: validate the message with a warm-up post or a core-user preview before the full campaign.
5. **Feed experience back**: record the channel mix and messaging that worked for direct reuse next time.

## Procedure

1. **Goal**: pick one objective (signups / activation / a specific feature adoption).
2. **Message**: pull the relevant pillar from the positioning hierarchy.
3. **Channel plan**: assign each channel a role and a format (see template).
4. **Demo**: ship one reproducible example that proves the claim.
5. **Launch**: T-0 tag/release + announcement + social; staff the Q&A window.
6. **Experiment**: run 2–3 message variants via AI-assisted A/B on the same channel.
7. **Retro**: capture what converted, what wasted, and the follow-ups.

## Templates

### Channel mix

| Channel | Job | Format |
|---|---|---|
| Hacker News | Technical credibility | Show the result + method, no hype |
| X / Twitter | Reach + narrative | Insight thread, demo clip |
| Reddit (r/*) | Community trust | Honest answer, link only if relevant |
| Dev communities | Deep users | Discussion, Q&A, feedback |
| Docs / blog | Activation | Runnable walkthrough |

### Launch timeline

| Time | Action |
|---|---|
| T-14 | Goal + message; draft announcement / release note |
| T-10 | Reproducible demo; internal docs review |
| T-7 | Finalize release note; pre-write social variants |
| T-3 | Core-user preview; set launch-day monitoring |
| T-0 | Tag/release + announcement + social; community sync |
| T+1–2 | Golden Q&A window: staff comments and DMs |
| T+7 | Retro: data, feedback, follow-ups |

### A/B variant brief (for AI)

> Generate 3 launch posts for [feature] on X. Variant A leads with speed, B with cost, C with a concrete user story. Keep each under 280 chars. No superlatives.

## Gotchas

- **Never announce a date before the release note is final.** Scope creep between announcement and tag is the #1 cause of missed launch days. The announcement is the last artifact, not the first.
- **A demo that only works on the author's machine is a launch-day bug report.** If it can't run from a clean checkout, it isn't ready.
- **The 48h Q&A window needs a named owner, not "the team".** "Everyone is responsible" means nobody answers the 2 a.m. comment.
- **Spamming Reddit with launch links burns trust permanently.** Answer the question, mention the tool only when it's the actual answer.
- **Don't A/B test more than one variable at a time.** Testing three messages and three audiences at once tells you nothing. One variable, clean read.
- **Capture day-zero data on launch day itself.** Signups, stars, and discussion volume from the first 24h are your baseline; you can't reconstruct them later.

## Checklist

- [ ] Is there one launch objective (not "awareness")?
- [ ] Does each channel have a distinct job and format?
- [ ] Is there a named owner for the T+0 to T+2 window?
- [ ] Is the demo reproducible from a clean checkout?
- [ ] Is day-zero data capture scheduled?

## Shared Context

- Outcomes over output: we measure whether developers adopt, not whether they liked the post.
- Evidence-based: cite real signals and proof; never invent metrics or claims.
- Developer respect: no hype, speak their language, never fake "best".
- AI is a lever, not autopilot: AI drafts and analyzes; a human owns the message and the judgment.

## Related Skills

- [devtool-positioning](../devtool-positioning/) — campaigns execute the messaging hierarchy.
- [dev-content-engine](../dev-content-engine/) — announcements and social copy come from the content engine.
- [dev-community-listening](../dev-community-listening/) — post-launch signal tells you which message landed.
- [client-gtm-report](../client-gtm-report/) — the 7 days of post-launch data flow into the weekly report.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/brand-voice.md` — brand voice and tone for launch content
- `references/gtm-principles.md` — GTM operating principles
