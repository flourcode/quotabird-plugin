# Pay Check: reference

Ported from quotabird.com/pay. Do not re-tune.

## Math

```
acc   = accelerator rate (1.5 for 150%); 1 if none
start = where it starts (1.0 for 100%); 1 if not given
cap   = cap on variable as a multiple of target (2.0 for 200%); none if not given
th    = threshold (0.5 for 50%); 0 if not given

pay(a) = 0                                                         if a < th
       = min( variable × min(a, start) + variable × (a − start) × acc if a > start,
              variable × cap )                                      otherwise

total pay at attainment a = base + pay(a)
extra    = pay(1.5) − pay(1.0)
straight = variable × 0.5          (what a straight-line plan adds from 100% to 150%)
ratio    = extra ÷ straight
```

Show money as $K below $1M and $X.XXM at $1M and above (trailing zeros dropped).

## Verdicts (checked in this order)

| Condition | Verdict (say first) | Next line |
|---|---|---|
| cap below 150% and ratio < 0.3 | The cap takes the upside. | The cap stops your variable at [cap]% of target. Ask whether it's ever been lifted for a big year. |
| ratio < 0.95 | Not much above 100%. | A cap or a late start takes most of the upside. Know that before you count on a big year. |
| ratio ≥ 1.2 | Yes, it pays for beating the number. | Plan your budget on the 75% and 100% rows. The rows above them are the good years. |
| ratio ≥ 1.02 | A little extra above 100%. | The accelerator starts late or pays a small premium. Plan on the 75% and 100% rows. |
| otherwise | It pays in a straight line. | Fair, with no extra reward for beating the number. Plan on the 75% and 100% rows. |

Sentence: "At 150% of quota you'd make [base + pay(1.5)], [extra] more than at 100%."
Big number: "+[extra]".

## Rows

At 50%, 75%, 100%, 125%, 150% and 200% of quota: total pay. If there is a threshold, add "Nothing pays below [th]%" and mark the rows under it.

## Worked example

Base $150,000, variable $130,000, accelerator 150% from 100%, no cap, no threshold.
pay(1.5) = 130 + 130 × 0.5 × 1.5 = $227.5K. At 150%: $377.5K, shown $378K. extra $97.5K, shown +$98K. ratio 1.5.
Verdict: "Yes, it pays for beating the number. At 150% of quota you'd make $378K, $98K more than at 100%."
Rows: 50% $215K, 75% $248K, 100% $280K, 125% $329K, 150% $378K, 200% $475K.

Capped at 120%: everything from 125% up is $306K. extra $26K, ratio 0.4: "Not much above 100%."
