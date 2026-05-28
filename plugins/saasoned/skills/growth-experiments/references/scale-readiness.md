# Scale-readiness gate, premature scaling, double-down vs. switch

**Sources.** Weinberg & Mares, *Traction* (don't scale before the signal;
Critical Path); Andrew Chen, *The Cold Start Problem* (no scaling without an
atomic network). This file operationalizes the hub's hard Guardrails.

---

## Premature scaling

**Definition.** Spending to scale a channel, feature, network, or org *before*
its success signal exists. The cardinal growth sin: it converts an unproven
hypothesis into a large, hard-to-reverse loss.

**When it applies.** Any "let's scale / increase budget / hire the team / launch
broadly" request.

**When it does NOT.** When every gate below passes — then scaling is the correct
move, not a risk.

**Decision cue.** If asked to scale, run the gate. **Any** fail → refuse, cite
the source, and prescribe the missing proof. This refusal is mandatory, not
advisory.

---

## The scale-readiness gate (all must pass)

```
1. Signal exists?        Pre-set threshold met, on an ACTIONABLE metric,
                         repeatable (not a one-off spike).         [Traction]
2. Economics clear?      CLV > CAC with margin for this channel.   [Zero to One]
3. Atomic network?       (Network products only) at least one atomic
                         network self-sustains unattended.   [Cold Start Problem]
4. One channel focused?  Not diversifying — scaling THE channel
                         with the signal.                           [Traction]
5. Whole product ready?  (Crossing the chasm) the beachhead can fully
                         adopt at scale.               [Crossing the Chasm]
6. Kill condition held?  The success bar was set before, not after.   [hub]

ANY box fails  → REFUSE to recommend scaling. Name the failed box,
                 cite its source, prescribe the missing proof, route to
                 the owning sibling.
ALL pass       → scaling is justified; proceed.
```

**Worked micro-example.** *vai-nascer-v2*: "we have 5,000 signups, let's buy
ads in 10 regions." Gate: box 1 fails (signups = vanity, no actionable signal),
box 3 fails (no evidence the single-family atomic network self-sustains). →
**Refuse**: cite *Traction* and *The Cold Start Problem*; prescribe — define an
actionable North Star, prove one self-sustaining family network — before any
regional ad spend.

---

## Double-down vs. switch

**Definition.** After a test resolves: **double down** (focus harder) when there
is a real signal and headroom; **switch** (return to Bullseye / next atomic
network) when the kill condition is hit or the channel saturates.

**Decision cue.**

```
Signal + not yet saturated      → double down; do not add other channels
Signal but saturating           → re-run Bullseye for the next channel
                                  (growth-traction-channels)
Kill condition hit              → stop; route back to the owning sibling
Ambiguous                       → ONE tighter iteration → forced keep/kill
                                  (never "leave it running")
```

**When it does NOT.** Don't switch off a winning channel out of novelty-seeking
— the distribution power law says the winner deserves disproportionate focus
until genuinely maxed.

**Failure it prevents.** Both abandoning a working channel too early and
clinging to a dead one too long — and, above all, scaling either without proof.
