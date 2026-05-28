# Distribution Power Law, the Dead Zone, and CAC

**Source.** Thiel & Masters, *Zero to One* (the distribution chapter and the
power law).

---

## Distribution power law

**Definition.** Distribution channels follow a power law: among all channels,
typically **one** works far better than all others combined. Most companies get
*zero* channels working; winners get *one*. The implication is concentration,
not a balanced portfolio.

**When it applies.** Whenever choosing how much effort to spread across
channels; whenever someone proposes "a multi-channel strategy" early.

**When it does NOT.** Late-stage companies with a saturated primary channel may
legitimately layer a second — but only after the first is genuinely maxed.

**Decision cue.** *"Have we found and saturated the one channel yet?"* If no,
adding channels is dilution. If yes (and only then), test the next.

**Worked micro-example.** *vai-nascer-v2* finding that organic content for
pregnancy-stage queries dominates: the correct move is to pour effort there, not
to "balance" it with paid social that tested weak.

**Failure it prevents.** A diluted portfolio where no channel ever gets enough
focus to dominate.

---

## The dead zone

**Definition.** The mid-range of customer acquisition where a product is *too
cheap* to justify a direct sales force (per-deal economics can't pay a
salesperson) yet *too expensive or considered* to grow purely through viral
loops or low-touch ads. Products stuck here have no viable acquisition path as
designed.

**Source.** *Zero to One* — the gap between personal sales and pure
advertising/viral.

**When it applies.** "CAC is stubbornly higher than it should be and no ad
tweak fixes it"; mid-priced products with a considered purchase but no sales
motion.

**When it does NOT.** Clearly low-touch self-serve (viral/ads viable) or clearly
high-value enterprise (sales viable) — those aren't in the zone.

**Decision cue.** Plot: would a salesperson's cost be covered by one deal? If
no — and the purchase is too considered for pure viral/ads — you're in the dead
zone. The fix is usually **pricing or positioning** (raise value/price into a
sales motion, or simplify into a self-serve viral motion), *not* another ad
campaign. Route to `growth-positioning`.

**Worked micro-example.** A mid-tier *vai-nascer-v2* family plan priced too low
for any human sales touch but framed as a considered family purchase that
doesn't spread on its own — dead zone. Resolve by either making the in-app
family invite genuinely viral (lower-touch) or repositioning/pricing toward a
clearer self-serve impulse — not by buying more ads.

**Failure it prevents.** Burning acquisition budget on a channel that is
economically impossible for the product as priced.

---

## CAC (and why CLV gates it)

**Definition.** CAC is the fully-loaded cost to acquire one paying customer via
a channel. A channel is only viable if CLV exceeds CAC with margin.

**Source.** *Zero to One* (CLV must exceed CAC).

**Decision cue.** Estimate CAC *during* the inner-ring test, not after scaling.
If CLV ≤ CAC, the channel is dead regardless of volume — do not scale it (hub
Guardrail). The CLV > CAC threshold mechanics live in `growth-experiments`.

**Failure it prevents.** Scaling a channel whose unit economics guarantee
losses — the most expensive form of premature scaling.
