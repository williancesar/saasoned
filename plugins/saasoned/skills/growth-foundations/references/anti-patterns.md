# Cross-cutting anti-patterns

The suite-wide mistakes these frameworks exist to prevent. Each sibling adds a
narrower catalog for its own domain; this file holds only the failures that span
the whole suite. Format per entry:
**Symptom → Why it fails (source) → The rule that replaces it → Routed fix.**

---

### 1. Building before distribution is designed

- **Symptom.** Roadmap is all product; no named channel; "we'll market it when
  it's ready"; no answer to "who are the first 100 users and how do they
  arrive?"
- **Why it fails.** A great product with no distribution channel is a bad
  business (*Zero to One*). No audience is waiting (*The Embedded
  Entrepreneur*).
- **Rule.** Distribution + positioning are designed with the product, 50/50.
- **Routed fix.** `growth-positioning`, then `growth-traction-channels`.

### 2. Scaling before a traction signal / before an atomic network

- **Symptom.** Increasing ad spend, hiring sales, or PR push with no proven
  channel; launching a marketplace city-wide with an empty supply side.
- **Why it fails.** Spending to scale before the success signal exists is
  premature scaling (*Traction*); a network with no atomic network has nothing
  to scale (*The Cold Start Problem*).
- **Rule.** Earn a signal on a cheap test (or saturate one atomic network)
  *first*. This is a hard Guardrail — refuse and cite.
- **Routed fix.** `growth-experiments` (define the signal/kill condition);
  `growth-network-effects` (seed the atomic network).

### 3. Channel diversification too early

- **Symptom.** Running six channels at 10% effort each "to see what sticks";
  dashboards everywhere; nothing decisively working.
- **Why it fails.** The distribution power law: typically one channel dominates;
  spreading guarantees none gets a real test (*Zero to One*; *Traction*
  Bullseye).
- **Rule.** Test inner-ring options cheaply, then focus the ONE with signal;
  add channels only when the first is saturated.
- **Routed fix.** `growth-traction-channels`.

### 4. Vanity metrics as a success signal

- **Symptom.** "Numbers are up" = total signups, pageviews, app installs,
  registered users — with no retention/value cut and no decision attached.
- **Why it fails.** Numbers that rise without proving delivered value can't
  justify a bet and hide a leaky product.
- **Rule.** Commit to a North Star / one-metric-that-matters tied to value;
  judge channels by CLV > CAC, not raw volume.
- **Routed fix.** `growth-experiments`.

### 5. Broad-market positioning before niche domination

- **Symptom.** "It's for everyone"; the pitch lists many segments; messaging is
  generic to avoid excluding anyone.
- **Why it fails.** You stall in the chasm and beat no competitor decisively;
  monopoly comes from owning a small market first (*Crossing the Chasm*;
  *Zero to One*).
- **Rule.** Pick one beachhead, dominate, expand niche-by-niche.
- **Routed fix.** `growth-positioning`.

### 6. Customer interviews contaminated into pitches

- **Symptom.** Interview transcripts full of "would you use…?", "do you like
  this idea?", compliments treated as validation, the founder talking more than
  the user.
- **Why it fails.** Opinions, hypotheticals, and compliments are bad data; you
  learn nothing about real past behavior (*The Mom Test*).
- **Rule.** Ask about their life and specific past actions; seek commitment/
  advancement, not praise.
- **Routed fix.** `growth-customer-discovery`.

### 7. Manufacturing a habit without an ethics gate

- **Symptom.** Engagement loop designed purely to maximize time-in-app;
  retention up, user benefit unexamined.
- **Why it fails.** A complete Hook can drive behavior the user doesn't benefit
  from; ungated, it is manipulation (*Hooked*, Manipulation Matrix).
- **Rule.** Run any habit loop through the Manipulation Matrix before
  recommending it; require genuine user benefit.
- **Routed fix.** `growth-habit-loops`.

---

**Use.** When a request matches a symptom, name the anti-pattern, cite the
source, state the rule, and route to the fix. For anti-patterns 1, 2, and 5 the
hub Guardrails require an explicit refusal of the scaling/broadening ask before
offering the routed fix.
