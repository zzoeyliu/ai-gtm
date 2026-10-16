---
name: devrel-gtm-metrics
description: Define and track the DevRel GTM funnel for a devtool client — awareness, signup, activation, retention, and advocacy. Use when reporting GTM ROI to a client or setting quarterly targets. Covers north-star selection, funnel metrics, leading and lagging indicators, and AI-assisted reporting.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# DevRel GTM Metrics

## When to Use

- Setting quarterly GTM targets for a devtool client.
- Reporting marketing ROI to a client or internal stakeholders.
- Content and campaigns run, but nobody can say what they returned.

## Core Principles

1. **One north star, not ten.**
2. **Funnel thinking**: awareness → signup → activation → retention → advocacy.
3. **Metrics serve decisions, not vanity** — a number nobody acts on is noise.
4. **Leading indicators predict, lagging indicators confirm** — watch both.

## North Star (examples)

- **Infra / library tools**: weekly active adopters (real usage, not stars).
- **Platform / API tools**: activated accounts per week (first successful call).

## GTM Funnel

| Stage | What it measures | Example metrics |
|---|---|---|
| Awareness | Reached developers | Impressions, HN/Reddit reach, search volume |
| Signup | Opted in | Account created, repo starred, newsletter sub |
| Activation | Got value once | First successful run, first API call, demo deployed |
| Retention | Came back | Weekly active, 2nd-week return, dependency kept |
| Advocacy | Pulls others in | Referral, community answer, case-study yes |

## Leading vs Lagging

- **Leading**: content reads, trial starts, docs searches — move before revenue.
- **Lagging**: activated accounts, retained users, pipeline — confirm after.

## Data Sources

- GitHub / package registry: clones, installs, stars, forks.
- Product analytics: signups, activation events, retention cohorts.
- Web / docs: traffic, search terms, time on page.
- Social / community: reach, signals from [dev-community-listening](../dev-community-listening/).

## Reporting Cadence

- **Weekly**: leading signals and anomalies (see [client-gtm-report](../client-gtm-report/)).
- **Monthly / quarterly**: funnel movement and goal attainment.

## Gotchas

- **Stars are vanity unless paired with an adoption proxy.** A repo with 10k stars and 12 weekly users is a marketing artifact, not a product. Track installs or active usage alongside.
- **Don't report a funnel you can't measure at both ends.** If the gap between "signup" and "activation" can't be quantified, someone fills it with a guess that hardens into strategy.
- **Quarterly targets without a baseline are wishes.** Measure the current state for 2–4 weeks before committing to a number.
- **Version your metric definitions.** "Activated user" redefined mid-quarter makes every trend line unreadable. Note changes and restate history where feasible.
- **One metric per decision.** If a metric changes no decision, stop reporting it — every number costs attention.
- **Don't claim attribution you can't defend.** "This campaign drove 200 signups" needs a trackable link or UTM; otherwise say "associated with", not "caused".

## Checklist

- [ ] Is there exactly one north-star metric?
- [ ] Does every funnel stage have at least one measurable metric?
- [ ] Are leading indicators separated from lagging ones?
- [ ] Is the baseline measured before targets are set?

## Shared Context

- Outcomes over output: we measure whether developers adopt, not whether they liked the post.
- Evidence-based: cite real signals and proof; never invent metrics or claims.
- Developer respect: no hype, speak their language, never fake "best".
- AI is a lever, not autopilot: AI drafts and analyzes; a human owns the message and the judgment.

## Related Skills

- [client-gtm-report](../client-gtm-report/) — the weekly report is the carrier for weekly-cadence metrics.
- [dev-content-engine](../dev-content-engine/) — content reads, clicks, and signups enter the funnel.
- [dev-community-listening](../dev-community-listening/) — community signal feeds awareness and advocacy stages.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/gtm-principles.md` — GTM operating principles
- `references/brand-voice.md` — brand voice and tone
