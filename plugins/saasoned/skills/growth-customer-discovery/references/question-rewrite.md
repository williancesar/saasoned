# Question critique-and-rewrite procedure

A deterministic procedure to audit a set of customer-interview questions against
*The Mom Test* and return a corrected script. Use whenever the user supplies (or
asks you to write) interview/survey questions.

## Procedure

For each question, classify and act:

1. **Hypothetical/future** ("Would you…", "Do you think you'd…") → **rewrite**
   to past behavior ("When did you last…", "Walk me through the last time…").
2. **Opinion on the solution** ("Do you like this idea/feature?") → **rewrite**
   to a problem/behavior question, or **cut** if it only fishes for approval.
3. **Leading** (embeds the desired answer) → **rewrite** neutral, open.
4. **Generic** ("Do you usually struggle with X?") → **rewrite** to a specific
   instance ("Tell me about the last time X happened").
5. **Pricing-as-hypothetical** ("Would you pay $N?") → **rewrite** to current
   spend ("What do you use today for this, and what does it cost you —
   money/time/workarounds?").
6. **Already good** (asks for a specific past event/behavior) → **keep**.

Then append a **commitment step**: end the script with a request for a real
currency (time/reputation/money) and a defined next step (advancement).

## Output format

A table — `Original → Verdict → Rewrite (or Cut, with reason)` — followed by the
appended commitment ask. State explicitly which questions were the
hypothetical/leading ones (this is an acceptance criterion of the suite).

## Worked example (illustrative — not a product spec)

Input script for *family-agent*:

| Original | Verdict | Rewrite / Cut |
|---|---|---|
| "Would you use an app that coordinates your family?" | Hypothetical | "Tell me about the last time something fell through the cracks coordinating your family — what happened?" |
| "Do you like the idea of an AI family assistant?" | Solution opinion | Cut — fishes for a compliment; replace with the problem question above |
| "Don't you find shared calendars frustrating?" | Leading | "How do you currently keep the family's schedule in sync? When did that last break down?" |
| "Do you usually forget tasks?" | Generic | "What's the last thing that got dropped because no one owned it? Walk me through it." |
| "Would you pay $9/mo for this?" | Pricing-hypothetical | "What do you pay or do today to deal with this — apps, time, a planner, a person?" |
| "What did you do the last time plans changed last-minute?" | Good | Keep |

Appended commitment ask: *"Could we do a 30-minute session with your partner
this week where you show me how you currently coordinate?"* — secures **time**
currency + **advancement**; a yes is signal, "sounds great, keep me posted" is
not.

## Common failure it prevents

Running a polished interview script that manufactures agreement, then "building
the validated thing" on bad data.
