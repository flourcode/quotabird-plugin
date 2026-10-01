---
tags: [pipeline, export, math]
allowed_tools: [Skill, AskUserQuestion]
expected_outcome: Pipeline Check reads the export: qualified = Proposal and Negotiation closing by Sep 30 2027 = $2.7M; closed $600K; at 25% need $13.6M; "No. You're short."
---

Here's my pipeline export. Our year ends September 30, 2027. Target is $4M, win rate 25%. Proposal and Negotiation count as qualified.

account,amount,stage,close_date,probability,notes
Acme,1500000,Proposal,2027-03-15,60%,
Beta,900000,Discovery,2027-02-01,10%,
Gamma,1200000,Negotiation,2027-06-30,80%,
Delta,800000,Proposal,2027-11-15,60%,
Echo,600000,Closed Won,2026-12-10,100%,
Fox,400000,Closed Lost,2026-11-20,0%,

Is that enough?
