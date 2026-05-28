---
name: growth-experiments
description: Turn any growth framework into a prioritized, cheap, measurable test with a pre-stated kill condition; pick a North Star / one-metric-that-matters; reject vanity metrics; and gate against premature scaling. Use when the user asks how to test or prioritize a growth idea, what metric to track, whether a result is a real signal, whether they're ready to scale, or when any other growth-* skill needs its claim converted into an experiment.
---

# Growth: Experiments

The application engine. Hub: `growth-foundations` (worldview, shared vocabulary,
router). Every other sibling routes here to convert its framework into a test.
This skill does not own any framework's *content* — it owns turning content into
a falsifiable, cheap, prioritized experiment and judging the result.

**Stance.** Nothing scales without a pre-defined **traction signal** and a
**kill condition**. Vanity metrics are not evidence. Claude refuses to call a
result a signal, or to recommend scaling, when the bar wasn't set in advance
(hub Guardrails). State the refusal and the reason.

## Frameworks index

| Topic | Source | Depth |
|---|---|---|
| Experiment design · cheap test · prioritization · kill condition | Weinberg & Mares, *Traction* (test cheaply + Bullseye) | [references/experiment-design.md](references/experiment-design.md) |
| North Star / one-metric-that-matters · vanity vs. actionable · CLV > CAC · traction signal | *Zero to One* (CLV>CAC); growth canon | [references/metrics.md](references/metrics.md) |
| Scale-readiness gate · premature scaling · double-down vs. switch | *Traction*; *The Cold Start Problem* | [references/scale-readiness.md](references/scale-readiness.md) |

## The experiment card (default output)

Convert any proposal into this before any spend. Refuse to proceed if a field
is blank:

```
Hypothesis      : <specific, falsifiable — "X will cause Y for segment Z">
Framework basis : <which sibling/framework this operationalizes>
Cheapest test   : <smallest action that could disprove it, ≤ ~2 weeks>
Primary metric  : <one value-backed metric; NOT a vanity metric>
Success / signal: <threshold decided NOW, before running>
Kill condition  : <result that ends it — decided NOW>
Timebox         : <date/iteration limit>
Decision rule   : signal → <next>; kill → <stop/route>; ambiguous → <iterate once, then decide>
```

A test with no kill condition is a bet — name it as such and refuse to call its
outcome a "signal."

## Converting each sibling into a test

| Sibling | What it hands over | Becomes the experiment's… |
|---|---|---|
| `growth-traction-channels` | an inner-ring channel | hypothesis + CAC/volume/quality metric |
| `growth-positioning` | a rewritten 5(+1) / pitch | message test; metric = comprehension/conversion of the beachhead |
| `growth-habit-loops` | a Hook stage change (post–Manipulation Matrix) | habit-testing metric (value-backed habitual behavior) |
| `growth-customer-discovery` | a problem hypothesis | commitment/advancement as the metric (currency spent + next step) |
| `growth-network-effects` | one atomic network | success = that network self-sustains; never aggregate user count |

## Decision cues

- **"Is this working?"** → was a success threshold set *before* running? No →
  you cannot conclude; refuse to declare a signal, cite the reason.
- **"Our numbers are up"** → which number? If it's totals/installs/pageviews
  with no value or retention cut → **vanity metric**; demand the North Star.
- **"Ready to scale?"** → run the scale-readiness gate
  ([references/scale-readiness.md](references/scale-readiness.md)). Any gate
  fails → **refuse to recommend scaling**, cite *Traction* / *Cold Start
  Problem*, prescribe the missing proof instead.
- **"Which test first?"** → prioritize by cheapest-to-signal × belief-changing
  power, anchored to Bullseye ring order — not gut.
- **"It half-worked"** → ambiguous result → one tighter iteration, then a
  forced keep/kill; never "let it run and see."

## When this skill does NOT apply

- You need the *content* of a framework (channels, positioning, hooks, etc.) →
  go to the owning sibling first, then return here to test it.
- Pure strategy/worldview question with no testable proposition →
  `growth-foundations`.

## Anti-patterns (this skill's catalog)

1. **Vanity metrics as success** (hub anti-pattern 4) — totals that rise
   without proving value or driving a decision.
2. **No kill condition** — open-ended "experiments" that can't fail and so never
   inform anything.
3. **Premature scaling** — spending to scale before the signal/atomic network
   exists (hub anti-pattern 2; hard Guardrail).
4. **Post-hoc success bar** — moving the threshold after seeing the result.
5. **Metric soup** — many dashboards, no single North Star, no decision rule.
6. **Running expensive when a cheap test would answer it** — skipping the
   "cheapest test that changes our mind."

## Worked example (illustrative — not a product spec)

*family-agent* proposal: "build a referral program." Card: Hypothesis = existing
users will invite a co-parent if asked at the right moment (basis:
`growth-traction-channels` Viral). Cheapest test = manually offer 20 active
users a small reward for one invite (no engineering). Primary metric = accepted
invites that activate (value-backed), **not** invite links sent (vanity).
Signal = ≥ a pre-set activation rate; Kill = below it in 2 weeks. Decision rule:
signal → build the automated loop; kill → route back to
`growth-traction-channels` for the next inner-ring channel. Refuse to greenlight
the build before this test resolves.

## See also

- Hub: `growth-foundations`
- All siblings route *into* this skill to operationalize their frameworks:
  `growth-traction-channels`, `growth-positioning`, `growth-habit-loops`,
  `growth-customer-discovery`, `growth-network-effects`.
