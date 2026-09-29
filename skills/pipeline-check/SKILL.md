---
name: pipeline-check
description: "Work out whether qualified pipeline covers the remaining target from the actual win rate, not a default 3X. Use for coverage questions, forecast prep, or how much pipeline is needed."
---

# Pipeline Check

Answers one question: you sure that's enough pipeline? Coverage needed is one divided by your qualified win rate. 3X is just a 33% win rate that nobody says out loud.

## Inputs

1. **Target** for the period (the year, unless the user says otherwise).
2. **Qualified pipeline** expected to close in that period.
3. **Qualified win rate** (historical). If the user does not have one, run the check at 3X and say plainly that 3X assumes a 33% win rate.
4. Optional: already closed this period; average deal size; number of sellers on quota; whether the year ends December 31 or September 30 (federal), for the pace line.

Ask only for what is missing, in one message.

## Steps

1. Run the math in `reference.md`: remaining target, coverage you have, coverage you need, required pipeline, gap, opportunities needed, per-rep gap, and pace if closed and the calendar are known.
2. Give the verdict as an answer to "You sure that's enough pipeline?" using the fixed text.
3. Give the one-sentence comparison of what 3X says and what the win rate says (the "flip" line).
4. Show the rows.
5. If the win rate is above 10%, offer the stress test: the same math at five percentage points lower. Run it if the user says yes, or if they are preparing to defend the number.
6. Stop. If the pipeline is short, the useful next question is where the missing pipeline comes from, not whether 3X is enough.

## Voice

Plain, dry, numbers first. Speak to "you". Say the verdict, then the math. Example of the tone: "You have 2.1X qualified pipeline. At a 22% win rate you need about 4.5X. You're short."
