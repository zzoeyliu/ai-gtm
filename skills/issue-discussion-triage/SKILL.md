---
name: issue-discussion-triage
description: Classify, label, prioritize, and reply to Issues and Discussions in open-source technical communities. Use when issues or discussions are piling up, when building a label system and priority standards, or when you need reusable standard replies that cut repetitive work. Covers a label taxonomy, severity matrix, reply templates, and escalation paths.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Issue / Discussion Triage

## When to Use

- Issues / Discussions are piling up and you need a consistent handling standard.
- You want to build a label system and priority criteria.
- You need copy-paste standard replies to reduce repetitive work.

## Core Principles

1. **Classify before responding**: labels are the foundation of operating at scale.
2. **Every reply points to a next step**: no dead-end answers.
3. **Merge duplicates**: point to the existing answer instead of re-explaining.
4. **Emotion first**: when someone is frustrated, acknowledge before solving.

## Label System (suggested)

| Label | Meaning |
|---|---|
| `bug` | Reproducible functional defect |
| `question` | Usage inquiry |
| `good first issue` | Suitable for newcomers |
| `docs` | Documentation-related |
| `duplicate` | Duplicate |
| `wontfix` / `out-of-scope` | Outside current scope |
| `needs-info` | Insufficient information, awaiting reporter |

## Severity Matrix

| Severity | Definition | Response SLA |
|---|---|---|
| P0 blocker | Main flow unusable | 24h |
| P1 major | Feature impaired but workaround exists | 3 days |
| P2 normal | Experience issue | 1 week |
| P3 minor | Suggestion / polish | Scheduled |

## Reply Templates

### Needs more information

> Thanks for the report! To help us pinpoint it, could you add: [environment / version / repro steps / error screenshot]? We'll follow up as soon as we have it.

### Duplicate / existing answer

> This was already discussed and resolved in #[number] — merging over there. If that thread doesn't cover your case, feel free to reply here.

### Resolved / closing

> Fixed in [version / PR]. Thanks for the report that made the project better 🎉 If convenient, please help verify.

### Out of scope

> This scenario is currently outside the project's scope. I've logged it in [Discussion / backlog] and will sync if the direction changes.

## Escalation Paths

- Can't judge severity → ask a maintainer.
- Security-related → follow the private disclosure process; no public discussion.
- Asked repeatedly → fold into FAQ / docs (see `dev-content-writing`).

## Gotchas

- **A label system nobody applies is worse than none.** Five labels actually used beat twenty defined and ignored. Start with the smallest set your team will genuinely apply, and add labels only when a category keeps recurring.
- **Closing a duplicate without linking the original frustrates the reporter.** Always link the canonical thread and explicitly invite them back if it doesn't cover their case — an unlinked close reads as a brush-off.
- **`needs-info` issues rot silently.** Without a timer they sit open for months. Close after ~2 weeks of no response with a friendly "reopen anytime with more info".
- **Never discuss security issues in public threads, even "just to confirm".** Public confirmation of a vulnerability starts the exploitation clock. Move to private disclosure in the first reply.
- **P0 is blast radius, not volume.** The loudest complainer is not automatically P0. Severity is judged by impact on the main flow — a single angry voice about a cosmetic bug is P3.
- **Standard replies are starting points, not scripts to blast.** A templated reply that ignores what the person actually wrote does more damage than no template. Adapt the first line to their specific situation.

## Checklist

- [ ] Does every issue have at least one label and one severity?
- [ ] Have P1 items past their SLA been escalated?
- [ ] Have high-frequency questions flowed back into the docs?

## Shared Context

- Safety before speed: security issues go through private disclosure, never public discussion.
- Respect and patience, especially with newcomers.
- Transparent and traceable: decisions stay public and reviewable.
- Never speak in a project's official voice unless you actually are an official member.

## Related Skills

- [community-onboarding](../community-onboarding/) — high-frequency questions become FAQ / getting-started docs, feeding back into newcomer onboarding.
- [dev-content-writing](../dev-content-writing/) — recurring questions turn into docs and tutorials, cutting repeat questions at the source.
- [community-weekly-report](../community-weekly-report/) — backlog volume, severity distribution, and SLA attainment are core weekly signals.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/voice-and-tone.md` — voice and tone for all external replies
- `references/community-principles.md` — community operating principles
