---
name: community-weekly-report
description: Summarize open-source community activity on a weekly cadence for your team or the community itself. Use when syncing community status weekly, when scattered signals need to converge into decision-ready information, or when "I'm operating this seriously" needs to be visible to leadership. Covers the report template, metrics to track, signal grading, and distribution channels.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Community Weekly Report

## When to Use

- Weekly status sync for your team / maintainers.
- Scattered community signals need to converge into decision-ready information.

## Core Principles

1. **The weekly report is decision input, not a log.**
2. **Grade signals**: what needs action now, what is just recorded.
3. **Always include "recommended actions for next week".**

## Template

```
# Community Weekly Report (YYYY-Www)

## Key Metrics
- New stars / forks:
- New issues / closed:
- New discussions / replied:
- New contributors:

## Signals This Week
- 🔴 Blocker: [needs immediate action]
- 🟡 Watch: [worth monitoring]
- 🟢 Good: [positive progress]

## Notable Discussions
- [Discussion link + one-line takeaway]

## Recommendations for Next Week
- [Action 1]
- [Action 2]
```

## Metrics List

- **Growth**: stars / forks / new contributors.
- **Health**: issue close rate, first-response time.
- **Content**: docs visits, blog reads.

## Signal Grading

- 🔴 **Blocker**: security, main-flow outage, loss of a key contributor.
- 🟡 **Watch**: rising repeat questions, concentrated inquiries on one module.
- 🟢 **Good**: contribution growth, positive feedback.

## Distribution

- Internal: team channel / weekly meeting.
- Public: pinned community Discussion (optional).

## Gotchas

- **A report that's only numbers is a dashboard, not a report.** Every signal needs a "so what" and a proposed action. Numbers without interpretation get skimmed and ignored.
- **Don't grade a week green because nothing exploded.** Absence of signals is not health — check the leading indicators (question volume trend, first-response time, newcomer count). A quiet week often means a quiet community, not a healthy one.
- **Red signals need an owner and a date.** A blocker listed without both will be "noted" every week until it becomes an incident.
- **The same yellow item three weeks running is a red item you're avoiding.** Recurring watch items are either escalated or consciously dropped — they don't get to linger forever.
- **Report the trend, not just the level.** "42 open issues" means little; "open issues up 30% for 3 weeks while close rate fell" is a decision.

## Checklist

- [ ] Does every signal have a "so what" and a proposed action?
- [ ] Does every 🔴 have an owner and a date?
- [ ] Are leading indicators checked, not just absence of fires?

## Shared Context

- Grade signals by blast radius and urgency, not by who complained loudest.
- Respect and privacy: don't quote private threads or personal data in reports.
- Evidence-based: cite official sources, no invented numbers.

## Related Skills

- [devrel-metrics](../devrel-metrics/) — the report's metrics and signals are the data foundation for monthly / quarterly funnel reviews.
- [issue-discussion-triage](../issue-discussion-triage/) — blocker / watch signals in the report map directly to triage escalation items.
- [launch-runbook](../launch-runbook/) — post-launch data retrospecting is one input to the weekly report.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/community-principles.md` — community operating principles
- `references/voice-and-tone.md` — voice and tone
