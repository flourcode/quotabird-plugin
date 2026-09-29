# Quota Check: reference

Ported from quotabird.com/quota. Do not re-tune.

## Math

- OTE = base + variable
- multiple = quota ÷ OTE
- variable share = variable ÷ OTE
- implied rate on quota = variable ÷ quota (what a dollar of quota pays at 100%)
- growth over last year = (quota − closed last year) ÷ closed last year, only if last year was given. Flag it when over +30%.

Show the multiple with one decimal below 10 (4.6x) and as a whole number at 10 and above (21x). Show the implied rate as a whole percent at 10% and above, one decimal from 1% to 10%, two decimals below 1%.

## Cutoffs by basis

| Basis | c0 | c1 | c2 | c3 | c4 | Working range ("standard") |
|---|---|---|---|---|---|---|
| Bookings (new ARR or ACV) | 3 | 4 | 6 | 8 | 12 | 4 to 6x |
| Run rate (cloud consumption growth) | 8 | 15 | 30 | 45 | 60 | 15 to 30x |
| Whole book | 20 | 40 | 80 | 120 | 160 | 40 to 80x |

If the basis is unknown, ask. (The site defaults to run rate only when nothing is chosen.)

## Bands and fixed verdict text

Let X be the multiple, and "the range" be c1 to c2 for the basis.

| Condition | Verdict (say this first) | Sentence | Next line |
|---|---|---|---|
| X < c0 | It's unusually low. | Your quota is Xx your OTE. For [basis] that's unusually low: a ramp, an overlay, or a plan with a condition in it. | Read the plan twice. Low multiples usually come with a catch. |
| c0 ≤ X < c1 | No. It's favorable. | Your quota is Xx your OTE, below QuotaBird's working range of [range] for [basis]. | Common in new territories, SMB and commercial. Enjoy it while it lasts. |
| c1 ≤ X ≤ c2 | No. It's standard. | Your quota is Xx your OTE, inside QuotaBird's working range of [range] for [basis]. | The number is ordinary. Whether the territory can produce it is a different question. |
| c2 < X ≤ c3 | Not crazy. A stretch. | Your quota is Xx your OTE, above QuotaBird's working range of [range] for [basis]. | Normal for enterprise and strategic roles, and it needs a strong pipeline behind it. |
| c3 < X ≤ c4 | Close. It's aggressive. | Your quota is Xx your OTE, well above QuotaBird's working range of [range] for [basis]. | Strategic-account territory. You need coverage and a territory that can produce it. |
| X > c4 | Yes. It's crazy. | Your quota is Xx your OTE. For [basis], the plan is asking your territory for something it may not have. | Check the territory before you sign, and get the sizing in writing. |

Basis names in sentences: "new bookings", "cloud consumption growth", "a whole book".

## Pay-mix note

- Variable share under 40%: "Variable is under 40% of OTE. You're paid mostly to show up, and the quota matters less than it looks."
- Variable share over 60%: "Variable is over 60% of OTE. The quota is most of your pay. Treat it like one."

## Where the ranges come from (say this when asked, and label it this way always)

- **Bookings, 4 to 6x:** a QuotaBird working range built around published data. Bridge Group's 2026 study of 158 B2B companies reports a median quota-to-OTE of 4.6x; its 2024 study reported a 4.2x median with the middle half between 3.2x and 4.8x.
- **Run rate 15 to 30x and whole book 40 to 80x:** QuotaBird working ranges from cloud-provider plans, not a published survey. They follow from one identity: quota ÷ OTE = variable share ÷ commission rate. With a 46% variable share, a rate of about 1.5 to 3% on consumption growth gives 15 to 30x, and about 0.6 to 1.2% on a whole book gives 40 to 80x.
- Never call any of these an industry average or benchmark.

## Worked example

Base $150,000, variable $130,000, quota $6,000,000, run rate. OTE $280,000. Multiple 21.4x, shown as 21x. Implied rate 2.2%. Variable share 46%. Band: 15 ≤ 21.4 ≤ 30, so "No. It's standard. Your quota is 21x your OTE, inside QuotaBird's working range of 15 to 30 for cloud consumption growth."
