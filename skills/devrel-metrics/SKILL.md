---
name: devrel-metrics
description: Define, track, and report the key metrics of developer ecosystem operations. Use when setting quarterly goals, reporting to leadership, or evaluating the ROI of community and content work. Covers north-star metric selection, the conversion funnel, tiered KPIs, data sources, reporting cadence, and common pitfalls.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Developer Ecosystem Metrics (DevRel Metrics)

## When to Use

- Setting quarterly goals, reporting to leadership, or evaluating operations ROI.

## Core Principles

1. **One north star, not ten.**
2. **Funnel thinking**: awareness → onboarding → adoption → contribution.
3. **Metrics serve decisions, not vanity.**

## North Star (examples)

- **Infrastructure-type projects**: weekly active adopters (people genuinely using it).
- **Community-type projects**: monthly active contributors.

## Conversion Funnel

| Stage | Metrics |
|---|---|
| Awareness | Impressions, stars, social reach |
| Onboarding | Docs visits, first clone, example runs |
| Adoption | Production usage, dependency added |
| Contribution | Issues / PRs, doc patches, answers |

## Tiered KPIs

- **Growth**: new user / new contributor growth rate.
- **Engagement**: active discussions, first-response time.
- **Health**: issue close rate, contributor retention.

## Data Sources

- GitHub API: stars / forks / issues / PRs.
- Social platforms: reach / engagement.
- Docs analytics: visits / search terms.

## Reporting Cadence

- **Weekly**: signals and anomalies (see `community-weekly-report`).
- **Monthly / quarterly**: funnel movement and goal attainment.

## Common Pitfalls

- Treating stars as adoption (a star is not usage).
- Tracking metrics nobody looks at.
- Too many goals → lost focus.

## Gotchas

- **Stars are vanity unless paired with an adoption proxy.** Track installs, production usage, or dependency additions alongside stars. A repo with 10k stars and 12 weekly users is a marketing artifact, not a product.
- **Don't report a funnel you can't measure at both ends.** If the gap between "awareness" and "adoption" can't be quantified, someone will fill it with a guess — and that guess will harden into strategy.
- **Quarterly targets set without a baseline are wishes, not goals.** Measure the current state for at least 2–4 weeks before committing to a number. "Double weekly active users" is meaningless when nobody knows the current count.
- **Version your metric definitions.** "Active contributor" redefined mid-quarter makes every trend line unreadable. When a definition changes, note it in the report and restate history where feasible.
- **One metric per decision.** If a metric doesn't change any decision you make, stop tracking it — every reported number costs attention.

## Checklist

- [ ] Is there exactly one north-star metric?
- [ ] Does every KPI map to a decision or owner?
- [ ] Is the baseline measured before targets are set?

## Related Skills

- [community-weekly-report](../community-weekly-report/) — the weekly report is the carrier for weekly-cadence metrics: definitions live here, presentation lives there.
- [dev-content-writing](../dev-content-writing/) — content engagement and conversions enter the awareness / adoption funnel stages, used to evaluate content ROI.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/community-principles.md` — community operating principles
- `references/voice-and-tone.md` — voice and tone
