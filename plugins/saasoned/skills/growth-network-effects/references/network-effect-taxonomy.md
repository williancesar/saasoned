# Network-Effect Taxonomy, Come-for-the-Tool, Anti-Network Effects

**Source.** Andrew Chen, *The Cold Start Problem*.

---

## Network-effect taxonomy

**Definition.** "Network effects" is not one thing. Distinguish:

- **Acquisition effects** — the network drives new-user acquisition (viral
  invites, word of mouth from existing members).
- **Engagement effects** — more/active users make the product more engaging for
  existing users (more content, more matches, more activity).
- **Economic effects** — the network improves monetization/unit economics over
  time (better conversion, pricing power, lower CAC).

Also: **direct** (same-side: more users → more value for that side) vs.
**cross-side** (more of side A → more value for side B, e.g., buyers↔sellers);
and **data network effects** (more usage → better data → better product).

**When it applies.** Diagnosing *which* effect is weak; deciding what to
strengthen at Escape Velocity.

**When it does NOT.** Single-user products with no other-user dependency — don't
retrofit network language onto them.

**Decision cue.** Name which of acquisition/engagement/economic effects you
actually have and which is the weak link; "improve network effects" is too vague
to act on. Strengthen the specific weak loop.

**Failure it prevents.** Generic "grow the network" effort that doesn't target
the loop that's actually broken.

---

## Come for the tool, stay for the network

**Definition.** A single-player **tool** delivers standalone value that solves
the cold start (the product is useful with zero other users), while a **network**
layer accrues underneath and becomes the long-term retention and moat.

**When it applies.** Cold Start, when the hard side won't show up for an empty
network — give them solo value first.

**When it does NOT.** When no honest standalone tool value exists — don't fake
it; forced "tool" with no real utility just adds friction.

**Decision cue.** Is there genuine single-user value *before* any network forms?
If yes, lead with the tool to break the cold start, then layer the network. If
no, you need a different seeding strategy (hand-built supply).

**Worked micro-example.** *vai-nascer-v2*: the pregnant woman gets real solo
value (tracking, week-by-week guidance) *before* any family joins — that solves
her cold start; the family network ("stay for the network") accrues afterward
and becomes the retention/moat. This is why the hard side (her) can be seeded
without a network existing yet.

**Failure it prevents.** Requiring a network to exist before anyone gets value —
the unbreakable empty-room cold start.

---

## Anti-network effects

**Definition.** When **more users *decrease* value**: congestion, spam, low-
quality content, trust erosion, overcrowded supply/demand, degraded matching.
The network can shrink as it grows.

**When it applies.** Ceiling stage; "more users but the experience got worse";
quality complaints rising with scale.

**When it does NOT.** Genuine undersupply (that's Cold Start, the opposite
problem) — diagnose direction before prescribing.

**Decision cue.** If adding users degrades the core experience, **fix
quality/congestion before adding more users** — and treat raw user count here as
a *vanity metric* (cross-ref `growth-experiments`). Growth tactics now make it
worse, not better.

**Worked micro-example.** A community feature in *family-agent* that, opened
broadly, fills with spam/noise so real coordination value drops — adding users
accelerates the decline. Fix moderation/scoping (or keep it bounded to the
atomic family network) before any growth push.

**Failure it prevents.** Scaling user count straight into experience collapse
while a rising vanity metric hides it.
