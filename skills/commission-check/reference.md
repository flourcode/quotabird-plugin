# Commission Check: reference

Ported from quotabird.com/commission. Do not re-tune.

## Math

```
credit   = deal × share of credit × product multiplier     (share and multiplier default to 100%)
gross    = credit × rate
set aside = gross × tax share                               (default 30%)
take-home = gross − set aside
```

## Result

- Verdict: "That's your take-home." Big number: the take-home.
- Sentence: (if split) "Your credit on this deal is [credit]. " + "Set aside [tax]% and you keep about [100 − tax] cents of every commission dollar on this deal."
- Next line: "A planning buffer, not tax advice. Change the percentage to yours."
- Rows: (if split) Deal size, Your credit on it; then Gross commission, Set aside about, Take-home about.

## Worked examples

$500K deal at 8%, no split: gross $40K, set aside $12K, take-home $28K. "Set aside 30% and you keep about 70 cents of every commission dollar on this deal."

$1M deal at 8% with 50% credit: credit $500K, gross $40K, take-home about $28K.

A split through a channel credited at half: $1M deal, 50% share, 50% multiplier: credit $250K, gross $20K, take-home about $14K.
