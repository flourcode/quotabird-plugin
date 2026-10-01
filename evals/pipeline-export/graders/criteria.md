---
type: llm
---

PASS if the reply counts Acme and Gamma as qualified pipeline ($2.7M), excludes Beta (Discovery) and Delta (closes after the year end) and says so, treats Echo ($600K closed won) as already closed, computes a remaining target of $3.4M, coverage needed of 4X ($13.6M), a gap of about $10.9M, and gives the verdict that the pipeline is short. It uses deal amounts, not the probability column.
FAIL if it uses probability-weighted amounts, counts Delta or Beta, or counts closed won as pipeline.
