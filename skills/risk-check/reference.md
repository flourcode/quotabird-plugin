# Risk Check: reference

Ported from quotabird.com/risk. Do not re-tune.

## The five questions, in order

| # | Pillar | Question | Weight |
|---|---|---|---|
| 1 | SPREAD | Would you still make the number if your biggest deal slipped a quarter? | 24 |
| 2 | MOTION | Has every deal in commit moved stage in the last sixty days? | 20 |
| 3 | NEXT | Does every commit deal have a customer action on the calendar, not just yours? | 22 |
| 4 | TIMING | Is at least half of it due before the last month of the period? | 16 |
| 5 | FRESH | Did you create at least a quarter of it this quarter? | 18 |

Answer values: yes = 92, sort of = 50, no = 8.

## Scoring

```
total = round( Σ (value × weight) ÷ Σ weight )     (Σ weight = 100)
if any answer = no: total = min(total, 74)
```

Proven count: yes = 1, sort of = ½, no = 0, out of 5. Weakest pillar: the lowest answer; ties go to the heavier weight.

## Verdicts

| total | Label | Say first | Sentence | Next line |
|---|---|---|---|---|
| ≥ 75 | Sturdy | No. It's spread out. | Spread out, moving, customers on the calendar. | Now check the coverage number too. A well-spread pipeline can still be too small. |
| 55 to 74 | Lopsided | Almost. It's lopsided. | One weakness, and it's the one the review will find. | Fix the weakest answer before someone asks about it. |
| 35 to 54 | Fragile | Yes. It's fragile. | A slip or a quiet customer takes you off the number. | Re-underwrite every commit deal this week. Whose calendar is the next step on? |
| < 35 | Won't hold | Yes. It won't hold. | It looks like coverage, but it's mostly hope. | Rebuild it from the customers up, starting with the deals that haven't moved. |

## Moves (for pillars that were not a yes, weakest first, up to three)

- SPREAD: Write the number without your biggest deal. That's the plan you're actually running.
- MOTION: Move every deal that hasn't changed stage in sixty days back a stage, today. Then work the ones that argue.
- NEXT: For each commit deal, get one customer action onto their calendar this week or move it out of commit.
- TIMING: Pull one deal into an earlier month, or accept that the year is a December bet and tell your manager so.
- FRESH: Block two mornings this week for creation. Nothing else fixes a crater.

If everything was a yes: "Keep the shape. Now check the size: run the coverage math with your real win rate."

## What the review will ask (weakest pillar)

- SPREAD: What happens to the number if the big one slips a quarter?
- MOTION: Which commit deals haven't changed stage since last quarter?
- NEXT: Which commit deals have a customer action on the customer's calendar?
- TIMING: How much of the number lands in the last month?
- FRESH: How much of this did you create this quarter?

## Federal wrinkle

On a federal year, a September close has nowhere to slip. Say so only when the user sells to government.

## Worked example

Spread no, Motion sort of, Next yes, Timing sort of, Fresh yes. Mean = (8×24 + 50×20 + 92×22 + 50×16 + 92×18) ÷ 100 = 56.7 → 57; any-no cap 74 doesn't bind. Verdict: Lopsided, "Almost. It's lopsided." 3 of 5 proven. Weakest: SPREAD. First move: write the number without your biggest deal.
