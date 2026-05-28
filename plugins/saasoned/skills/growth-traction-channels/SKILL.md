---
name: growth-traction-channels
description: Pick and operationalize the ONE distribution channel that moves the needle, using Traction's 19 channels and the Bullseye Framework plus Zero to One's distribution power law and dead zone. Use when the user asks how to get users, which marketing/distribution channel to use, why growth is flat, why CAC is too high, how to run cheap channel tests, or whether to add or switch channels.
---

# Growth: Traction Channels

Owns channel selection and operations. Hub: `growth-foundations` (worldview,
shared vocabulary, router). This sibling does not redefine hub terms.

**Stance.** There are 19 channels; you brainstorm all, test the inner ring
cheaply, and **focus the ONE** that shows a traction signal. Spreading effort
across many channels is the default failure, not a hedge.

## Frameworks index

| Framework | Source | Depth |
|---|---|---|
| The 19 traction channels | Weinberg & Mares, *Traction* | [references/nineteen-channels.md](references/nineteen-channels.md) |
| Bullseye (brainstorm → rank → test → focus) | *Traction* | [references/bullseye.md](references/bullseye.md) |
| Distribution power law + the dead zone + CAC | Thiel & Masters, *Zero to One* | [references/distribution-power-law.md](references/distribution-power-law.md) |

## Bullseye — the operating procedure (checklist)

1. **Brainstorm.** One concrete idea for *every* one of the 19 channels — no
   skipping a channel because it "feels wrong." (See the catalog.)
2. **Rank into rings.** Inner = 3 most promising, testable now. Middle =
   possible. Outer = long shots. Rank on plausible reach × cost × time-to-signal
   for *this* product's beachhead.
3. **Test the inner ring — cheaply, in parallel.** Each test answers: roughly
   what does it cost to acquire a customer here, how many are reachable, are
   they the right ones? Cheap = days-to-2-weeks, small spend, a kill condition.
4. **Focus the ONE.** If a channel shows a traction signal, drop the others and
   pour effort into it until it tops out (the distribution power law: one
   channel usually dominates).
5. **Re-run Bullseye** only when the focused channel saturates or breaks — not
   before. (Signal threshold / kill condition: `growth-experiments`.)

The 50% rule and Critical Path are hub worldview — apply them, don't restate.

## Decision cues

- **"Which channel?" with zero users** → full Bullseye pass; do not pre-judge.
- **"Add another channel?"** → only if the current one is saturated *and* shows
  a signal. Otherwise this is premature diversification — refuse and cite.
- **"Scale this channel" with no signal yet** → **refuse** (hub Guardrail 1).
  Cite Bullseye/50% rule; design the cheap test instead.
- **CAC seems too high and unfixable** → check the **dead zone** (*Zero to
  One*): order value too small for direct sales, too large for viral/ads. Fix
  is usually positioning/pricing (route to `growth-positioning`), not a new ad
  set.
- **"It works for me but doesn't pull new users"** → likely a network product,
  not a channel problem → route to `growth-network-effects`.

## When this skill does NOT apply

- Problem is "users don't understand what this is" → `growth-positioning`.
- Problem is "is the problem even real" → `growth-customer-discovery`.
- Problem is "they sign up then leave" → `growth-habit-loops`.
- You only need to define the success threshold/metric → `growth-experiments`.

## Anti-patterns (this skill's catalog)

1. **Channel diversification too early** — six channels at 10% each; none gets a
   real test. Rule: focus one. (Hub anti-pattern 3.)
2. **Skipping channels in brainstorm** — discarding "Speaking" or "Engineering
   as Marketing" on vibes before a single idea. Rule: one idea per all 19.
3. **Scaling on noise** — mistaking a handful of conversions for a signal. Rule:
   define the kill condition first (`growth-experiments`).
4. **Ignoring the dead zone** — pouring ad budget into an economically
   impossible CAC. Rule: diagnose dead zone; fix pricing/positioning.
5. **Confusing a channel problem with a retention or network problem.**

## Worked example (illustrative — not a product spec)

*family-agent* (Android + .NET), zero users. Brainstorm hits all 19; inner ring
ranked: **App-store/Existing Platforms** (Play Store optimization), **Community
Building** (parenting subreddits/Facebook groups), **Engineering as Marketing**
(a free "family chore-load calculator" web tool). Three cheap tests, two weeks:
ASO keyword variant; 20 genuine community posts answering coordination pain; one
shippable mini-tool with an install CTA. Focus whichever returns the right users
at viable cost; ignore the other 16 until it saturates.

## See also

- Hub: `growth-foundations`
- `growth-positioning` (fix the dead zone / who the channel targets)
- `growth-network-effects` (when "no growth" is really cold start)
- `growth-experiments` (defines the signal, kill condition, CLV > CAC gate)
