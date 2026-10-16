---
name: client-gtm-report
description: Produce a weekly GTM report for a devtool client or internal team. Use when syncing GTM status, grading signals, and recommending next actions. Covers the report template, signal grading (red / amber / green), growth signals, and client-ready framing.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Client GTM Report

## When to Use

- Weekly GTM status sync for a client or internal team.
- Scattered signals need to converge into decision-ready information.
- The client needs to see "the marketing is working" without reading raw analytics.

## Core Principles

1. **The report is decision input, not a log.**
2. **Grade signals**: what needs action now, what is just recorded.
3. **Always end with recommended actions** — and name an owner for each.
4. **Frame for the client**: lead with outcome and next step, not raw numbers.

## Template

```
# GTM Weekly — [Client] (YYYY-Www)

## Headline
[One sentence: are we on track, and the single most important move this week.]

## Funnel Snapshot
- Awareness: [reach / reach change]
- Signup: [new signups]
- Activation: [activated this week]
- Retention: [WAU / return rate]
- Advocacy: [referrals / case studies]

## Signals
- 🔴 Blocker: [needs action now] → owner / date
- 🟡 Watch: [worth monitoring]
- 🟢 Good: [positive momentum]

## What We Shipped
- [content / campaign / experiment]

## Recommended Next Actions
- [action 1] → owner
- [action 2] → owner
```

## Signal Grading

- 🔴 **Blocker**: signup drop, a broken demo, a competitor landing a key account, a trust incident.
- 🟡 **Watch**: rising CAC, a channel underperforming, recurring objection.
- 🟢 **Good**: activation up, a piece converted, a community win.

## Gotchas

- **A report that's only numbers is a dashboard, not a report.** Every signal needs a "so what" and a proposed action. Numbers without interpretation get skimmed and ignored.
- **Don't grade a week green because nothing exploded.** Absence of signals is not health — check the leading indicators (trial starts, content reads, search volume). A quiet week often means a quiet pipeline, not a healthy one.
- **Red signals need an owner and a date.** A blocker listed without both will be "noted" every week until it becomes an incident.
- **The same yellow item three weeks running is a red item you're avoiding.** Recurring watch items are either escalated or consciously dropped.
- **Report the trend, not just the level.** "42 signups" means little; "signups up 30% for 3 weeks while activation held" is a decision.
- **Never put unverified numbers in a client report.** If a metric isn't defensible, say "estimated" or omit it — a wrong number in a client deck is a trust event.

## Checklist

- [ ] Does the headline state the single most important move this week?
- [ ] Does every signal have a "so what" and a proposed action?
- [ ] Does every 🔴 have an owner and a date?
- [ ] Are leading indicators checked, not just absence of fires?
- [ ] Are all numbers in the report defensible?

## Shared Context

- Outcomes over output: we measure whether developers adopt, not whether they liked the post.
- Evidence-based: cite real signals and proof; never invent metrics or claims.
- Developer respect: no hype, speak their language, never fake "best".
- AI is a lever, not autopilot: AI drafts and analyzes; a human owns the message and the judgment.
- Client confidentiality: protect client data; never disclose unreleased plans without consent.

## Related Skills

- [devrel-gtm-metrics](../devrel-gtm-metrics/) — funnel metrics are the data foundation for this report.
- [dev-channel-campaign](../dev-channel-campaign/) — post-launch data is one input here.
- [dev-community-listening](../dev-community-listening/) — signal volume and type feed the grading.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/gtm-principles.md` — GTM operating principles
- `references/brand-voice.md` — brand voice and tone
