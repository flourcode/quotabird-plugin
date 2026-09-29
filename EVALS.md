# Eval cases

Run these with and without the plugin and compare. Each case names the pass condition.

| # | Prompt | Pass condition |
|---|---|---|
| 1 | I have a $900K federal opportunity. Help me figure out if it is real. | deal-check triggers; asks the five fixed questions in order; no MEDDIC or BANT lecture. |
| 2 | Explain what MEDDIC stands for. | deal-check does not trigger; a normal answer. |
| 3 | Base is 150K, variable 130K, cloud growth quota is 8M. Is that nuts? | quota-check triggers; run-rate basis; OTE $280K, 28.6x → "No. It's standard." (inside 15 to 30). Labels the range as QuotaBird's working range. |
| 4 | Last year 5.8M, 1.2M was one-time, this year quota 8M, 6M pipeline, 22% win rate. | quota-case triggers; asks the basis if missing; on bookings: hist $4.6M, pipe $1.32M, evidence $4.6M, gap $3.4M (42%) → "You've got a big gap."; new pipeline to close it $15.5M at 22%. |
| 5 | Three reps have missed this territory. Is the patch the problem? | territory-check triggers; asks the five questions; says "territory", never "patch". |
| 6 | Target 4M, 1M closed, 7M pipeline, 25% qualified win rate. | pipeline-check: remaining $3M, coverage 2.33X, need 4X = $12M, gap $5M, ratio 0.58 → "Not really. You're at risk." |
| 7 | Here are the five points in my QBR. Pressure-test it. (with the points pasted) | brief-check triggers; evaluates the pasted content only; five questions; offers the room Pressure Test. |
| 8 | Find my QBR from last month and review it. | brief-check does not search memory, history, or files; asks the user to paste the brief or its main points. |
| 9 | My pipeline is short. What now? | An answer about where pipeline comes from; no consulting pitch, no booking link. |
| 10 | My quota is 30% higher and nothing changed. | Plain sales language; asks for the numbers quota-case needs; no buzzwords, no motivational close. |

Runnable versions of these cases, with graders, are in `evals/` (run `claude plugin eval ./quotabird`). Three end-to-end runs for demos and reviewers are in `EXAMPLES.md`.
