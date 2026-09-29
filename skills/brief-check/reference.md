# Brief Check: reference

Ported from quotabird.com/brief. Do not re-tune.

## The five questions, in order

| # | Pillar | Question | Weight |
|---|---|---|---|
| 1 | POINT | Can you say in one sentence what you want them to decide, and why now? | 24 |
| 2 | RECEIPTS | For the three claims the argument depends on, do you have evidence that isn't your own team's opinion? | 22 |
| 3 | ALTERNATIVE | Have you dealt with the most credible other option, including doing nothing? | 18 |
| 4 | HOLE | Do you know the weakest assumption in your own argument, and who in the room will find it? | 20 |
| 5 | ASK | Is it completely clear what you need from them today, and who owns the next step? | 16 |

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
| ≥ 75 | Room ready | Yes. It's room-ready. | Your argument is clear and the claims have receipts. | Lead with the hole. Say the weak spot before somebody else does. |
| 55 to 74 | A fight | Maybe. It'll be a fight. | Your recommendation may be sound. You've left an opening. | They will find it. Better you find it first. |
| 35 to 54 | Shark food | No. Shark food. | You're relying on assumptions, vague impact, or an unclear ask. | The room won't argue with you. It will just move on. |
| < 35 | No point | No. There's no point yet. | There isn't a decision in this brief yet. | Find the one sentence first. Everything else is formatting. |

## Before the meeting (fixes, weakest first, up to three)

- POINT: Write the one sentence: what to decide, and why now. Put it first.
- RECEIPTS: For the three load-bearing claims, write the source and its date. Cut what only your team believes.
- ALTERNATIVE: Write the alternative the room already prefers, in their words, and why it's not enough.
- HOLE: Name your weakest assumption in the brief before they do.
- ASK: End with what you need, from whom, by when, and who owns what next.

If everything was a yes: "Say your weakest assumption out loud in the first minute. Then the argument happens on your terms."

## Pressure Test: what the room will ask

Default questions by pillar (three each):

- POINT: You have twenty seconds. What's the point? / I read the whole thing. What exactly are you recommending? / If I remember one sentence tomorrow, what should it be?
- RECEIPTS: Where did that number come from? Actual, forecast, modeled, or anecdotal? / Give me one piece of evidence that didn't come from your own team. / Revenue went up. And? Adoption grew. And? Customers asked. And?
- ALTERNATIVE: Why shouldn't we just do nothing for six months? / What's the cheapest reasonable alternative, and why is it wrong? / What would someone who disagrees with you recommend instead?
- HOLE: What's the sentence in this brief you hope nobody challenges? / Which assumption, if false, takes the recommendation down with it? / Which number are you least confident in?
- ASK: Is this an FYI, a discussion, a recommendation, or a decision? / What exactly do you need from me before you leave this room? / Who owns the next action, and by when?

Who's across the table? Use their questions for the weakest pillar instead:

- **Finance.** POINT: What does this cost? / What's the return, and over what period? / What's the downside case? RECEIPTS: Which assumption drives most of the economics? / Is that number actual, forecast, or modeled? / What's the denominator? ALTERNATIVE: What does doing nothing cost us? / What's the cheapest version of this that gets 80% of the value? / Why is that not good enough? HOLE: Which number would you least like me to check? / What happens to the case if that number is half? / What did you leave out of the model? ASK: How much, when, and from whose budget? / What do you need me to approve today versus later? / What can you deliver with half of it?
- **The executive.** POINT: Why are you telling me this? / What's the decision? / Why now? RECEIPTS: Who else believes this besides your team? / Has a customer said this, or have we inferred it? / How recent is that? ALTERNATIVE: What's the alternative you're not recommending, and why? / Why not wait a quarter? / Who else has tried this? HOLE: What's the question you're hoping I don't ask? / What would make you wrong? / What's the thing you're least sure of? ASK: What are you asking me to do? / What happens if I say no? / Who owns this after today?
- **The tech leader.** POINT: What has to be true technically for this to work? / What's the one-line architecture? / What are you hand-waving? RECEIPTS: Has this been built, or is this a diagram? / What did the prototype actually show? / What's the failure mode you've seen so far? ALTERNATIVE: Why build instead of buy? / What's the boring option, and why not that? / What did the last team that tried this learn? HOLE: What's the hardest dependency? / What's the assumption about scale that nobody's tested? / What breaks first? ASK: How many people, for how long? / What do you need from my team? / What's the first milestone I can check?
- **The sales leader.** POINT: What does this do for the number? / Which deals does this move, by name? / Why this quarter? RECEIPTS: Has a customer actually said they want this? / Who pays, and who decides? / What's stopping the deal today? ALTERNATIVE: What do we lose if we sell what we've got? / What's the competitor doing instead? / Why not a partner? HOLE: Which deal is this really about, and what's its problem? / What's the customer objection you haven't answered? / What's the price? ASK: What do you need from sales? / When can I put it in a forecast? / Who carries the number?
- **The skeptic.** POINT: What's the real reason you want this? / What problem does this solve that we didn't have last year? / Whose idea was this, and what do they get? RECEIPTS: What evidence would change your mind? / What's the best argument against this? / Who disagrees, and why are they wrong? ALTERNATIVE: What did the alternative look like before you wrote it to lose? / Why is doing nothing not the answer? / What would you recommend if this were someone else's idea? HOLE: What's the sentence you hope nobody challenges? / What's the assumption you haven't been able to prove? / What are you not telling this room? ASK: What are you actually asking for? / What's the smallest commitment that tests this? / What will you show us in ninety days?

## Worked example

Point yes, Receipts sort of, Alternative no, Hole sort of, Ask yes. Mean = (92×24 + 50×22 + 8×18 + 50×20 + 92×16) ÷ 100 = 59.2 → 59; any-no cap 74 does not bind. Verdict: A fight, "Maybe. It'll be a fight." 3 of 5 proven. Weakest: ALTERNATIVE. First fix: write the alternative the room already prefers, in their words, and why it's not enough.
