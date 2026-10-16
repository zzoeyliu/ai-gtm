---
name: dev-community-listening
description: Monitor developer communities, social, and issues to triage signals and turn them into marketing intelligence and content ideas for a devtool client. Use when you need to know what developers actually say, where the friction is, and which conversations to join or seed. Covers listening sources, a signal taxonomy, and the insight-to-content workflow.
license: CC-BY-4.0
metadata:
  author: zzoeyliu
  version: "1.0.0"
---

# Dev Community Listening

## When to Use

- A devtool client wants to know what developers say about them and competitors.
- Content feels disconnected from what the audience actually asks.
- Support and sales hear the same objection repeatedly but nothing flows back to marketing.

## Core Principles

1. **Listen where developers are, not where it's easy** — Issues, subreddits, HN, Discord, Stack Overflow, search console.
2. **Classify signal before reacting** — a complaint, a feature ask, a competitor switch, and a praise are four different actions.
3. **Every signal is a content brief waiting to happen** — the best posts answer a real, recurring question.
4. **Join, don't broadcast** — in community spaces, answer the question; mention the tool only when it's the answer.
5. **Protect trust**: never fake a user, never astroturf, never quote people out of context.

## Procedure

1. **Source map**: list the client's relevant channels (owned Issues + 2–3 community spaces + search terms).
2. **Collect**: pull recurring threads weekly; tag each by signal type.
3. **Triage**: grade by frequency and intent (see taxonomy).
4. **Route**: feedback → product; objection → content; competitor mention → battlecard; praise → proof.
5. **Act**: turn the top signal into a content piece or a community reply within the week.

## Signal Taxonomy

| Signal | Example | Action |
|---|---|---|
| Pain | "X is a pain to set up" | Content: setup guide |
| Feature ask | "Wish it had Y" | Product feedback + waitlist note |
| Competitor switch | "moving from A to B" | Battlecard + comparison content |
| Objection | "too complex for my team" | Content: simpler path |
| Praise / proof | "shipped in a day" | Testimonial, case study |
| Confusion | "not sure what it does" | Positioning fix |

## Templates

### Weekly signal digest

```
# Listening Digest (YYYY-Www)
- Top signal: [verbatim quote] → action: [content / feedback / battlecard]
- Recurring ask: [topic] → backlog it / write it
- Competitor chatter: [who said what] → note for next campaign
- Confusion to fix: [where] → positioning or docs fix
```

### Community reply (seed, not shout)

> Saw this come up a few times — here's the shortest path we found: [link]. Happy to go deeper if useful.

## Gotchas

- **Listening without acting is just a dashboard.** If the top signal this week produces no content or no product note, the loop is broken.
- **Astroturfing destroys a devtool brand permanently.** Never post fake questions or praise. Developers spot it and remember.
- **Answering with a link and no help reads as spam.** In community spaces, give the answer first, link second — if at all.
- **Don't over-react to one loud voice.** Grade by frequency across sources; a single angry thread is noise until it recurs.
- **Quoting users without context backfires.** A trimmed complaint used as marketing fuel can go viral for the wrong reason. Get permission or anonymize.
- **Search-console questions are the highest-intent signal.** "how do I X with Y" with volume is a content brief with built-in demand — prioritize it.

## Checklist

- [ ] Do we have a source map covering owned + community + search?
- [ ] Is every signal tagged by type and routed to an action?
- [ ] Did the top signal this week produce a content piece or note?
- [ ] Are we joining conversations, not just broadcasting?

## Shared Context

- Outcomes over output: we measure whether developers adopt, not whether they liked the post.
- Evidence-based: cite real signals and proof; never invent metrics or claims.
- Developer respect: no hype, speak their language, never fake "best".
- AI is a lever, not autopilot: AI drafts and analyzes; a human owns the message and the judgment.

## Related Skills

- [dev-content-engine](../dev-content-engine/) — the signal source that feeds the topic mine.
- [devtool-positioning](../devtool-positioning/) — recurring confusion signals a positioning gap.
- [dev-channel-campaign](../dev-channel-campaign/) — competitor chatter informs campaign battlecards.
- [client-gtm-report](../client-gtm-report/) — signal volume and type feed the weekly report.

## References

Canonical full versions (for repo readers; not bundled when this skill is installed standalone):
- `references/brand-voice.md` — brand voice and tone
- `references/gtm-principles.md` — GTM operating principles
