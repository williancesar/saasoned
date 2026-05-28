# Metrics — North Star, vanity vs. actionable, CLV > CAC, traction signal

**Sources.** *Zero to One* (CLV must exceed CAC); the growth canon's
one-metric-that-matters / actionable-metric discipline (Lean Analytics lineage,
applied through *Traction*'s traction goal).

---

## North Star / one-metric-that-matters

**Definition.** The single metric that best captures **value delivered to the
user** and that the team optimizes *now*. One, not a dashboard. It changes by
stage but there is always exactly one focal metric.

**When it applies.** Always — every growth effort reports against it.

**When it does NOT.** Never absent; but the *choice* of metric changes by stage
(discovery → activation; network → atomic-network self-sustain; etc.).

**Decision cue.** Ask: *if this number goes up, did the user get more real
value?* If yes and it drives a decision → North Star candidate. If it can rise
while users get nothing → vanity (below).

**Worked micro-example.** *vai-nascer-v2* North Star ≠ "registered users." Try
"subscribers whose family network is active weekly" — rises only if real
value (the family-sync core) is delivered.

**Failure it prevents.** Optimizing a number disconnected from value.

---

## Vanity vs. actionable metrics

**Definition.** A **vanity metric** rises without proving value or informing a
decision (cumulative signups, pageviews, app installs, raw user count,
impressions, "total" anything). An **actionable metric** ties to value and
changes what you do (activation rate, retention by cohort, paid conversion,
CLV:CAC, atomic-network self-sustain rate).

**Decision cue.** Two filters — *(1) can it go up while users get nothing? (2)
does a change in it change our next action?* Up-with-no-value or
no-action-attached → vanity → **refuse to treat it as a signal**; demand the
actionable equivalent.

**Worked micro-example.** "Installs are up 40%" for *family-agent* → vanity
until cut by *activated families retained at week 2*. Report the cut, not the
total.

**Failure it prevents.** Celebrating growth that hides a leaky or valueless
product.

---

## CLV > CAC (the economic gate)

**Definition.** A channel/business is viable only if customer lifetime value
exceeds fully-loaded acquisition cost, with margin. (*Zero to One*.)

**When it applies.** Judging any channel test; any "scale this" request.

**When it does NOT.** Pre-revenue learning tests where the metric is
problem-validation, not economics — but flag that economics are still unproven.

**Decision cue.** Estimate CAC *during* the test, not after scaling. CLV ≤ CAC →
the channel is dead at any volume → do not scale (hub Guardrail; ties to the
*dead zone* in `growth-traction-channels`).

**Failure it prevents.** Scaling structurally unprofitable acquisition.

---

## Traction signal (what counts as a signal)

**Definition.** A test result strong enough — against the **pre-set** threshold
— to justify focusing or scaling, distinguished from noise or a vanity bump.

**Decision cue.** A result is a signal only if: threshold was set before
running, the metric is actionable (not vanity), economics clear CLV > CAC (for
channels), and the result is repeatable — not a single spike. Miss any → not a
signal; **refuse to label it one** and say which condition failed.

**Failure it prevents.** Scaling on noise, vanity, or a post-hoc bar — the most
expensive class of growth mistake.
