# Offer Check: reference

Ported from quotabird.com/offer. Do not re-tune.

## Math

```
at = realistic attainment (0.85 if not given)
r  = min(12, ramp months)
year one   = base + variable ÷ 12 × ( r × (guarantee if given, else at × 0.5) + (12 − r) × at )
normal year = base + variable × at
diff  = normal B − normal A
d1    = year one B − year one A
rel   = |diff| ÷ max(normal A, normal B)
```

During ramp the offer earns the guarantee if there is one, otherwise half the normal attainment. That half is an assumption; say so when it matters.

## Verdicts

| Condition | Verdict (say first) | Next line |
|---|---|---|
| rel < 3% | About the same money. | Close enough that the rest of the job should decide it: the territory, the manager, and how many people actually hit quota. |
| B ahead | Offer B pays more in a normal year. | That assumes the same attainment at both jobs. If one quota is much harder, lower its attainment and run it again. |
| A ahead | Offer A pays more in a normal year. | (same next line) |

Sentence: "At [at]% attainment, Offer [X] pays [|diff|] more in a normal year." (When close: "...the two offers are within [|diff|] of each other in a normal year.") If d1 has the opposite sign and |d1| > $1K, add: "Offer [Y] pays [|d1|] more in year one, because of its ramp or guarantee."

## Rows

Offer A at 100% (OTE), Offer B at 100% (OTE), Offer A year one, Offer B year one, Offer A normal year at [at]%, Offer B normal year at [at]%.

## Worked examples

A: base $150K, variable $130K, 6-month ramp. B: base $170K, variable $150K, 6-month ramp. 85% attainment.
Normal: A $260.5K, B $297.5K, diff $37K. Year one: A $232.9K, B $265.6K.
Verdict: "Offer B pays more in a normal year. At 85% attainment, Offer B pays $37K more in a normal year."

Same, but A has a 100% guarantee during its ramp and B is $160K base, $140K variable:
Year one A $270.2K, B $249.2K; normal A $260.5K, B $279K.
"Offer B pays more in a normal year. At 85% attainment, Offer B pays $19K more in a normal year. Offer A pays $21K more in year one, because of its ramp or guarantee."
