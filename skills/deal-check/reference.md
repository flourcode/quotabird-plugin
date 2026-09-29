# Deal Check: reference

Ported from quotabird.com/deal. Federal-specific. Do not re-tune.

## The five questions, in order

| # | Pillar | Question | Weight |
|---|---|---|---|
| 1 | CUSTOMER | Has the customer actually said they want to solve this? | 20 |
| 2 | MONEY | Do you know where the money comes from? | 26 |
| 3 | POWER | Are you talking to someone who can make this happen? | 22 |
| 4 | PATH | Do you know how they will buy it? | 16 |
| 5 | NOW | Is there a real reason this happens now? | 16 |

Answer values: yes = 92, sort of = 50, no = 8.

## Scoring

```
total = round( Σ (value × weight) ÷ Σ weight )       (Σ weight = 100)
if MONEY = no:     total = min(total, 55)   "you can't say where the money comes from"
if POWER = no:     total = min(total, 60)   "you haven't reached anyone who can act"
if CUSTOMER = no:  total = min(total, 45)   "the customer hasn't confirmed they intend to act"
if any answer = no: total = min(total, 74)  (a single no keeps a deal out of Healthy)
```

Proven count: yes = 1, sort of = ½, no = 0, out of 5. Weakest pillar: the lowest answer; ties go to MONEY first, then the heavier weight.

## Verdicts

| total | Label | Say first | Next line |
|---|---|---|---|
| ≥ 75 | HEALTHY | It's real. | It survived. Bring the proof. |
| 55 to 74 | HOPIUM | Hopium. | You believe it. You haven't proved it. |
| 35 to 54 | AT RISK | Real, but at risk. | Something important is still a guess. Keep it out of commit for now. |
| < 35 | NOT A DEAL YET | Not a deal yet. | You've got a conversation. Not a deal yet. |

Meta line: "[proven] of 5 proven. Weakest: [pillar]."

## Attack line (by weakest pillar; Healthy uses the last one)

- CUSTOMER: You're the only person in the room who thinks this is a requirement.
- MONEY: Your boss is going to come after the money.
- POWER (pick one): You're best friends with someone who can't spend a single dollar. / Your champion likes you. They can't sign. / Your contact can say no, but they have zero power to say yes. / A technical evaluator can love you and still not move a dime. / The people who like you aren't the people who can spend.
- PATH: Nobody has said how this actually gets bought.
- NOW: Nothing is forcing them to act, so nothing will.
- HEALTHY: Nothing obvious to attack. Bring the proof anyway.

## Moves (for pillars that were not a yes, weakest first, up to three)

- CUSTOMER: Get the customer to say the problem out loud, in their words.
- MONEY: Get one person at the customer to name the funding line this week.
- POWER: Get one meeting above your current contact.
- PATH: Ask which contracting office and vehicle they would use.
- NOW: Find the deadline: expiring contract, end of life, mandate, or budget year.

## Pressure Test: the three questions a manager asks about the weakest pillar

- CUSTOMER: What has the customer actually done that proves they intend to buy? / Who said they want this, and what exactly did they say? / What happens to them if they do nothing?
- MONEY: Who exactly has told you the money is available? / What budget does it come out of? / What happens to your date if the funding slips a quarter?
- POWER: Who have you met who can move this forward? / Who signs, and have you ever been in a room with them? / Who inside is telling you things you didn't have to ask for?
- PATH: How would they award this, and through which contracting office? / What vehicle would it go through, and are you on it? / Who else can they buy this from more easily than you?
- NOW: What is forcing them to act this year instead of next? / What is the next dated step in their process? / Who owns that date on their side?

## Worked example

Customer yes, Money sort of, Power yes, Path no, Now yes. Mean = (92×20 + 50×26 + 92×22 + 8×16 + 92×16) ÷ 100 = 67.6 → 68. The any-no cap (74) does not bind, so total 68. Verdict: HOPIUM, "Hopium." 3½ of 5 proven. Weakest: PATH. Attack: "Nobody has said how this actually gets bought." First move: ask which contracting office and vehicle they would use.
