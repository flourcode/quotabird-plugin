# Quota Case: reference

Ported from quotabird.com/quota-case. Do not re-tune.

## Inputs

| Input | Used for |
|---|---|
| basis | bookings, or run rate / whole book |
| lastyear | last year's number on the same measure |
| oneoff | one-time deals inside last year (optional) |
| runrate | current run rate, MRR × 12 (run rate and whole book only) |
| pipeline | new qualified pipeline this year |
| win | historical win rate |
| repsthen, repsnow | reps last year, fully ramped reps now (optional) |
| quota | the new number |

Required: quota > 0 and lastyear > 0. Everything else improves the evidence.

## Model

```
last = lastyear − oneoff
cap  = repsnow ÷ repsthen        (only if both given; otherwise 1)
pipe = pipeline × win            (only if both given; otherwise 0)
hist = last × cap

Bookings:
  evidence = max(hist, pipe)     (run rate is ignored)

Run rate or whole book:
  base = runrate if given, else hist
  evidence = base + pipe         (run rate is never multiplied by cap)

gap    = quota − evidence
share  = gap ÷ quota
growth = (quota − last) ÷ last
need   = gap ÷ win               (only if gap > 0 and win given)
```

Headcount rule: on a bookings number, headcount scales last year's bookings (capacity). On a run-rate number, the run rate already reflects today's team, so headcount is shown as context only.

## Verdicts

| Condition | Verdict (say first) | Sentence | Next line |
|---|---|---|---|
| gap ≤ 0 | Yes. It already adds up. | The evidence supports [quota]. Hard, maybe, but defensible. | Stop arguing about it with the team and build the plan. |
| share ≤ 10% | You're a little short. | [gap] short of what the evidence supports. That's a stretch, not a scandal. | Find the [gap] with names attached, then build the plan. |
| share ≤ 25% | You've got a gap. | [gap] of your number that nobody has explained yet. | Push back with the gap below, or close it with growth in existing accounts and net-new ones. |
| share > 25% | You've got a big gap. | [gap], [share]% of the number, with nothing in the evidence to fill it. | Take the gap to your boss before you sign anything. |

## Rows, in order

1. Last year
2. Without one-time deals (if given)
3. Bookings: "Last year at today's headcount" (if headcount given). Run rate / whole book: "Run rate (MRR × 12)", or "Last year at today's headcount" / "Last year, as your baseline" when no run rate was given
4. "Pipeline at your N% win rate" (bookings) or "Plus new pipeline at your N% win rate" (run rate)
5. "Ramped reps, now vs last year" (run rate, when both given)
6. What the evidence supports
7. The new number
8. Growth over last year (flag it when over +25%)
9. Gap nobody has explained (or "None")
10. New pipeline to close it, at N% (when there is a gap and a win rate)

## The two scripts (only when there is a gap)

- **To push back:** "Here's last year, here's what we're running at [bookings: here's what the pipeline supports at our win rate], and here's a [gap] gap I can't explain. What assumption am I missing?"
- **To close it:** about [need] of new pipeline at your win rate, from growth in existing accounts and net-new ones.

When there is no gap: "The number holds up against the evidence. Now it's about the plan."

## What can move, and what usually can't

The growth rate on a cloud-provider number is usually set above the geo VP and rarely moves. What can move: the baseline (take out revenue that won't repeat), territory changes after the number was set, ramp time, and crediting. One ask gets heard.

## Worked example (run rate)

Last year $8.2M, no one-offs, run rate $8.7M, new pipeline $6M, win rate 25%, quota $12M.
pipe = $1.5M. evidence = 8.7 + 1.5 = $10.2M. gap = $1.8M, share 15%, growth +46%, need = 1.8 ÷ 0.25 = $7.2M.
Verdict: "You've got a gap. $1.8M of your number that nobody has explained yet."

## Worked example (bookings)

Last year $1M, 10 reps then and 8 ramped now, pipeline $4M at 25%, quota $1.2M.
hist = 1.0 × 0.8 = $800K. pipe = $1M. evidence = $1M. gap = $200K, share 17%. need = $800K.
Verdict: "You've got a gap."
