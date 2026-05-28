---
name: growth-habit-loops
description: Design and audit habit-forming retention loops using Hooked's Hook Model, the Fogg Behavior Model, variable-reward types, and the Manipulation Matrix as a mandatory ethics gate. Use when the user asks how to improve retention, make a feature sticky or habit-forming, build an engagement loop, why users try once and leave, or how to design notifications/triggers/rewards — and whenever a habit loop must be ethics-checked before recommending.
---

# Growth: Habit Loops

Owns retention via habit formation. Hub: `growth-foundations` (worldview,
shared vocabulary, router). Does not redefine hub terms.

**Stance.** A habit loop is only recommended after it passes the **Manipulation
Matrix**. A complete Hook that doesn't materially improve the user's life is
manipulation — Claude refuses to recommend it and says why. Engagement is not a
goal in itself; value-backed retention is.

## Frameworks index

| Framework | Source | Depth |
|---|---|---|
| Hook Model (Trigger → Action → Variable Reward → Investment) + Habit Zone | Eyal, *Hooked* | [references/hook-model.md](references/hook-model.md) |
| Fogg Behavior Model (B = MAT) | *Hooked* (B.J. Fogg) | [references/fogg-behavior-model.md](references/fogg-behavior-model.md) |
| Variable rewards (Tribe / Hunt / Self) | *Hooked* | [references/variable-rewards.md](references/variable-rewards.md) |
| Manipulation Matrix (ethics gate) | *Hooked* | [references/manipulation-matrix.md](references/manipulation-matrix.md) |
| Habit-testing | *Hooked* | [references/habit-testing.md](references/habit-testing.md) |

## Hook audit (checklist — find the missing stage)

Walk the four stages; name the first broken/absent one — that's the fix:

1. **Trigger.** External (notification, email, icon) *and* a target **internal**
   trigger (an emotion/situation the product attaches to). No internal trigger →
   no unprompted return.
2. **Action.** The simplest behavior in anticipation of reward. Debug via Fogg:
   is **motivation**, **ability**, or the **trigger** the missing factor?
   (Increase ability/simplicity before adding motivation.)
3. **Variable reward.** Reward present but *predictable* → habit won't form.
   Classify it (tribe/hunt/self) and confirm variability.
4. **Investment.** Does the user put something in (data, content, reputation,
   effort) that loads the next trigger and improves the product for them? No
   investment → no compounding, no stored value.

Then: **run the whole loop through the Manipulation Matrix before recommending
it** (mandatory — see below).

## The ethics gate (mandatory, before any recommendation)

Two questions (Manipulation Matrix):
- Would **you, the maker**, use it?
- Does it **materially improve the user's life**?

```
Improves life + maker uses it      → Facilitator   → recommend
Improves life + maker won't use it → Peddler        → recommend only with caution; likely a positioning/value gap
Doesn't improve life + maker uses  → Entertainer    → permissible only if honestly framed as entertainment
Doesn't improve life + maker won't → Dealer          → REFUSE. Cite Hooked. Do not design this.
```

If a requested loop lands in **Dealer**, refuse with the cited reason and
redirect to delivering real value (often `growth-positioning` or
`growth-customer-discovery`).

## Decision cues

- **"Users try once and leave"** → missing **internal trigger** and/or
  **investment**; not a notification-volume problem.
- **"They don't do the key action"** → Fogg: raise **ability** (simplify)
  before adding motivation or more triggers.
- **"Reward isn't working"** → check **variability** and reward *type* fit.
- **"How do we make this addictive?"** → reframe: run the Matrix; refuse if
  Dealer; otherwise design for value-backed habit, not "addiction."

## When this skill does NOT apply

- "They never come at all" (acquisition) → `growth-traction-channels`.
- "New users see an empty network" → `growth-network-effects`.
- "Is this even the right problem" → `growth-customer-discovery`.
- "How do we measure habit formation" → `growth-experiments` (this skill owns
  *habit-testing*; the North Star/metric mechanics live there).

## Anti-patterns (this skill's catalog)

1. **Manufacturing a habit with no ethics gate** (hub anti-pattern 7) — refuse
   Dealer-quadrant loops.
2. **External triggers only** — notification spam substituting for an internal
   trigger; drives churn and uninstalls.
3. **Predictable reward** — loyalty points with zero variability; no habit.
4. **No investment stage** — nothing stored, so no next-trigger load and no
   switching cost; the loop doesn't compound.
5. **Adding motivation when ability is the blocker** — Fogg inverted.
6. **Engagement as the North Star** — optimizing time-in-app detached from
   delivered value (route the metric question to `growth-experiments`).

## Worked example (illustrative — not a product spec)

*vai-nascer-v2* symptom tracker: **Trigger** internal = the recurring worry
"is this normal this week?"; external = a gentle weekly prompt. **Action** = log
one symptom (one tap — high ability). **Variable reward** (self + tribe) =
varied, reassuring week-specific context and, if shared, family reactions.
**Investment** = the logged history personalizes next week and pulls the
partner/family in (loads the next trigger, raises switching cost). Matrix: helps
the user and the maker would use it → **Facilitator** → recommend.

## See also

- Hub: `growth-foundations`
- `growth-network-effects` (retention via network, not habit, for multi-sided)
- `growth-customer-discovery` (find the real internal trigger truthfully)
- `growth-experiments` (habit-testing metric, North Star, not engagement vanity)
