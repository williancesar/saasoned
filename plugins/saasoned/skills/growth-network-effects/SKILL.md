---
name: growth-network-effects
description: Diagnose and grow network/marketplace/social products using The Cold Start Problem's atomic network, hard side, the five-stage arc, come-for-the-tool, and anti-network effects. Use when the user has a marketplace, social, multi-sided, or community product that won't take off, describes a chicken-and-egg problem, says it works for them but new users see an empty room, or asks how to seed or scale a network.
---

# Growth: Network Effects

Owns cold-start and network-driven growth. Hub: `growth-foundations`
(worldview, shared vocabulary, router). Does not redefine hub terms.

**Stance.** You do not scale a network — you scale **atomic networks**. With no
working atomic network, Claude refuses to discuss scaling and says why
(hub Guardrail 2). Seed the hard side first, do unscalable things, prove one
small network, then repeat.

## Frameworks index

| Framework | Source | Depth |
|---|---|---|
| Atomic network · the hard side · seeding | Chen, *The Cold Start Problem* | [references/atomic-network.md](references/atomic-network.md) |
| The five-stage arc | *The Cold Start Problem* | [references/the-arc.md](references/the-arc.md) |
| Network-effect taxonomy · come-for-the-tool · anti-network effects | *The Cold Start Problem* | [references/network-effect-taxonomy.md](references/network-effect-taxonomy.md) |

## Cold-start diagnosis (run before any growth advice)

1. **Is this actually a network product?** Does value depend on *other users*
   being present? No → this is a channel/retention problem; route out.
2. **Name the atomic network.** The *smallest* set of users that is stable and
   useful on its own (e.g., one city, one company, one friend group, one
   classroom). If you can't name it, that's the first deliverable.
3. **Identify the hard side.** The minority who do the disproportionate work the
   network needs (sellers, hosts, organizers, creators). Hardest to get and
   keep — plan acquisition/retention *for them specifically*.
4. **Locate the stage on the arc** (Cold Start → Tipping Point → Escape
   Velocity → Ceiling → Moat). Advice differs per stage.
5. **Only then** discuss tactics. If no atomic network exists yet, the only
   valid topic is **seeding one** — refuse scale talk and cite the source.

## Decision cues

- **"It works for me but new users see an empty room"** → classic empty-network
  cold start; the atomic network isn't reached for a new user. Seed density in
  one network, don't broaden.
- **"Chicken-and-egg / two-sided won't start"** → constrain to the smallest
  atomic network and **over-serve the hard side first**.
- **"Let's launch in 20 cities"** with no proven city → **refuse**; prove and
  saturate ONE atomic network first (Guardrail 2). Cite *The Cold Start
  Problem*.
- **"Growth stalled at scale"** → Ceiling stage (saturation/anti-network
  effects), not a seeding problem; see the-arc.md + anti-network effects.
- **"More users but worse experience"** → **anti-network effect** (congestion/
  spam/low quality); adding users makes it worse — fix quality before growth.

## When this skill does NOT apply

- Value does **not** depend on other users → it's a normal product:
  acquisition `growth-traction-channels`, retention `growth-habit-loops`.
- "What is this / who for" → `growth-positioning`.
- "How do we measure network health / when is it 'working'" →
  `growth-experiments` (define the atomic-network success threshold there).

## Anti-patterns (this skill's catalog)

1. **Scaling with no atomic network** (hub anti-pattern 2; hard Guardrail) —
   broad launch into empty rooms.
2. **Ignoring the hard side** — acquiring easy-side users while supply/creators/
   hosts starve; the network collapses.
3. **Spreading thin across many networks** instead of saturating one to density.
4. **Premature geographic/segment expansion** before the first network tips.
5. **Ignoring anti-network effects** — chasing raw user count while quality/
   congestion degrades value (overlaps the vanity-metric anti-pattern).
6. **Treating a network product as a funnel** — optimizing single-user
   acquisition while the network stays below critical density.

## Worked example (illustrative — not a product spec)

*vai-nascer-v2*: the family network is the product's network effect. **Atomic
network = one pregnant woman + her invited partner/family** (small, stable,
useful alone). **Hard side = the pregnant woman** — access is tied to her
subscription/trial; without her, no family member has value. Therefore seed and
retain *her* first; family-member growth is downstream. "Acquire lots of family
members" before the hard side is acquired is exactly the inverted error. No
discussion of scaling acquisition until that single-family atomic network
reliably forms and sticks.

## See also

- Hub: `growth-foundations`
- `growth-traction-channels` (channel to seed the hard side specifically)
- `growth-habit-loops` (retain the hard side once seeded)
- `growth-experiments` (define the atomic-network success/kill threshold)
