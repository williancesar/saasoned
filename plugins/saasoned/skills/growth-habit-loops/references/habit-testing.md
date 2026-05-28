# Habit-testing — Eyal

**Source.** Nir Eyal, *Hooked*. The empirical loop for finding, understanding,
and strengthening a habit once a product is live. This skill owns the *habit*
side; the general experiment/metric machinery lives in `growth-experiments` —
cross-reference, don't duplicate.

**Definition.** A three-step cycle:

1. **Identify.** Define what a habitual user looks like (a concrete
   behavior + cadence), then measure how many users actually meet it. Be honest
   about the bar; "active user" ≠ "habitual user."
2. **Codify.** Examine the habitual users' early behavior to find the
   **Habit Path** — the sequence of actions that the people who *did* form the
   habit took (and others didn't). This is a hypothesis about what creates the
   habit.
3. **Modify.** Change the product to guide new users down that Habit Path, then
   re-measure. Iterate.

**When it applies.** A live product with enough users to segment habituals;
"some users love it, most drift" — find what the lovers did and route others
through it.

**When it does NOT.** Pre-launch / too few users to find a habitual cohort —
you can't codify a path that doesn't exist yet (do `growth-customer-discovery`
and design the Hook first). Also not for choosing the headline metric — that's
`growth-experiments`.

**Decision cue.**

```
Enough users to find a habitual cohort?
├─ No  → too early; design the Hook + discovery first
└─ Yes → Identify (define + count habituals)
          → Codify (what did habituals do early that others didn't?)
          → Modify (steer new users down that path) → re-measure
```

Pair every Modify step with a kill/keep condition and a non-vanity metric
(see `growth-experiments`): the metric must be *value-backed habitual behavior*,
not raw sessions or time-in-app.

**Worked micro-example.** *vai-nascer-v2*: define habitual = logs a symptom in
≥3 of 4 weeks. Measure: small fraction qualifies. Codify: habituals
overwhelmingly added a family member in week 1; non-habituals didn't. Modify:
move the family-invite prompt into first-run onboarding; re-measure the habitual
rate. (Note the family-invite path also feeds `growth-network-effects`.)

**Common failure it prevents.** "Optimizing engagement" by guessing, instead of
finding the actual path your already-habitual users took and routing newcomers
through it — and doing so against a value-backed metric, not a vanity one.
