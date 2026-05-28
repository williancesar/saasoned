# Experiment design — cheap test, prioritization, kill condition

**Source.** Weinberg & Mares, *Traction* — test cheaply before committing; the
Bullseye ranking discipline. This file owns *how to build the test*; the
frameworks being tested live in the siblings.

---

## The cheapest test that changes your mind

**Definition.** The smallest, fastest action whose result would actually alter
the decision. Not a small version of the eventual build — a probe designed to
*disprove* the hypothesis quickly and cheaply.

**When it applies.** Before any spend on a channel/feature/positioning/network
move.

**When it does NOT.** Genuine one-way doors with no cheap proxy (regulatory,
contractual) — then reason explicitly by expected value and *say so*.

**Decision cue.** Ask: *"What is the cheapest thing we could do in ≤ ~2 weeks
that would make us abandon this if it's wrong?"* If you can't name it, you don't
understand the hypothesis well enough to spend on it.

**Worked micro-example.** Test "Speaking Engagements as a channel" for
*family-agent* by doing **one** talk to a gathered target audience with a
tracked CTA — not by building a webinar program.

**Failure it prevents.** Expensive builds answering questions a cheap probe
would have settled.

---

## Prioritization (which test first)

**Definition.** Rank candidate tests by **(belief-changing power) ×
(cheapness/speed to signal)**, anchored to the Bullseye ring order from
`growth-traction-channels` (inner ring first). Practitioner scoring schemes
(e.g., ICE/RICE) are acceptable *tools*, but the canonical anchor is Bullseye —
test the inner ring, in parallel, first.

**Decision cue.** If two tests tie, run the one whose *kill* result eliminates
the most future work. Never run more inner-ring tests than you can give a real
(not 10%) effort to in parallel.

**Failure it prevents.** Burning the calendar on low-information or
already-knowable tests while the decisive one waits.

---

## Kill condition & decision rule (set before running)

**Definition.** The pre-committed result that ends the test, plus what each
outcome triggers. Decided **before** the test starts; never adjusted after
seeing data.

**When it applies.** Every experiment, always.

**When it does NOT.** Never optional. A test with no kill condition is a bet.

**Decision cue.**

```
Before running, write:
  signal threshold  = <number/criterion decided now>
  kill condition    = <number/criterion decided now>
  decision rule     = signal → X ; kill → Y ; ambiguous → 1 tighter iteration → forced keep/kill
After running:
  threshold unchanged?  → conclude honestly
  tempted to move it?   → REFUSE; that is post-hoc rationalization (cite hub Guardrail)
```

**Worked micro-example.** *vai-nascer-v2* content-channel test: signal = ≥ N
qualified first-trimester installs in 14 days; kill = below N; ambiguous band →
one revised content angle, then decide. Moving N after seeing 0.7N is forbidden.

**Failure it prevents.** Endless "promising" experiments that never resolve, and
post-hoc threshold-moving that manufactures false signals.
