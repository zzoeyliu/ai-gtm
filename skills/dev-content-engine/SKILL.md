---
name: dev-content-engine
description: Run an AI-powered developer content engine for a devtool — mine topics from real signals, draft with AI, adapt one piece across blog / docs / X / LinkedIn / Hacker News, and measure what lands. Use when a client needs developer content that drives signups rather than impressions. Covers topic mining, AI drafting, multi-channel adaptation, and content metrics.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Dev Content Engine

## When to Use

- A devtool client needs a steady stream of developer content but can't staff a full editorial team.
- Content exists but doesn't convert — reads are high, signups are flat.
- You want AI to multiply a small team's output without sounding robotic.

## Core Principles

1. **Mine topics from signal, not from a content calendar.** The best devtool content starts in Issues, forums, and "how do I…" searches.
2. **One piece, one job**: every article or post exists to move a developer one step down the funnel.
3. **AI drafts, human steers**: AI produces 80% of the words; a human owns the claim, the example, and the voice.
4. **Write once, adapt many**: produce a strong long-form piece, then slice it into social, docs, and discussion replies.
5. **Small test before the long version**: validate the angle with a short post before investing in a 3,000-word guide.

## Procedure

1. **Mine**: pull recurring questions from the client's Issues, subreddits, HN, and search console.
2. **Decide the job**: for each topic, pick the funnel stage it serves (awareness / activation / retention).
3. **Draft with AI**: feed the topic + positioning + proof into the AI; require runnable code and a cited source.
4. **Adapt**: turn the long-form into a blog, a docs page, an X thread, a LinkedIn post, and a HN-ready abstract.
5. **Publish & measure**: ship, then track reads → clicks → signups per channel; kill what doesn't convert.

## Templates

### Topic card

- **Signal source**: [issue / forum / search term]
- **Question developers ask**: "[verbatim]"
- **Funnel job**: [awareness / activation / retention]
- **Proof we can use**: [benchmark / repo / customer story]

### AI draft brief (give this to the model)

> Write a developer blog post about [topic]. Audience: [persona]. Voice: [brand-voice link]. Must include a copy-paste runnable code sample with expected output. Cite [source]. End with one clear next step. No hype.

### Multi-channel slice

- **Blog**: full walkthrough + code.
- **X thread**: the 3 non-obvious points, one insight per tweet.
- **LinkedIn**: the "why this matters" framing for engineering leaders.
- **HN abstract**: the technical claim + reproducible result, no marketing.

## Gotchas

- **AI-generated code that doesn't run destroys trust instantly.** Every snippet must be executed before publishing. A broken quickstart is worse than no post.
- **"Best-in-class" and "revolutionary" read as marketing to developers.** Describe what changed and let readers judge. Specifics persuade; superlatives repel.
- **Don't ship the long guide before testing the angle.** A 3,000-word tutorial built on an assumption nobody shares is the expensive version of a wrong bet. Test the core claim with a short post first.
- **One post, one action.** If you can't name the single next step for the reader, the draft isn't finished. A post that asks for three actions gets none.
- **Slicing without re-voicing sounds like spam.** The X thread and the LinkedIn post need different openings, not the same sentence pasted twice.
- **Measure signups, not likes.** A post with 50 upvotes and zero signups is a vanity win; a quiet post that converts 5 developers is the real one.

## Checklist

- [ ] Did the topic come from a real developer signal?
- [ ] Does the draft have runnable, executed code?
- [ ] Is there one clear next step for the reader?
- [ ] Is each channel slice re-voiced, not copy-pasted?
- [ ] Are we tracking signups, not just reads?

## Shared Context

- Outcomes over output: we measure whether developers adopt, not whether they liked the post.
- Evidence-based: cite real signals and proof; never invent metrics or claims.
- Developer respect: no hype, speak their language, never fake "best".
- AI is a lever, not autopilot: AI drafts and analyzes; a human owns the message and the judgment.

## Related Skills

- [devtool-positioning](../devtool-positioning/) — the positioning statement anchors every piece's message.
- [dev-community-listening](../dev-community-listening/) — the signal source that feeds the topic mine.
- [devrel-gtm-metrics](../devrel-gtm-metrics/) — content reads, clicks, and signups enter the funnel metrics.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/brand-voice.md` — brand voice and tone
- `references/gtm-principles.md` — GTM operating principles
