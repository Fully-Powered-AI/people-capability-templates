# Employee health plan comparison: tried on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-10

The inputs were the invented example in [example.md](example.md): Company A, Broker D, Insurer X and Insurer Y, and the invented people and figures in it. No client data was used. The run followed the instructions block and the output format in the member template (version 0.1.0, as revised on 10 November 2026 after an earlier run and a review; see "The earlier run" below). The arithmetic was checked with a short script that was run for this trial, not worked by eye.

This run is not independent of the template. The same session that made the revisions then ran it, and had already read the example's published output and the earlier run's record. It shows that the revised instructions can be followed to the output below; it is not a blind test.

## Inputs used

All eight inputs from the example: the scope brief, the plan list (4 rows), the premium list (12 rows), the contribution list (3 tiers), the enrollment list (30 enrolled), Broker D's notes B1 to B6, the preparer's notes N1 to N4, and the settings.

## What came out

```
HEALTH PLAN COMPARISON: Company A, plan year from 1 January 2027

For: Owner. Prepared by: Office and people manager. Prepared: 10 November 2026. Decision due: 1 December 2026. Currency: US dollars. Why now: Broker D has sent the renewal and two alternative quotes.
From: plan list (4 rows), premium list (12 rows), contribution list (3 tiers), enrollment list (30 enrolled), broker's notes (6), preparer's notes (4), settings.
Read by: Owner, Office and people manager.
Left out: a person's name, their treatment and their question about their own cover (N3). The question in N3 about a person's own cover goes to the broker or the insurer, privately, with that person.

SUMMARY
Options compared: 3 (Plan A, renewal; Plan B, alternative; Plan C, alternative). Enrolled today: 30 of 38 employees (78.9%).
Cost to the company for the year: Plan A, renewal $246,068; Plan B, alternative $210,984; Plan C, alternative $199,548. This year: $221,712. Budget: $235,000.
Lowest cost to the company: Plan C, alternative. Lowest cost to a typical employee: low use Plan C, alternative; middle use Plan B, alternative; high use Plan C, alternative.
Renewal: total premiums up 11.0%. Flags: 1. Questions for the broker: 7. Points for the Owner: 4.

PLAN DESIGN
Plan A, renewal: Insurer X. PPO. Network: Insurer X broad network. Deductible $1,500 single, $3,000 family. Coinsurance 20%. Out-of-pocket maximum $5,000 single, $10,000 family. Primary care $30. Specialist $60. Generic drugs $10. Out-of-network: 40% after a separate $3000 deductible.
Plan B, alternative: Insurer Y. HMO. Network: Insurer Y regional network (B2: a specialist visit needs a referral from the member's primary care doctor; the children's hospital downtown is in the network, the university medical center is not). Deductible $500 single, $1,000 family. Coinsurance 20%. Out-of-pocket maximum $5,500 single, not stated in the documents family. Primary care $25. Specialist $50. Generic drugs $10. Out-of-network: No (emergencies only).
Plan C, alternative: Insurer X. High-deductible. Network: Insurer X broad network (B3: the same broad network as Plan A). Deductible $3,300 single, $6,600 family. Coinsurance 10%. Out-of-pocket maximum $6,000 single, $12,000 family. Primary care after deductible. Specialist after deductible. Generic drugs after deductible. Out-of-network: 30% after deductible.

PREMIUMS AND SHARES, per month
Plan A, renewal
- Employee only · Premium $688.00 · Company $550.40 · Employee $137.60 · Employee for the year $1,651
- Employee + one · Premium $1,445.00 · Company $722.50 · Employee $722.50 · Employee for the year $8,670
- Family · Premium $1,996.00 · Company $998.00 · Employee $998.00 · Employee for the year $11,976
Plan B, alternative
- Employee only · Premium $590.00 · Company $472.00 · Employee $118.00 · Employee for the year $1,416
- Employee + one · Premium $1,239.00 · Company $619.50 · Employee $619.50 · Employee for the year $7,434
- Family · Premium $1,711.00 · Company $855.50 · Employee $855.50 · Employee for the year $10,266
Plan C, alternative
- Employee only · Premium $495.00 · Company $396.00 · Employee $99.00 · Employee for the year $1,188
- Employee + one · Premium $1,040.00 · Company $520.00 · Employee $520.00 · Employee for the year $6,240
- Family · Premium $1,436.00 · Company $718.00 · Employee $718.00 · Employee for the year $8,616

COST TO THE COMPANY FOR THE YEAR, at today's enrollment
- Plan A, renewal · Premiums $402,972 · Company share $246,068 · Employer account none · Company total $246,068 · Against this year +$24,356 (+11.0%) · Against budget over $11,068
- Plan B, alternative · Premiums $345,504 · Company share $210,984 · Employer account none · Company total $210,984 · Against this year -$10,728 (-4.8%) · Against budget under $24,016
- Plan C, alternative · Premiums $289,944 · Company share $177,048 · Employer account $22,500 · Company total $199,548 · Against this year -$22,164 (-10.0%) · Against budget under $35,452
- This year, Plan A, current · Premiums $363,072 · Company share $221,712 · Company total $221,712

COST TO A TYPICAL EMPLOYEE FOR THE YEAR, employee-only cover
Use levels: low $800, middle $6,000, high $40,000 of covered in-network spending.
- Plan A, renewal · Premium share $1,651 · Low: out-of-pocket $800, total $2,451 · Middle: out-of-pocket $2,400, total $4,051 · High: out-of-pocket $5,000, total $6,651
- Plan B, alternative · Premium share $1,416 · Low: out-of-pocket $560, total $1,976 · Middle: out-of-pocket $1,600, total $3,016 · High: out-of-pocket $5,500, total $6,916
- Plan C, alternative · Premium share $1,188 · Low: out-of-pocket $800, total $1,238 · Middle: out-of-pocket $3,570, total $4,008 · High: out-of-pocket $6,000, total $6,438 · Employer account $750 taken off each total

WHAT THE RENEWAL CHANGES
Plan A: Deductible single from $1,000 to $1,500; Deductible family from $2,000 to $3,000; Out-of-pocket max single from $4,500 to $5,000; Out-of-pocket max family from $9,000 to $10,000; Out-of-network from "40% after a separate $2000 deductible" to "40% after a separate $3000 deductible". Employee only premium from $620.00 to $688.00 (+11.0%); Employee + one premium from $1,302.00 to $1,445.00 (+11.0%); Family premium from $1,798.00 to $1,996.00 (+11.0%). Total premiums for the year at today's enrollment from $363,072 to $402,972 (+$39,900, +11.0%). FLAG: above the renewal threshold of 10%.

QUESTIONS FOR THE BROKER
1. Plan B, alternative: the family out-of-pocket maximum is not stated in the documents (plan list). What is it?
2. Plan A, renewal: total premiums for the year at today's enrollment rise from $363,072 to $402,972, up $39,900 or 11.0%, above the renewal threshold of 10% (premium list, settings); B1 puts the rise at about 11%. What is behind the increase, and is there room on the renewal rates?
3. B1 says Insurer X will hold the rise at 8% if Plan A's single deductible moves to $2,000, with full terms on request; those terms are not in the plan list or the premium list. Can you send them in full, with every field that changes and the premium for each tier?
4. B5 says each plan has its own drug list and that you can send them; none was supplied. Can you send the drug lists for Plan A, renewal, Plan B, alternative, and Plan C, alternative?
5. N1 says almost all staff live within 20 miles of the office, and no broker note says how far either network reaches. Can you send the in-network primary care doctors and hospitals within 20 miles of the office for the Insurer X broad network (Plans A and C) and the Insurer Y regional network (Plan B)?
6. N2 says several families on the team use the children's hospital downtown, which is in the current network. B2 says it is in Plan B's network; no broker note says whether it stays in the Insurer X broad network used by Plan A, renewal, and Plan C, alternative (B3). Is it in that network for next year?
7. B6 says all rates assume at least 70% of eligible employees enroll. Enrolled today: 30 of 38 employees, 78.9% (enrollment list, settings). How does each insurer count eligible employees, and does the condition hold at that count for all three plans?

POINTS FOR THE OWNER
1. Plan A, renewal: the company total of $246,068 for the year is over the budget of $235,000 by $11,068 (settings). Which should move: the plan, the company's contribution or the budget?
2. Plan C, alternative: the employer account of $750 a year for each enrolled employee is marked proposed (settings). At today's enrollment it costs $22,500, included in Plan C's company total of $199,548. Is it decided at that amount?
3. Plan B, alternative, changes the plan type from PPO to HMO and the network from the Insurer X broad network to the Insurer Y regional network: a specialist visit needs a referral and the university medical center is not in the network (B2), and out-of-network care is covered only in an emergency (plan list). Does the company want to offer Plan B?
4. Plan C, alternative, changes the plan type from PPO to high-deductible on the same broad network (B3); primary care, specialist visits and generic drugs are paid after the deductible (plan list). Does the company want to offer Plan C?

ASSUMPTIONS
- Every employee enrolled today takes the option, at today's tier.
- Premiums: monthly figures times 12. Company shares: Employee only 80%; Employee + one 50%; Family 50% (contribution list).
- Typical employee: employee-only cover, in-network care only, spending of $800, $6,000 and $40,000 a year (settings), through the deductible, then coinsurance, up to the out-of-pocket maximum.
- Copays: shown under Plan design for Plan A, renewal and Plan B, alternative, not counted in the totals; a copay charged before the deductible means a low user may pay less than shown.
- Employer account: $750 a year for each enrolled employee on Plan C, alternative, proposed, taken off the typical employee's total in full, with no tax effect counted.
- Rounding: monthly premiums and shares to the cent, other amounts to the whole dollar.

ALSO NOTED
- B4: quotes are valid until 1 December 2026; the decision is needed by then for a 1 January start.
- N4: the owner wants to keep paying 80% of employee-only cover and half of the other tiers, whichever plan is chosen.

Draft for the Owner's decision. It compares plans from the documents supplied and gives no advice on insurance, tax or the law. It says nothing about which plan any employee should choose. No quote has been accepted, no application signed, no one enrolled, nothing sent or paid, and no payroll or record changed.
```

## What was observed

- **Every required part was produced.** All sections of the output format were filled, in order, with the closing draft line. Nothing made the run stop: all inputs and headers were present, no plan, status or tier was duplicated, no premium or contribution was missing, and an employee-only tier exists.
- **The figures were checked by script.** Every premium share, company cost, comparison with this year and the budget, typical-employee figure and renewal change was recomputed from the inputs by the script and agrees with the output above. The lowest typical-employee cost is Plan C at low use ($1,238), Plan B at middle use ($3,016) and Plan C at high use ($6,438, against $6,651 for Plan A, renewal and $6,916 for Plan B).
- **The figures agree with the example.** Every amount and percentage matches the published example's body and summary, to the dollar.
- **The revised rules were exercised.** The drug-list note (B5), which covers every plan, was not repeated beside each network and became question 4. The N3 question about a person's own cover was not answered, and the Left out line sends it to the broker or the insurer, privately. Plan C, which changes type but not network, received its own point. The Flags count of 1 is the renewal flag; plan design raised none. "Proposed" appears in the Assumptions line for the employer account.
- **Differences from the example, none in a figure.** Wording only: question 2 here cites B1 and also asks whether there is room on the renewal rates, where the example also cites the deductible and maximum rises; question 3 asks for every changed field rather than listing them; question 5 asks for the doctors and hospitals rather than their number; point 3 names the network change and leaves out the children's hospital (N2), which the example repeats there and both ask about in question 6. Smaller differences of phrasing, with the same facts and figures, run through questions 4, 6 and 7 and points 1, 2 and 4: question 4 here names each option in full, question 7 asks whether the condition holds at today's count, and point 4 says the plan type changes "on the same broad network".
- **Nothing was added that is not in the inputs.** The 78.9% enrollment share, the 11.0% rises and the account cost of $22,500 are worked from the inputs; that Plan B covers out-of-network care only in an emergency is read from the plan list.
- **The reviewer checklist held on this run.** Rows and counts match (1). Shares match the contribution list (2). Totals add up from enrollment, premium and the account (3). Each typical-employee figure follows the formula, including the cap and the below-deductible cases (4). Every differing field is listed (5). No person is named or described (6). Each blank field and flag has a question, and nothing recommends a plan (7). Item 8 concerns the broker's answers and the approver's decision, which come after the draft.

## The earlier run

An earlier run on the same date (Claude Sonnet 5.5, model ID claude-sonnet-5-5) followed the template as first written. It found that the published example had an error: the example's summary said the lowest cost to a typical employee at high use was "Plan A, renewal", while its own body showed Plan C at $6,438 against $6,651 for Plan A, renewal. The earlier run's summary said Plan C. The example's summary was corrected after that run, and now says Plan C, alternative. That run also asked whether the children's hospital (N2) is in the Insurer X network, which the example then lacked; the example now asks it.

It recorded these points where the instructions needed a guess, each addressed in the revision this run used:

- "Employee for the year" sits in the monthly section while other amounts print in whole units. The rounding rule now names it as a whole-unit amount.
- Whether "Flags" counts plan-design and renewal flags together. It now does, in so many words.
- Where a broker note covering every plan goes. It now goes once, as a question or under Also noted, not beside each plan.
- Whether a change of type alone earns a point. It now does.
- Nothing told the preparer where a person's own question in the notes should go. The Left out line now says it goes to the broker or the insurer, privately.
- The Assumptions line had no slot for a proposed employer account. It now has one.
- This year's cost to a typical employee is not shown beside the options. That is unchanged and is listed under What to customize.

## What was not exercised

The three-or-fewer-enrolled reader check (every tier had five or more), the "not calculated" path, the stop conditions and the refusals were not triggered by this example, so this run says nothing about them. The template's acceptance tests are still proposed, and none was run here.

## Edits made after this run

After an independent review, three small edits were made that have not been run again. The instructions block now repeats three input rules the procedure already stated: plans and tiers are matched across lists exactly as written, extra columns are ignored, and a set of notes not given is written as "none supplied". The procedure, the instructions block and the summary line of the output format now say that an option whose typical-employee cost is not calculated is left out of the lowest-cost line and named there; this example has no such option, so the output above would not change. In the example, point 2 for the Owner now says the account "costs $22,500, included in Plan C's company total of $199,548", the wording of this run, where it said "adds $22,500 to Plan C's company total". No figure changed.

## What this does and does not show

One run of one product on one invented example, by the session that revised the template. It shows the instructions can be followed to a complete, checkable output. It does not show how the template behaves with real broker documents, with other products, or on the cases listed above as not exercised.
