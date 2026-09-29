# Pipeline Check: reference

Ported from quotabird.com/pipeline. Do not re-tune.

## Math

```
closed    = min(closed, target)                (0 if not given)
remaining = target − closed                    (if ≤ 0: the number is done; say so and stop)
coverage  = pipeline ÷ remaining               ("you have")
covNeed   = 1 ÷ win                            (3 if no win rate; if within 0.05 of 3, treat as exactly 3)
need      = remaining × covNeed
gap       = max(0, need − pipeline)
ratio     = pipeline ÷ need
req3      = remaining × 3
gap3      = max(0, req3 − pipeline)
deals     = ceil(gap ÷ deal size)              (if deal size given and gap > 0)
perRep    = gap ÷ reps                          (if reps given and gap > 0)
```

Pace (only if closed and the year end are known): monthsIn is how far into the period today is; monthsLeft = 12 − monthsIn. runNow = closed ÷ monthsIn; runNeed = remaining ÷ monthsLeft; pace = runNeed ÷ runNow. Say what the monthly rate has to rise to. Calendar year runs January 1 to December 31; a federal year runs October 1 to September 30.

## Verdicts

| ratio | Verdict (say first) | Next line |
|---|---|---|
| ≥ 1.0 | Yes. You're covered. | Coverage only counts if the deals are real. Check a few before you commit it. |
| 0.75 to 0.99 | Close. Not quite. | Close. A couple of real deals would get you there. |
| 0.50 to 0.74 | Not really. You're at risk. | Half the pipeline you need isn't there. Where does it come from? |
| < 0.50 | No. You're short. | Don't forecast this yet. You don't have enough pipeline to close your way out of it. |

## The 3X line (pick the one that fits)

- No win rate given, covered at 3X: "Covered at 3X. Add your win rate to find out if 3X is your number."
- No win rate given, short at 3X: "At 3X you're [gap3] short. Add your win rate to see the real number."
- Win rate is about 33%: "Your [win]% win rate is the 3X assumption. [Covered. / [gap] short.]"
- 3X says covered but the win rate says short: "3X says you're covered. Your [win]% win rate says you're [gap] short."
- 3X says short but the win rate says covered: "3X says you're [gap3] short. Your [win]% win rate says you're covered."
- Both short: "3X says [gap3] short. Your [win]% win rate says [gap]."
- Both covered: "Covered either way: at 3X and at your [win]% win rate."

## Rows

You have [coverage]X. 3X says you need [req3] ([covered] / [gap3] short). Your [win]% win rate says you need [need] ([covered] / [gap] short). If deal size: about [deals] more qualified deals. If reps: [perRep] per seller, and deals per seller if deal size is also known.

## Stress test

Offered when the win rate is above 10%: "Before you defend it, try to break it." Rerun the math at (win − 5 points) and show the new coverage needed and gap. Say what it means in one line.

## Source labeling

- Coverage needed = 1 ÷ win rate is arithmetic. No source needed.
- 3X is a common rule of thumb. It is a 33% win rate stated another way, not a benchmark.
- Any win-rate figure the user does not supply is unknown. Do not assume one.

## Worked example

Target $4M, closed $1M, pipeline $7M, win rate 25%. remaining $3M. coverage 2.33X. covNeed 4X. need $12M. gap $5M. ratio 0.58. Verdict: "Not really. You're at risk." The 3X line: "3X says you're covered. Your 25% win rate says you're $5M short." Stress test at 20%: need $15M, gap $8M.
