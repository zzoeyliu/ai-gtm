---
name: launch-runbook
description: Run a version, feature, or campaign launch for an open-source developer project. Use when preparing a release and you need a repeatable T-14 to T+7 checklist instead of improvised execution. Covers the launch timeline, channel responsibilities (RACI), pre-launch checklist, and post-launch retro template.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Launch Runbook

## When to Use

- Preparing a new version, feature, or community campaign.
- You want the launch process repeatable instead of dependent on improvisation.

## Core Principles

1. **Developer launches run on docs + demo + hands-on**, not slogans.
2. **Clear channel division**: announcements, social, and community each own their lane.
3. **The first 48h after launch are the golden Q&A window — someone must be present.**
4. **Small test before full push**: launches are expensive; validate the message with a warm-up post or core-contributor preview before the full campaign.
5. **Feed experience back**: record the channel mix and messaging that worked into this runbook for direct reuse next time.

## Timeline

| Time | Action |
|---|---|
| T-14 | Define launch goals and messaging; draft announcement / release note |
| T-10 | Prepare demo / minimal runnable example; internal docs review |
| T-7 | Finalize release note; prepare social copy (multiple versions) |
| T-3 | Notify core contributors / early preview; set up launch-day monitoring |
| T-0 | Launch: tag/release + announcement + social; community sync |
| T+1–2 | Golden Q&A window: staff Issues / Discussions / comments |
| T+7 | Retro: data, feedback, follow-ups |

## Channel Division (simplified RACI)

| Channel | Owner | Content |
|---|---|---|
| GitHub Release | Maintainer | Release note, upgrade guide |
| Discussion / blog | DevRel | Technical deep-dive, use cases |
| Social (X / LinkedIn) | DevRel | Highlights, links, @mentions |
| Community groups | Community ops | Syncs, Q&A routing |

## Pre-Launch Checklist

- [ ] Release note covers: changes / how to upgrade / breaking changes / acknowledgments
- [ ] Demo or example reproduces in one step
- [ ] Monitoring and on-call rotation in place

## Retro Template

- Goal attainment (installs / stars / discussion volume / new issues)
- What worked / what was wasted
- Issues to follow up and documentation gaps

## Gotchas

- **Never announce a date before the release note is final.** Scope creep between announcement and tag is the #1 cause of missed launch days. The announcement is the last artifact, not the first.
- **The T-3 contributor preview is mandatory for breaking changes.** A breaking change discovered on launch day becomes firefighting instead of Q&A — and early contributors are your best pre-launch testers.
- **If the demo isn't reproducible from a clean checkout by someone outside the team, it isn't ready.** "Works on my machine" demos convert launch-day excitement into launch-day bug reports.
- **The 48h Q&A window needs a named owner on rotation, not "the team".** "Everyone is responsible" means nobody answers the 2 a.m. comment.
- **Capture day-zero data on launch day itself.** Install counts, stars, and discussion volume from the first 24h are your baseline; you cannot reconstruct them later.

## Checklist

- [ ] Is there a named on-call owner for T+0 to T+2?
- [ ] Has the T-3 preview happened for anything breaking?
- [ ] Is day-zero data capture scheduled?

## Shared Context

- Verify before you claim: cite official sources, don't invent numbers or promises.
- Small test before full push: validate messaging cheaply before spending on the big version.
- Feed experience back: what worked this launch is recorded for the next one.

## Related Skills

- [dev-content-writing](../dev-content-writing/) — announcements, release notes, and social copy are produced by the content skill; this runbook provides the timeline and messaging, the content skill handles execution.
- [community-weekly-report](../community-weekly-report/) — the 7 days of post-launch data and feedback flow into the weekly report's retro and signal grading.
- [community-onboarding](../community-onboarding/) — a feature launch must ship with updated getting-started docs and fresh `good first issue` tasks to absorb the incoming users.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/voice-and-tone.md` — voice and tone for launch content
- `references/community-principles.md` — community operating principles
