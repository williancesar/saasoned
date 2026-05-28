# Worldview — the four cross-cutting stances

Each stance follows the suite's standard shape:
**Definition → Source → When it applies → When it does NOT → Decision cue →
Worked micro-example → Common failure it prevents.**

These stances govern *every* sibling. A sibling may sharpen a stance for its
domain but never contradict one.

---

## 1. Distribution-first thinking

**Definition.** Distribution (how the product reaches users) and positioning
(what it is and who it's for) are first-class design problems, addressed *while*
the product is built — not afterward. A superior product does not earn its own
distribution.

**Source.** Thiel & Masters, *Zero to One* — "a great product with no
distribution channel is a bad business"; the engineer's bias that good products
sell themselves is false. Reinforced by Kahl, *The Embedded Entrepreneur* —
"build it and they will come" fails because no audience is waiting.

**When it applies.** Any product/feature decision; any "should we build X"
question; any roadmap. Always, by default.

**When it does NOT.** Never fully off, but de-emphasize when the engagement is
explicitly internal tooling with a captive mandated user base (no acquisition
problem exists). Even then, adoption ≈ distribution.

**Decision cue.** Before approving build work, ask: *"Through which specific
channel will the first 100 of the right users arrive, and who owns that?"* No
credible answer → distribution is unsolved → fix that before more build.

**Worked micro-example.** *vai-nascer-v2*: "let's add a contraction timer" — the
distribution-first question is *not* "is the timer good" but "what gets a
first-trimester pregnant woman to install at all, and how does that pull in the
partner/family members whose access depends on her subscription?" The timer is
product; the install trigger and the family pull are distribution.

**Failure it prevents.** Months of polish on a product nobody can find or be
told about.

---

## 2. Niche-monopoly before scale

**Definition.** Deliberately pick a market segment small enough that you can
dominate it, win it completely, then expand into adjacent segments from that
base of strength.

**Source.** Thiel, *Zero to One* (monopoly via a small market you own; the
power law — a few bets dominate outcomes). Moore, *Crossing the Chasm*
(beachhead segment; bowling-alley expansion; D-Day niche domination).

**When it applies.** Pre-traction and early-traction products; any "who is our
market" question; any temptation to widen the audience to grow the number.

**When it does NOT.** A genuine, defended monopoly expanding into a *new*
adjacent niche (still niche-by-niche, just not the first one). Not a license to
go broad — it's the same rule applied again.

**Decision cue.** *"Can we be the obvious first choice for this exact segment
within a defined time, with current resources?"* If the segment is too big to
dominate, it is the wrong segment — narrow it until the answer is yes.

**Worked micro-example.** *family-agent*: "families with kids" is not a
beachhead. "Two-parent households already coordinating via a shared calendar,
with school-age children, who have abandoned a paper chore chart" is one — small
enough to saturate, specific enough to message.

**Failure it prevents.** Spreading thin across a market too large to win,
landing nowhere, beating no competitor decisively.

---

## 3. Traction is a parallel track (the 50% rule)

**Definition.** Pursuing traction and building product are two separate tracks
run **at the same time**, with roughly equal attention. Traction work is not a
phase that starts after launch.

**Source.** Weinberg & Mares, *Traction* — the 50% rule: spend ~50% of effort
on traction, ~50% on product. Plus the Critical Path: only do product work that
serves the next traction milestone.

**When it applies.** Every stage from idea onward. Especially when the team's
instinct is "we'll do marketing once the product is ready."

**When it does NOT.** A pure research/discovery sprint with an explicit,
time-boxed learning goal and no growth goal yet — but the *next* sprint
re-balances to 50/50.

**Decision cue.** *"What fraction of this week went to reaching/learning from
users vs. building?"* Persistently <30% on traction → you are violating the
rule; rebalance and trim product scope to the Critical Path.

**Worked micro-example.** *vai-nascer-v2*: while engineers build the family-
access flow, an equal effort runs a positioning test and one inner-ring channel
test. If both can't progress in parallel, scope is too big — cut product to the
Critical Path.

**Failure it prevents.** A finished product launched into silence with no
tested channel and no audience.

---

## 4. Everything is a cheap test before it is a bet (the Bullseye master loop)

**Definition.** Growth advances by one cheap, measured experiment at a time:
brainstorm options → rank into rings → run small tests → double down on the one
with signal → kill the rest. This loop sequences the entire suite.

**Source.** Weinberg & Mares, *Traction* (Bullseye Framework; test cheaply
before committing). The application engine is `growth-experiments`.

**When it applies.** Any "should we do X to grow" decision, any channel/feature/
positioning/network choice. The default mode of all siblings.

**When it does NOT.** A forced one-way door with no cheap test available (e.g.,
a regulatory/contractual commitment) — then reason explicitly about expected
value instead, and say you are doing so.

**Decision cue.** *"What is the cheapest test that would change our mind in
under ~2 weeks, and what result kills this?"* If you can't state the kill
condition, you're betting, not testing.

**Worked micro-example.** *family-agent*: instead of "build a referral program"
(a bet), test "manually offer 20 existing users a reward for one invite each"
(a test) — cheap, measured, killable, and it tells you whether referral is even
a candidate channel before any engineering.

**Failure it prevents.** Large irreversible spend on an untested channel,
feature, or market — premature scaling.
