---
name: growth-foundations
description: Entry point and router for distribution, go-to-market, growth, and customer-acquisition questions, grounded in Zero to One, Traction, Hooked, The Mom Test, Crossing the Chasm, Obviously Awesome, The Embedded Entrepreneur, and The Cold Start Problem. Use when the user asks how to grow, get users, pick a marketing channel, position or describe a product, validate an idea, improve retention, start a network/marketplace, or decide what to test next — and to route the question to the right growth-* sibling skill.
---

# Growth Foundations

The hub for distribution, go-to-market, and growth. It carries the cross-cutting
worldview, defines the shared vocabulary **once**, and **routes** every question
to the sibling that owns the mechanics. Siblings link back here; do not redefine
hub vocabulary in a sibling.

**Stance, not neutrality.** This suite is opinionated and grounded in named
sources. It will refuse certain recommendations (see Guardrails). Take the
stance; don't hedge into "it depends" without giving the decision rule.

## The worldview (4 stances)

Full treatment with sources, when-it-applies/does-not, decision cue, worked
example, and the failure each prevents: [references/worldview.md](references/worldview.md).

1. **Distribution-first.** A great product with no distribution channel is a bad
   business (Thiel & Masters, *Zero to One*). Distribution and positioning are
   designed *with* the product, never bolted on after. "Build it and they will
   come" is a predictable failure (Kahl, *The Embedded Entrepreneur*).
2. **Niche-monopoly before scale.** Win a market small enough to dominate, then
   expand (Thiel, *Zero to One*; Moore's beachhead, *Crossing the Chasm*).
   Competing broadly on day one is the error.
3. **Traction is a track you run in parallel with product.** Spend pursuing
   traction roughly equal to spend building product — the 50% rule
   (Weinberg & Mares, *Traction*). Product quality does not substitute for a
   distribution channel.
4. **Everything is a cheap test before it is a bet.** One channel/feature/claim
   at a time, measured, killed fast if no signal (the Bullseye master loop).
   This loop is the orchestration spine for the whole suite.

## The master loop (orchestration spine)

Resolve any growth effort in this order; each step is run *as an experiment*
(`growth-experiments` cross-cuts all of them):

```
Position  →  Discover the truth  →  Pick ONE channel  →  [Solve cold start]  →  Build the habit
(who/what)   (is the problem real)   (Bullseye)            (only if a network)    (retention)
```

You cannot pick a channel for a product you cannot describe (positioning first),
and you cannot trust a channel test built on a fictional problem (discovery
before spend). Skip "solve cold start" only if the product has no network effect.

## Decision tree — route the question

Identify what the question is *really* about, then hand off:

```
What is the question really about?

├─ Who is this for? What is it? What category? "Nobody understands what we do."
│   Naming, framing, competitive comparison, the pitch.
│      → growth-positioning           (Obviously Awesome 5+1; Crossing the Chasm)
│
├─ Is the problem real? What do users actually do? How do I interview / find
│   an audience / build in public / know I'm building the right thing?
│      → growth-customer-discovery    (The Mom Test; The Embedded Entrepreneur)
│
├─ How do I get users? Which channel? No growth. CAC too high. Marketing plan.
│      → growth-traction-channels     (Traction 19 channels + Bullseye)
│
├─ Marketplace / social / multi-sided / community won't start. Chicken-and-egg.
│   "It works for me but new users see an empty room."
│      → growth-network-effects       (The Cold Start Problem)
│
├─ Users try once and leave. No retention. How do I make this a habit / a
│   recurring engagement loop?
│      → growth-habit-loops           (Hooked; Fogg Behavior Model)
│
└─ How do I test / prioritize this? What metric? Is it working? Am I ready to
    scale? "Our numbers are up" (but which numbers?).
       → growth-experiments          (cross-cuts all; Traction test-cheaply)

If several apply, follow the master-loop order above. Every branch is
ultimately executed through growth-experiments.
```

## Guardrails (Claude refuses these, with the cited reason)

State the refusal and the source; offer the correct next step instead.

- **Won't recommend scaling a channel with no traction signal.** Cite the
  Bullseye discipline and the 50% rule (*Traction*). Correct step: design a
  cheap inner-ring test first (`growth-traction-channels`).
- **Won't recommend scaling a network with no atomic network yet.** Cite the
  atomic-network requirement (*The Cold Start Problem*). Correct step: seed and
  saturate one smallest viable network (`growth-network-effects`).
- **Won't endorse "build it and they will come."** Cite *Zero to One*
  (distribution thesis) and *The Embedded Entrepreneur* (audience-first).
- **Won't treat vanity metrics as a success signal.** Cite `growth-experiments`;
  demand a North Star / one-metric-that-matters tied to value delivered.
- **Won't broaden the target before the niche is dominated.** Cite *Zero to
  One* and *Crossing the Chasm* (beachhead).

## Shared vocabulary

Defined once here; siblings use these exactly and do not redefine them. Full
definitions with sources: [references/vocabulary.md](references/vocabulary.md).

Distribution channel · Traction (vs. product) · 50% rule · Monopoly /
niche-monopoly · Power law (of returns *and* of distribution) · CAC · CLV/LTV ·
Bullseye (inner/middle/outer ring) · Beachhead / whole product · Atomic network ·
Hard side · Positioning · North Star / one-metric-that-matters · Traction signal ·
Premature scaling · Habit Zone.

## Cross-cutting anti-patterns

Suite-wide failures (each sibling adds its own narrower catalog). Full catalog:
[references/anti-patterns.md](references/anti-patterns.md).

1. Building before distribution is designed.
2. Scaling before a traction signal / before an atomic network.
3. Diversifying channels early instead of focusing the ONE that works.
4. Vanity metrics standing in for value delivered.
5. Broad-market positioning before niche domination.
6. Treating customer interviews as pitches (contaminating the data).

## Worked example (running, illustrative — not a product spec)

**vai-nascer-v2** (pregnancy/baby; network-member access tied to the pregnant
woman's subscription/trial). A growth question — "should we run ads?" — routes:
positioning is undefined ("a pregnancy app" is a category, not a position) →
`growth-positioning` first. Only then is "the pregnant woman in her first
trimester, in Brazil" a beachhead a channel test can target. Jumping straight to
ads violates the master loop and Guardrail 1.

**family-agent** (Android app + .NET backend). "Which channel?" with zero users
is a Bullseye question (`growth-traction-channels`), but "do families even want
this?" is a discovery question (`growth-customer-discovery`) and must precede
channel spend.

## See also (siblings — built after this hub is approved)

- `growth-traction-channels` — Traction's 19 channels + Bullseye operations.
- `growth-positioning` — Obviously Awesome 5+1; Crossing the Chasm.
- `growth-habit-loops` — Hooked Hook Model; Fogg; Manipulation Matrix.
- `growth-customer-discovery` — The Mom Test; The Embedded Entrepreneur.
- `growth-network-effects` — The Cold Start Problem.
- `growth-experiments` — cheap prioritized tests; North Star metric.
