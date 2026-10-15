---
name: dev-content-writing
description: Write technical content developers actually read — blogs, tutorials, release notes, and social posts — for your own brand or for an open-source project you support. Use when drafting developer-facing technical content, when content needs to drive action rather than impressions, or when you want AI-assisted drafting that follows a proven structure. Covers structure frameworks, title formulas, code sample rules, and voice standards.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Developer Technical Content Writing

## When to Use

- Writing a technical blog, tutorial, release announcement, or social post.
- The goal is to make developers actually read and act, not just browse.

## Core Principles

1. **Answer "what does this mean for me" before explaining the mechanism.**
2. **Code samples must be copy-paste runnable with expected output.**
3. **Speak developer language; no marketing filler.**
4. **One piece, one clear conclusion or action.**
5. **Small test before full push**: before writing the long version, validate the angle with a short post or a discussion — cheaply test whether the idea lands.
6. **Feed experience back**: record which tone / angle got accepted into the voice reference so the next piece starts warmer.

## Structure Template (blog / tutorial)

1. **Hook**: a concrete pain point, or "if you've ever…".
2. **Context**: why this problem exists.
3. **Solution**: step-by-step + code.
4. **Verification**: how to confirm it worked.
5. **Close**: next step / related resources.

## Title Formulas

- "How to solve Z in Y with X"
- "Getting started with X: from 0 to your first working example"
- "Why we dropped X for Y"

## Code Rules

- State the runtime environment and versions.
- Annotate the key lines.
- Give expected output — it prevents the "why won't this run" frustration.

## Voice

- Professional, never condescending.
- Concrete, verifiable, fact-based.
- Starting point: "help the developer succeed".

| Scenario | Tone |
|---|---|
| Docs / tutorials | Clear, stepwise, neutral |
| Community Q&A | Friendly, empathetic, point to the next step |
| Announcements | Concise, lead with value and changes |
| Social | Relaxed, opinionated, link included |

Never use: exaggerated claims ("best", "revolutionary"), speaking in a project's official voice (unless you truly are an official member), or unverified data and promises.

## Gotchas

- **Code that isn't copy-paste runnable destroys trust faster than any typo.** State the environment and version, annotate key lines, and show expected output. A reader who burns 20 minutes on a broken snippet never comes back.
- **"Revolutionary" and "best-in-class" read as marketing to developers.** Describe what changed and let readers judge. Specifics persuade; superlars repel.
- **Don't write the long guide before validating the angle.** A 3,000-word tutorial built on an assumption nobody shares is the expensive version of a wrong bet. Test the core claim with a short post or discussion first.
- **One post, one action.** If you can't name the single next step for the reader, the draft isn't finished. A post that asks for three actions gets none.
- **Tutorials rot.** Pin versions and dates in the intro ("written for v0.9, January 2026") so readers on newer versions know what to distrust.

## Publishing Checklist

- [ ] Does the title make the value obvious at a glance?
- [ ] Does the code run as copied?
- [ ] Is there a "next step" for the reader?

## Related Skills

- [launch-runbook](../launch-runbook/) — launch content (announcements / release notes) follows the runbook's timeline and messaging.
- [issue-discussion-triage](../issue-discussion-triage/) — mine high-frequency questions for material; turning Q&A into docs cuts repeat questions at the source.
- [devrel-metrics](../devrel-metrics/) — content reads, engagement, and conversions enter the metrics funnel; use data to judge content ROI.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/voice-and-tone.md` — full voice and tone guide
- `references/community-principles.md` — community operating principles
