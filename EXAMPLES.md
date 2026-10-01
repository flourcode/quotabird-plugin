# Examples

Three end-to-end runs, the way they should read. Use them to demo the plugin or to check a build.

## 1. Quota dispute

**User:** Last year we did $8.2M. We're running at $8.7M annualized. I've got $6M of new qualified pipeline, my win rate is 25%, and the new quota is $12M. It's a cloud consumption number. Is it possible?

**Claude (quota-case):**

You've got a gap. $1.8M of your number that nobody has explained yet.

- Last year: $8.2M
- Run rate (MRR × 12): $8.7M
- Plus new pipeline at your 25% win rate: $1.5M
- What the evidence supports: $10.2M
- The new number: $12M
- Growth over last year: +46%
- Gap nobody has explained: $1.8M
- New pipeline to close it, at 25%: $7.2M

To push back: "Here's last year, here's what we're running at, and here's a $1.8M gap I can't explain. What assumption am I missing?"

To close it: about $7.2M of new pipeline at your win rate, from growth in existing accounts and net-new ones.

The growth rate almost never moves. What can move: the baseline, the territory, ramp time, crediting. Pick one ask.

## 2. Federal deal

**User:** $900K opportunity with an Army program office. They told us they want to fix this. Money: our contact says it's "in the budget" but nobody's named the line. We're talking to the program manager. We haven't figured out the vehicle. There's an end-of-life on the current system next spring.

**Claude (deal-check):**

Reading that as: customer yes, money sort of, power yes, path no, now yes.

Hopium. 3½ of 5 proven. Weakest: path. Nobody has said how this actually gets bought. You believe it. You haven't proved it.

- Path: Ask which contracting office and vehicle they would use.
- Money: Get one person at the customer to name the funding line this week.

Want the pressure test? Your manager will ask three questions about the path. Say yes and I'll put them to you one at a time.

**User:** Yes.

**Claude:** How would they award this, and through which contracting office?

**User:** Probably through their usual office. I'm not sure which vehicle.

**Claude:** That's a miss. Next: what vehicle would it go through, and are you on it?

(and so on; after three)

You wouldn't survive. You couldn't answer 2 of 3 from your manager. The one you can't bluff is path.

Before the forecast call: ask which contracting office and vehicle they would use.

## 3. Pipeline

**User:** Target is $4M, I've closed $1M, I've got $7M of qualified pipeline and my qualified win rate is 25%. Is that enough?

**Claude (pipeline-check):**

Not really. You're at risk.

3X says $2M short. Your 25% win rate says $5M.

- Remaining target: $3M
- You have: 2.3X
- 3X says you need: $9M ($2M short)
- Your 25% win rate says you need: $12M ($5M short)

Half the pipeline you need isn't there. Where does it come from?

If your win rate is really 20%, the gap is $8M. Coverage only counts if the deals are real, so check a few before you commit any of it.

## Comp plan (Pay Check)

Inputs: base $150K, variable $130K, 1.5x the normal rate above 100% of quota, no cap, no threshold.
Rows: 50% $215K, 75% $248K, 100% $280K, 125% $329K, 150% $378K, 200% $475K.
Verdict: "+$98K. Yes, it pays for beating the number. At 150% of quota you'd make $378K, $98K more than at 100%." About half of AEs hit quota (Bridge Group, 2026), so budget on the 75% and 100% rows.
With variable capped at 120% of target: everything from 125% up is $306K, and the verdict becomes "Not much above 100%."

## Pipeline from an export, with the slip test

Inputs: a pasted export with amount, stage, close date and probability columns; target $4M, 25% win rate, year ends September 30. Proposal and Negotiation count as qualified.
Count: Acme $1.5M (Proposal) and Gamma $1.2M (Negotiation) are qualified pipeline, $2.7M. Beta (Discovery) is early; Delta closes after the year end. Echo ($600K closed won) is already closed. The probability column is not used.
Math: remaining $3.4M; at 25% you need 4X, $13.6M; you have 0.8X; $10.9M short. Verdict: "No. You're short."
Slip test: without Acme, $1.2M of pipeline, 0.35X, $12.4M short.
