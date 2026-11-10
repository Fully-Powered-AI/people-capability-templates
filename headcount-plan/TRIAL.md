# Headcount plan: a trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs for this trial are the invented example in `public/example.md` (Company A, a made-up 16-person software company). No client data was used. The assistant that ran it did not write the template. It read the template's instruction block and output format, took only the five inputs from the example (scope brief, current roles list, changes list, notes, settings), produced the plan, and only then compared it with the example's output and the reviewer checklist.

One thing to know about how it was run: the arithmetic was done with a small throwaway script written for the trial, not by hand. The script followed the template's cost formula, and the plan below was written from its results. A chat assistant without code tools would do the same sums in its head, which is a larger risk of slips than this trial shows.

## Inputs used

The five inputs under "The inputs" in `public/example.md`, unchanged: scope brief, current roles list (8 rows), changes list (6 rows), eight notes, and settings. The settings gave no pay gap, so the template's default of 15% applied.

## What came out

**HEADCOUNT PLAN: Company A, Jan 2027 to Dec 2027**

For: Chief executive. Prepared by: Finance and people lead. Prepared: 10 November 2026. Currency: US dollars. Why now: the board reviews next year's budget in December.

From: current roles list (8 rows), changes list (6 rows), notes (8 notes), settings; defaults used: pay gap 15%.

Read by: Chief executive, Finance and people lead.

Left out: a person's name (note 2); leave (note 8).

**SUMMARY**

Base case: 16 people now, 20 by Dec 2027 (+4). Cost for the year $3,055,088 against a budget of $2,940,000: over by $115,088.

Lower case: 18 people by Dec 2027; cost $2,734,988, under by $205,012.

Higher case: 21 people by Dec 2027; cost $3,116,088, over by $176,088.

Changes: 6 (2 approved, 3 proposed, 1 confirmed departure). Flags: 1. Questions: 4.

**CURRENT ROLES, Jan 2027, at today's pay**

Product and engineering
- Engineering lead · one person · Employee · Pay $180,000 a year · Bonus target 10% · $20,300 a month
- Software engineer · 6 people · Employee · Pay $840,000 a year · Bonus target 0% · $87,000 a month
- Product designer · one person · Employee · Pay $120,000 a year · Bonus target 0% · $12,500 a month

Team total: 8 people, $119,800 a month.

Sales and customer
- Account executive · 2 people · Employee · Pay $200,000 a year · Bonus target 20% · $25,000 a month
- Customer success manager · 3 people · Employee · Pay $270,000 a year · Bonus target 0% · $28,500 a month

Team total: 5 people, $53,500 a month.

Operations
- Chief executive · one person · Employee · Pay $150,000 a year · Bonus target 0% · $15,500 a month
- Finance and people lead · one person · Employee · Pay $130,000 a year · Bonus target 0% · $13,500 a month
- Bookkeeper · one person · Contractor · Pay $36,000 a year · Bonus target 0% · $3,000 a month

Team total: 3 people, $32,000 a month.

Company total: 16 people (1 contractor), $205,300 a month. Cost rate entering the year: $2,463,600.

**CHANGES IN THE PLAN**

P1 Product and engineering, Software engineer: New 2 from Mar 2027. Approved. Employee. Pay $140,000 a person a year. In: all cases; lower case from Jun 2027. Cost in the plan year: $296,000 (base case), including one-off $6,000; lower case $209,000. Why: Second product team (note 1: the board approved it at its September meeting).

P2 Sales and customer, Customer success manager: Leaving 1 from Feb 2027. Confirmed. Employee. Pay: role average $90,000 a person a year. In: all cases. Cost in the plan year: −$107,740 (base case). Why: Confirmed departure (note 2: leaves at the end of January; the backfill is wanted from March).

P3 Sales and customer, Customer success manager: Backfill 1 from Mar 2027. Approved. Employee. Pay $92,000 a person a year. In: all cases. Cost in the plan year: $100,000 (base case), including one-off $3,000. Why: Replaces the departing customer success manager.

P4 Sales and customer, Account executive: New 1 from Apr 2027. Proposed. Employee. Pay $120,000 a person a year, bonus target 20%. In: base and higher cases. Cost in the plan year: $137,100 (base case), including one-off $3,000. Why: New region (note 3: the region opens only if the spring renewals come in; not opened if revenue lands low). FLAG: pay 20% above the role's current average.

P5 Product and engineering, Product manager: New 1 from Jul 2027. Proposed. Employee. Pay $150,000 a person a year. In: base and higher cases. Cost in the plan year: $96,000 (base case), including one-off $3,000. Why: First product manager (note 4: the chief executive's priority, but it can wait if revenue is low).

P6 Product and engineering, Software engineer: New 1 from Sep 2027. Proposed. Employee. Pay $140,000 a person a year. In: higher case only. Cost in the plan year: $61,000 (higher case), including one-off $3,000. Why: Faster roadmap if revenue lands high (note 5: a third engineer in September if revenue lands high).

**MONTH BY MONTH, BASE CASE**

- Jan 2027 · People 16 · Cost $205,300 · Budget $245,000 · Under $39,700
- Feb 2027 · People 15 · Cost $195,800 · Budget $245,000 · Under $49,200
- Mar 2027 · People 18 · Cost $243,500 · Budget $245,000 · Under $1,500
- Apr 2027 · People 19 · Cost $259,832 · Budget $245,000 · Over $14,832
- May 2027 · People 19 · Cost $256,832 · Budget $245,000 · Over $11,832
- Jun 2027 · People 19 · Cost $256,832 · Budget $245,000 · Over $11,832
- Jul 2027 · People 20 · Cost $275,332 · Budget $245,000 · Over $30,332
- Aug 2027 · People 20 · Cost $272,332 · Budget $245,000 · Over $27,332
- Sep 2027 · People 20 · Cost $272,332 · Budget $245,000 · Over $27,332
- Oct 2027 · People 20 · Cost $272,332 · Budget $245,000 · Over $27,332
- Nov 2027 · People 20 · Cost $272,332 · Budget $245,000 · Over $27,332
- Dec 2027 · People 20 · Cost $272,332 · Budget $245,000 · Over $27,332
- Year · People at year end 20 · Cost $3,055,088 · Budget $2,940,000 · Over $115,088

**THREE CASES**

- Lower · People at year end 18 · Cost for the year $2,734,988 · Under budget by $205,012 · Months over budget: Jun 2027 · Revenue $4,200,000 · People cost 65.1% of revenue · Revenue per person $233,333 · Cost rate entering next year $2,903,184
- Base · People at year end 20 · Cost for the year $3,055,088 · Over budget by $115,088 · Months over budget: Apr 2027 to Dec 2027 · Revenue $4,800,000 · People cost 63.6% of revenue · Revenue per person $240,000 · Cost rate entering next year $3,267,984
- Higher · People at year end 21 · Cost for the year $3,116,088 · Over budget by $176,088 · Months over budget: Apr 2027 to Dec 2027 · Revenue $5,400,000 · People cost 57.7% of revenue · Revenue per person $257,143 · Cost rate entering next year $3,441,984

What changes: Lower case: P4 and P5 left out; P1 from Jun 2027 instead of Mar 2027. Higher case: P6 added.

**ASSUMPTIONS AND CHECKS**

- On-cost: 20% of base pay and bonus target, employees only (settings).
- Per-person cost: $500 a month for each employee (settings).
- One-off cost: $3,000 for each person joining, in the month they join (settings).
- Pay review: 4% from Apr 2027, current roles only (settings).
- Bonus targets: spread evenly across the months.
- Contractors: annual amount divided by twelve, nothing added.
- Departures: at the role's average pay.
- Budget: $2,940,000 for the year, spread evenly at $245,000 a month (settings).
- Check against the accounts: Oct 2026, people cost $201,800 and 16 people paid (settings); current roles $205,300 a month and 16 people; difference $3,500 (1.7%), within 5%.

**QUESTIONS FOR THE CHIEF EXECUTIVE**

1. The base case costs $3,055,088 for the year against the budget of $2,940,000 (settings), $115,088 over. It is over in every month from Apr 2027 to Dec 2027, by between $11,832 and $30,332. Which changes, if any, should move or come out, or should the budget change?
2. The higher case costs $3,116,088 for the year, $176,088 over the same budget (settings). Does the budget rise with the higher revenue, or must that case fit $2,940,000?
3. Note 6 asks that people cost stay under 60% of revenue. The lower case is at 65.1% ($2,734,988 against $4,200,000) and the base case at 63.6% ($3,055,088 against $4,800,000); the higher case is at 57.7% ($3,116,088 against $5,400,000). How should the lower and base cases meet the limit, or is the limit measured another way?
4. P4: pay of $120,000 a year is 20% above the current average of $100,000 for an account executive in Sales and customer (current roles list). Is that the pay intended for the new-region role?

**ALSO NOTED**

- Note 7: the bookkeeper's contract renews in June at the same rate.

Draft for the Chief executive's approval. It plans roles and cost only: no person has been named or chosen, no role opened or posted, no offer made, and no pay, payroll, record or budget changed.

## What was observed

**Every required part was produced.** All sections of the output format appear, in order. The assistant was not told to stop at any point: both lists had the default headers, no team and role or Ref repeated, every New and Backfill row had pay, month and a whole number of people, and the one Leaving row matched a current role and took away fewer people than it has.

**Difference from the published example.** None in any figure. Every amount, count, flag, question, and the left-out list matched the example's output. The only differences are small wording choices: the notes' "what it adds" text on P2, P4, P5 and P6, and the second question's phrasing (the example also mentions P6's $61,000 and the $5,400,000 revenue; this trial left those out). Both are within what the format allows. The two outputs were produced independently, so the agreement on all the figures is a real check on the template's formula, though it is one run by one model and says nothing about other products.

**Facts not in the inputs.** None found in either output. Every figure is either in the inputs or derived from them. The name in note 2 and the leave in note 8 were left out as the template requires.

**Where the template was ambiguous or a guess was needed.**
1. Step 2 says not to repeat "one person's own pay", but the output format and the stop conditions require each current role, including one-person rows such as the chief executive and the engineering lead, to be shown with its pay and marked "one person". The template resolves this only by implication (the pay is the role's pay, and Read by is kept to two people). A cautious model could reasonably leave those amounts out and fail the format. The assistant, like the example, showed them.
2. Whether the per-person monthly cost ($500) counts in the saving from a departure. The formula for an employee row includes it and a departure is costed "at the matching current row's average", so the assistant included it ($9,500 a month before the pay review, $9,860 after). It matches the example, but the departure step does not say so in words.
3. The pay review multiplies base pay before the bonus target and the on-cost are applied. The formula implies this, and nothing says otherwise.
4. A note used "elsewhere" is not defined. The assistant attached notes 1 to 6 to the change they relate to, which is what the example does, and left only note 7 under Also noted. Note 5 adds nothing beyond P6's reason, yet the format's "(note n: what it adds)" invites a restatement. A model could just as reasonably list notes that add nothing under Also noted.
5. Note 7 (the bookkeeper's contract renews at the same rate) has no effect on any figure, so Also noted is correct, but a reader might expect the plan to say it was checked.
6. The month-by-month "people" count includes the contractor. Step 8 says so; the summary's "16 people now" does too. It is easy to misread if you are counting employees.
7. There is a one-month gap with no customer success manager cover (February) between the departure and the backfill. The template has no flag for a gap, only for an overlap, so nothing was raised. This matches the example.
8. The cost rate entering next year takes the last month's cost less one-off costs in it. In this example December has no one-off cost, so the rule was not exercised.
9. The answer to "which questions" depends on judging whether the higher case being over budget needs its own question. The template says each case over budget does, so question 2 follows; but the template does not say whether to ask it as a question about the budget or about the higher case's changes. The assistant asked about the budget.

**Shortcomings.** The trial ran once, with one model, on a small, tidy example: no stop condition, no renamed header, no personal detail beyond a name and a leave, no overlap, no lower case month on a change that is not in the lower case. Most of the template's acceptance tests (stop conditions, overlap, backfill with no departure, declining requests, a check outside tolerance) were not exercised. The script's totals were compared with the example only after the plan was written.

## After this run

The output and observations above are as recorded and have not been changed. After the review, the same day, the template's wording was clarified without changing any input, formula, section or figure, and the template was not run again:

- Observation 1: the template now says in words that a one-person row is still shown with its pay, marked "one person". This run already did so.
- Observation 2: the departure step now says the saving includes the per-person monthly cost for an employee. This run already did so.
- The instruction block now states the month format ("Jan 2027") and the rule to keep Read by to the approver and the preparer when a row has one or two people. This run already followed both.
- Observation 4: a note that adds nothing beyond a change's reason is now cited by its number alone, as "(note 5)", and still counts as used. This run attached notes in the same way but restated note 5 on P6; the clarified template would print "(note 5)" there, as the published example does.
- When this record was written, the published example's Left out line read "family leave (note 8)" where this run wrote "leave (note 8)", a wording difference the comparison above did not mention. The example now reads "leave (note 8)".
- Observation 7: a month with no cover between a departure and its backfill is still not flagged; the template now lists it under what to customize.
