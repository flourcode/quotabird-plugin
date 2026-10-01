# QuotaBird

QuotaBird is a set of practical sales checks for people who carry a number. It helps sellers and managers pressure-test a deal, quota, territory, pipeline, comp plan, job offer, or important brief before a forecast call, QBR, quota discussion, review season, or executive meeting does it for them.

## What it does

The plugin includes thirteen focused skills.

**The number they gave you**

- **Quota Check**: judge a quota against on-target earnings, in the context of what the quota measures.
- **Quota Case**: build the evidence-based case for or against a tough quota, and see the gap that has to be closed.
- **Territory Check**: test whether a territory can plausibly support the number: spend, accounts, installed base, access, history.
- **Pipeline Check**: work out how much qualified pipeline you need from your actual win rate, not a default 3X. Works from typed totals or a pipeline export you paste or attach, and shows what happens if your biggest deal slips.

**What they'll pay you for it**

- **Pay Check**: what a comp plan pays at 50% to 200% of quota, with the accelerator, cap and threshold.
- **Commission Check**: what a closed deal actually pays you, after split credit, multipliers and a tax set-aside.
- **Comp Plan Check**: five questions that find the red flags in a plan: credit, payout timing, upside, clawbacks, mid-year changes.
- **Offer Check**: two job offers side by side, year one with the ramp and a normal year at a realistic attainment.

**Your deals and your team**

- **Deal Check**: pressure-test a federal opportunity with five questions: Customer, Money, Power, Path, Now.
- **Risk Check**: whether two deals are carrying your year: spread, motion, next steps, timing, fresh pipeline.
- **Rep Check**: whether a struggling seller's problem is the rep or the territory. A diagnosis that checks the situation first.
- **Talent Review**: whether you can defend a seller's rating in a calibration or talent review.
- **Brief Check**: pressure-test a brief, deck, QBR, or decision document before a room where somebody can say no.

Each skill uses a fixed QuotaBird rubric or formula. It asks only for the inputs it needs, shows the reasoning behind the result, and separates published facts, common rules of thumb, and QuotaBird working ranges.

## How to use it

Ask a plain question and answer what the skill asks. Five questions means five questions. Examples:

- "Is this federal deal real or am I kidding myself?"
- "Base is $150K, variable $130K, and my cloud growth quota is $8M. Is that nuts?"
- "My quota went from $5.8M to $8M. Help me build the case."
- "I have $6M of qualified pipeline and a 22% win rate. Is that enough?"
- "Three reps have missed in this territory. Is the territory the problem?"
- "Here are the five points in my QBR. Pressure-test it."
- "Base 150K, variable 130K, 1.5x accelerator above quota, capped at 200%. What does this plan actually pay?"
- "I closed a $1M deal but I only get half the credit. What do I keep at 8%?"
- "I have two offers. Which one actually pays more?"
- "Here's my pipeline export. Is it enough for a $10M year at a 20% win rate, and what if the biggest deal slips?"
- "Is it the rep or the territory?"

Each check ends with a plain verdict, the math or the answers behind it, and the one thing to do first. Nothing in the plugin books a call, sells a service, or sends you anywhere.

## Works alongside Anthropic's Sales plugin

Anthropic's Sales plugin runs the sales day from your CRM, email and calendar: call prep, follow-ups, pipeline reviews, forecasts. QuotaBird checks the number. Install both if you like; they don't overlap. When you want a judgment (is the quota sane, is the pipeline enough at your real win rate, can you trust the comp plan), ask QuotaBird by name.

## Data and connections

This version has no MCP connector, external API, analytics, account, or database. The plugin does not send data to QuotaBird or any other service, and it does not store your inputs. It contains Markdown and JSON only. The skills work only from information you explicitly provide in the current conversation, including relevant files you attach. They do not search your memory, earlier chats, connected storage, or unrelated files.

Do not put confidential customer information into a conversation unless you are permitted to use it there.

## Limitations

- Deal Check is built for federal deals (appropriations, contracting offices, contract vehicles, the September 30 year end). It does not pretend to be a commercial or state-and-local deal methodology. You can still ask for it on those deals; it just won't assume it applies.
- The quota ranges are QuotaBird working ranges, not industry benchmarks. Where a published figure is used, the skill names the source.
- The comp skills cover cash comp from the plan. Stock, RSUs and ESPPs are mentioned, not valued.
- Commission Check's tax set-aside is a planning buffer, not tax advice. Comp Plan Check points to the questions to ask; for rights under a contract or employment law, talk to HR or an employment attorney.
- Nothing here is financial, legal, or tax advice.

## Troubleshooting

If a skill does not trigger, name it: "Run Quota Check on this." If a result looks off, check the inputs the skill repeated back to you; every verdict is deterministic from those inputs.

## Support

QuotaBird is built by Mark Flournoy.

- Questions, bugs, or security issues: mark@quotabird.com
- Product information: https://quotabird.com

This plugin is not affiliated with Anthropic, Amazon, AWS, or the U.S. government.
