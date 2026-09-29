---
name: quota-check
description: "Judge a sales quota against OTE and what it measures: low, favorable, standard, a stretch, aggressive, or crazy. Use when someone asks if a quota is sane, fair, or too high."
---

# Quota Check

Answers one question: is your quota crazy? It divides quota by OTE and compares the multiple with the range for what the quota is measured on. It does not judge whether the territory can produce the number.

## Inputs

Collect these, and only these. Ask for what is missing in one message.

1. **What the quota is measured on.** One of: bookings (new ARR or ACV), run rate (cloud consumption growth), whole book. If the user does not say, ask. Do not guess; the ranges differ by a factor of ten.
2. **Base salary.**
3. **Target variable at 100%.** If the user gives OTE and one of base or variable, derive the other.
4. **Quota.**
5. Optional: what they closed last year on the same measure.

## Steps

1. Compute OTE, the multiple, the variable share, and the implied rate, exactly as in `reference.md`.
2. Pick the band from the cutoffs for the basis. Do not round the multiple before comparing.
3. Give the verdict as an answer to "Is your quota crazy?", using the fixed verdict text.
4. Show the rows: OTE, quota ÷ OTE, implied rate on quota, variable share, and growth over last year if given.
5. Add the pay-mix note if the variable share is under 40% or over 60%.
6. Label the range correctly. Bookings: a QuotaBird working range built around published data (Bridge Group 2026 median 4.6x). Run rate and whole book: QuotaBird working ranges from cloud-provider plans, not a survey.
7. Stop. If the verdict is Aggressive or Crazy, say that the next step is building the case with evidence (quota-case), in one sentence.

## Voice

Plain, dry, to the point. Speak to "you": your quota, your OTE. Say the verdict first. No motivational close. Never present a working range as an industry average.
