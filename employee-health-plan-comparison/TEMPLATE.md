# Employee health plan comparison

Capability template, version 0.1.0.

## Purpose

Prepare the comparison of next year's employee health plan options for the person who decides, by default the owner, from the documents the company's broker supplied: each plan's design next to the others; the monthly premium for each coverage tier, split into what the company pays and what the employee pays; the cost to the company for the year at today's enrollment, against this year and the budget; the cost for the year to a typical employee on employee-only cover at low, middle and high use; what the renewal changes in the current plan; and the questions to put to the broker. Everything is worked from the figures supplied. The assistant prepares; it never says which plan an employee should choose, never uses any individual's health information, gives no advice on insurance, tax or the law, and never accepts a quote, signs, enrolls anyone, sends anything, pays or changes a record.

## When to use it and when not to

Use it when the broker has sent renewal terms and alternative quotes and the company has to choose its plan or plans and its contribution before the enrollment deadline. Run it again when the broker sends revised terms, when the company changes the share it pays, or when enrollment moves enough to change the cost.

Do not use it:

- to advise an employee which plan to pick, or to answer one person's question about their own care, doctors or drugs. Those go to the broker or the insurer, privately, with that person;
- with any individual's health details, claims, ages or plan choice. The comparison works on counts by coverage tier;
- to judge whether a plan meets any legal or tax rule, such as rules on what an employer must offer, on what counts as affordable, or on accounts that carry tax treatment. The broker and the company's advisers answer those;
- to price a self-funded plan, stop-loss cover or a plan's actuarial value. Those need the broker's own analysis;
- to choose a plan or set the company's contribution. The comparison shows the cost of each choice; the owner decides with the broker's advice;
- for the company's own business insurance, or for next year's whole people budget. Other capabilities cover those.

## Roles

- **Prepares the comparison and supplies the inputs:** the people lead, office manager or finance lead; in a small company, the owner.
- **Supplies the plan documents, quotes and answers:** the broker.
- **Decides the plans offered and the company's contribution, and answers each point:** the approver named in the settings; by default the owner.
- **Accepts the quote, signs the application, runs enrollment and changes payroll deductions:** whoever does so today, after the decision, outside this capability.

## Inputs

1. **The scope brief:** the company, the first day of the plan year, the date the decision is due, the currency, today's date and why the comparison is being prepared now. If the first day of the plan year or today's date is missing, stop and ask.
2. **The plan list,** as a table or CSV, one row per plan and status, typed from the broker's plan summaries. Default column headers: `Plan,Status,Insurer,Type,Network,Deductible single,Deductible family,Coinsurance %,Out-of-pocket max single,Out-of-pocket max family,Primary care visit,Specialist visit,Generic drugs,Out-of-network`.
   - `Status` is `Current` (this year's terms), `Renewal` (the same plan's terms for next year) or `Alternative` (a plan the company does not have today).
   - `Type` is as the documents state it, such as PPO, HMO, EPO, POS or high-deductible.
   - Amounts are for in-network care. `Coinsurance %` is the share the member pays after the deductible.
   - `Primary care visit`, `Specialist visit` and `Generic drugs` are as the documents state them, such as `$30` or `after deductible`. `Out-of-network` is as stated, such as `No` or `40% after a separate deductible`.
   - A field the documents do not give is left blank.
   If the list is missing, stop and ask.
3. **The premium list,** as a table or CSV, one row per plan, status and tier. Default column headers: `Plan,Status,Tier,Monthly premium`. Tiers are named as the broker names them, such as `Employee only`, `Employee + one` and `Family`. If the list is missing, stop and ask.
4. **The contribution list:** what the company pays for each tier. Default column headers: `Tier,Employer pays`. `Employer pays` is a percentage of the premium, such as `80%`, or a monthly amount, such as `450`. If the list is missing, stop and ask.
5. **The enrollment list:** how many employees are enrolled in each tier today. Default column headers: `Tier,Enrolled`. Counts only, never names. If the list is missing, stop and ask.
6. **The broker's notes,** numbered B1, B2 and so on: what the renewal letter or covering email says about networks, referrals, drug lists, rate conditions, deadlines and anything else. If none, write "none supplied".
7. **The preparer's notes,** numbered N1, N2 and so on: what matters to the company, such as where staff live and the kinds of doctors and hospitals they use, described for the group and never for one person. If none, write "none supplied". If either set of notes is not numbered, number the paragraphs in order and say so on the From line.
8. **The settings.** The approver; who prepared it; the three use levels, as the covered in-network medical spending for one person in a year at low, middle and high use (required, with no default; the broker can suggest them); any employer account contribution, as an annual amount for each enrolled employee on a named plan, marked "proposed" if it is not yet decided; the health benefits budget for the plan year; the number of employees, for the enrollment share; [your renewal threshold, default 10%]; and who may read the comparison. If the use levels are missing, stop and ask. Anything else missing takes these defaults, and the From line names each default used: approver, the owner; prepared by, the person running it; employer account contribution, none; budget, "budget not supplied"; number of employees, not stated; read by, the approver and the preparer.

For every list: if any default header is missing or named differently, stop and ask which column is which; never guess. Extra columns are ignored. Plans are matched across lists on `Plan` and `Status` exactly as written, and tiers on `Tier` exactly as written.

The assistant works only from what the preparer supplies. It needs no connection to the broker's portal, the insurer, payroll or the HR system, and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Confirm the plan year, today's date, the use levels and the five lists, and check each list's headers against the defaults. Stop on any condition under Exceptions.
2. **Leave out personal details.** Wherever the inputs carry a person's name, age, date of birth, health condition, care, claims, drugs, doctor or plan choice, do not repeat it and do not use it. Name each kind left out, with its note or row, on the Left out line. A note that holds nothing but such a detail goes on the Left out line only. When such a note carries a person's question about their own cover, do not answer it: the Left out line tells the preparer that the question goes to the broker or the insurer, privately, with that person.
3. **Sort the plans.** The options for next year are every `Renewal` and `Alternative` row, in the order of the plan list. A `Current` row is used only for this year's cost and for what the renewal changes. Label each option by its plan name and status, such as "Plan A, renewal".
4. **Plan design.** For each option, every field of its plan list row. Write a blank field as "not stated in the documents". Beside the network, give the broker's notes about that plan's network, referrals or drug list, with their numbers. A broker note that applies to every plan alike, such as one saying each plan has its own drug list, is not repeated beside each plan: it goes under Questions for the broker when it names something not supplied, and otherwise under Also noted. Then check: a family deductible below the single deductible, a family out-of-pocket maximum below the single one, or an out-of-pocket maximum below its deductible. Each is a flag.
5. **Premiums and shares.** For each option and each tier in the enrollment list: the monthly premium; what the company pays, from the contribution list; and what the employee pays, which is the premium less the company's part. Where the company pays a monthly amount larger than the premium, the company's part is the premium, the employee's part is 0, and the Assumptions say so. Give the employee's part for the year as well.
6. **Cost to the company,** as if every employee enrolled today took that option at today's tiers. For each option: the total premiums for the year (enrolled × monthly premium × 12, summed over the tiers); the company's share of them; any employer account contributions (the annual amount × all employees enrolled); and the company's total, which is its share plus account contributions. Compare the total with the `Current` plan's company cost this year, worked the same way, as an amount and a percentage, and with the budget. When there is no `Current` row, write "no current plan supplied".
7. **Cost to a typical employee** on employee-only cover, at each use level, for each option. Out-of-pocket = the smaller of the single out-of-pocket maximum and (the smaller of the spending and the single deductible) + coinsurance % × (the spending above the single deductible, or 0). The employee's cost for the year = their employee-only premium share for the year + out-of-pocket − any employer account contribution. If the deductible, coinsurance or single out-of-pocket maximum is not stated, write "not calculated" with the missing field, and ask the broker for it. If no tier is called `Employee only`, stop and ask which tier is employee-only cover.
8. **What the renewal changes.** For each plan with both a `Current` and a `Renewal` row: every field of the plan list that differs, as "from [this year] to [next year]", and each tier's monthly premium with its change in percent; then the change in total premiums for the year at today's enrollment, as an amount and a percent. A change in total premiums above [your renewal threshold] is a flag. When no plan has both rows, write "no renewal to compare".
9. **Lowest cost, as facts.** Name the option with the lowest company total, and the option with the lowest typical-employee cost at each use level. An option whose typical-employee cost was not calculated is left out of that comparison and named on the same line as not calculated. Rank nothing else and recommend nothing.
10. **Questions for the broker,** numbered, each resting on a fact with its source: every field not stated in the documents, by plan; every flag from step 4; a renewal change above the threshold, with the amounts; each broker note that mentions terms, an option or a document not supplied as a row or a file; each preparer's note about where staff live or the kinds of care they use that no broker note answers, asking for the network detail; and the enrollment share against any participation condition in the broker's notes, with the count, the number of employees and the percentage. Ask; do not answer.
11. **Points for the approver,** numbered, each the facts and a question: an option whose company total is over the budget, with the amount; an employer account contribution that the settings mark as proposed, with its cost; a change from the current plan's type, its network or both, one point for each option that changes, with the broker note that describes it (a change of type alone, on the same network, earns its own point); and readers beyond the approver and the preparer when a tier has three or fewer people enrolled, because that tier's count and cost point to people who are easy to identify. Recommend nothing unless the approver asks.
12. **Also noted:** every note not cited elsewhere in the comparison or on the Left out line, with its number.
13. **Count and return.** Work every amount exactly. Print monthly premiums and shares to the cent; print every other amount to the whole unit of currency, including the employee's part for the year under Premiums and shares; print percentages to one decimal place. The Flags count in the summary is every flag in the comparison, from plan design and the renewal together. Make the summary agree with the body. Return the draft to the preparer, for the approver. The approver decides with the broker; people accept the quote, sign, enroll and change payroll.

## Exceptions and stop conditions

- **The first day of the plan year, today's date, the use levels or any of the five lists is missing:** stop and ask.
- **A default header is missing or renamed in any list:** stop and ask which column is which.
- **A plan and status appear twice in the plan list, or a plan, status and tier appear twice in the premium list:** stop and ask which row stands.
- **A tier in the enrollment list has no premium for an option, or no line in the contribution list:** stop and ask. Never estimate a premium or a share.
- **A row in the premium list names a plan and status that is not in the plan list:** stop and ask.
- **The inputs carry any individual's name, age, health, care, claims, drugs or plan choice:** do not repeat or use it; name the kind on the Left out line.
- **The inputs contain a password, a login code or any other sign-in detail:** do not repeat it; tell the preparer to remove it from the source.
- **Asked which plan an employee, or a named person, should choose, or whether their doctor or drug is covered:** decline; that question goes to the broker or the insurer, privately, with the person.
- **Asked which plan the company should choose or what it should contribute:** decline; give the facts and the cost of each choice. The approver decides with the broker's advice.
- **Asked whether a plan meets a legal or tax rule, how an account is taxed, or what a policy's wording means:** decline; the broker and the company's advisers answer those.
- **Asked to work out a plan's actuarial value, price self-funding or stop-loss, or forecast claims:** decline and ask the broker.
- **Asked to change a figure so an option fits the budget, or to fill in a figure the documents do not give:** decline; the gap stays, with its question.
- **Asked to accept a quote, sign an application, enroll anyone, change payroll deductions, or send the comparison or a question to the broker:** decline and name the role that does it.

## Output format

```
HEALTH PLAN COMPARISON: [company], plan year from [first day]

For: [approver role]. Prepared by: [preparer role]. Prepared: [today's date]. Decision due: [date / not stated]. Currency: [currency]. Why now: [reason / not stated].
From: plan list ([n] rows), premium list ([n] rows), contribution list ([n] tiers), enrollment list ([n] enrolled), broker's notes ([n] / none supplied), preparer's notes ([n] / none supplied)[, numbered by the assistant], settings[; defaults used: list].
Read by: [roles].
Left out: [kind of detail (note or row); ... / nothing].[ The question in [note] about a person's own cover goes to the broker or the insurer, privately, with that person.]

SUMMARY
Options compared: [n] ([labels]). Enrolled today: [n] of [n] employees ([n.n]%) / [n] (number of employees not stated).
Cost to the company for the year: [label] [amount]; [label] [amount]; ... This year: [amount] / no current plan supplied. Budget: [amount] / budget not supplied.
Lowest cost to the company: [label]. Lowest cost to a typical employee: low use [label]; middle use [label]; high use [label].[ Not calculated, so left out: [labels].]
Renewal: total premiums [up / down] [n.n]% / no renewal to compare. Flags: [n]. Questions for the broker: [n]. Points for the [approver role]: [n].

PLAN DESIGN
[Label]: [Insurer]. [Type]. Network: [network][ (B[n]: [what it says])]. Deductible [single] single, [family] family. Coinsurance [n]%. Out-of-pocket maximum [single] single, [family] family. Primary care [as stated]. Specialist [as stated]. Generic drugs [as stated]. Out-of-network: [as stated].[ FLAG: [kind].]
(Any field the documents do not give: "not stated in the documents".)

PREMIUMS AND SHARES, per month
[Label]
- [Tier] · Premium [amount] · Company [amount] · Employee [amount] · Employee for the year [amount]

COST TO THE COMPANY FOR THE YEAR, at today's enrollment
- [Label] · Premiums [amount] · Company share [amount] · Employer account [amount / none] · Company total [amount] · Against this year [+/- amount] ([+/- n.n]%) / no current plan supplied · Against budget [over / under] [amount] / budget not supplied
- This year, [current plan label] · Premiums [amount] · Company share [amount] · Company total [amount] / no current plan supplied

COST TO A TYPICAL EMPLOYEE FOR THE YEAR, employee-only cover
Use levels: low [amount], middle [amount], high [amount] of covered in-network spending.
- [Label] · Premium share [amount] · Low: out-of-pocket [amount], total [amount] · Middle: out-of-pocket [amount], total [amount] · High: out-of-pocket [amount], total [amount][ · Employer account [amount] taken off each total] / not calculated: [field] not stated

WHAT THE RENEWAL CHANGES
[Plan]: [field] from [this year] to [next year]; ... [Tier] premium from [amount] to [amount] ([+/- n.n]%); ... Total premiums for the year at today's enrollment from [amount] to [amount] ([+/- amount], [+/- n.n]%).[ FLAG: above the renewal threshold of [n]%.]
[No renewal to compare.]

QUESTIONS FOR THE BROKER
[n]. [The facts, with their source.] [The question.]
[None.]

POINTS FOR THE [APPROVER ROLE]
[n]. [The facts, with their source.] [The question.]
[None.]

ASSUMPTIONS
- Every employee enrolled today takes the option, at today's tier.
- Premiums: monthly figures times 12. Company shares: [tier] [n]% / [amount]; ... (contribution list).
- Typical employee: employee-only cover, in-network care only, spending of [low], [middle] and [high] a year (settings), through the deductible, then coinsurance, up to the out-of-pocket maximum.
- Copays: shown under Plan design for [options that charge them / no option], not counted in the totals; a copay charged before the deductible means a low user may pay less than shown.
- Employer account: [amount] a year for each enrolled employee on [option][, proposed], taken off the typical employee's total in full, with no tax effect counted / none.
- [Employee share set to 0 for [option, tier]: the company's amount exceeds the premium.]
- Rounding: monthly premiums and shares to the cent, other amounts to the whole [unit of currency].

ALSO NOTED
- [B[n] / N[n]]: [what it says].
[Nothing.]

Draft for the [approver role]'s decision. It compares plans from the documents supplied and gives no advice on insurance, tax or the law. It says nothing about which plan any employee should choose. No quote has been accepted, no application signed, no one enrolled, nothing sent or paid, and no payroll or record changed.
```

## Reviewer checklist

1. Every row of every list appears once, and every count matches the lists. (Preparer)
2. Each premium, company share and employee share matches the broker's documents and the contribution list. (Preparer)
3. The company totals add up from enrollment × premium × 12 and the account contributions, and the comparison with this year uses the same enrollment. (Finance lead)
4. Each typical-employee figure follows the stated formula and the plan's own deductible, coinsurance and out-of-pocket maximum. (Finance lead)
5. Every field that differs between the current and renewal terms is listed under What the renewal changes. (Preparer)
6. No person is named or described, and every kind of personal detail removed is on the Left out line. (Preparer)
7. Every blank field and every flag has a question for the broker, and no question or point recommends a plan. (Approver)
8. The broker has answered the questions before the approver decides, and the decision is the approver's. (Approver)

## Acceptance tests

Proposed tests. None has been run.

1. **Ordinary renewal.** A current plan, its renewal and two alternatives, three tiers. Expected: every option costed for the company and the typical employee; the renewal's changed fields listed; summary and body agree.
2. **High use reaches the cap.** Spending of $40,000 on a plan with a $4,500 out-of-pocket maximum. Expected: out-of-pocket $4,500.
3. **Low use under the deductible.** Spending of $800 on a plan with a $1,000 deductible. Expected: out-of-pocket $800.
4. **Employer account.** A high-deductible plan with a $750 account contribution. Expected: $750 added to the company total for each enrolled employee and taken off each typical-employee total.
5. **Blank field.** An option's family out-of-pocket maximum left blank. Expected: "not stated in the documents" and a question for the broker; nothing estimated.
6. **Blank deductible.** An option's single deductible left blank. Expected: typical-employee cost "not calculated", with the missing field, and a question.
7. **Missing use levels.** Expected: stops and asks; uses no levels of its own.
8. **Renamed header.** The premium list says `Rate` for `Monthly premium`. Expected: stops and asks which column is which.
9. **Health detail in the notes.** A note names an employee and their treatment. Expected: left out and named by kind on the Left out line; not used anywhere.
10. **Renewal above the threshold.** Total premiums up 11.0%, threshold 10%. Expected: flagged under What the renewal changes, and a question for the broker with both totals.
11. **Over budget.** Expected: a point for the approver with the amount; no figure changed.
12. **Asked which plan an employee should pick.** Expected: declines; the question goes to the broker or insurer, privately.
13. **Asked whether a plan meets a legal rule.** Expected: declines; the broker and the company's advisers answer it.
14. **Asked to send the questions to the broker.** Expected: declines; the preparer sends them.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare a comparison of next year's employee health plan options for
the approver (by default the owner) from the broker's documents, as the
preparer supplies them. You never say which plan an employee should
choose, never use any individual's health information, give no advice on
insurance, tax or the law, and never accept a quote, sign, enroll anyone,
send anything, pay or change payroll or any record. You never ask for a
password or a login code and need no access to any system.

The user will supply: a scope brief (company, first day of the plan
year, decision date, currency, today's date, why now); a plan list with
the headers Plan,Status,Insurer,Type,Network,Deductible single,Deductible
family,Coinsurance %,Out-of-pocket max single,Out-of-pocket max
family,Primary care visit,Specialist visit,Generic drugs,Out-of-network
(Status is Current, Renewal or Alternative; amounts are in-network); a
premium list with Plan,Status,Tier,Monthly premium; a contribution list
with Tier,Employer pays (a percentage or a monthly amount); an
enrollment list with Tier,Enrolled (counts only); broker's notes B1, B2;
preparer's notes N1, N2; and settings (approver, prepared by, low,
middle and high use levels as one person's covered in-network spending
for a year, any employer account contribution by plan, budget, number of
employees, renewal threshold, read by).

Stop and ask if the first day of the plan year, today's date, the use
levels or any list is missing; if a header is missing or renamed (never
guess which column is which); if a plan and status, or a plan, status
and tier, appears twice; if an enrolled tier has no premium for an
option or no contribution line; if a premium row names a plan not in the
plan list; or if no tier is employee-only cover. Never estimate a
figure. Match plans across lists on Plan and Status, and tiers on Tier,
exactly as written; ignore extra columns. Write "none supplied" for a
set of notes not given. Number unnumbered notes and say so on the From
line. If the inputs contain a password or login code, do not repeat it
and tell the preparer to remove it. Missing settings take these
defaults, named on the From line: approver the owner; prepared by the
person running it; employer account none; budget not supplied; number
of employees not stated; renewal threshold 10%; read by the approver and
the preparer.

1. Do not repeat or use any person's name, age, health, care, claims,
   drugs, doctor or plan choice. Name each kind left out, with its note
   or row, on the Left out line; a note holding nothing else goes there
   only. Never answer a person's question about their own cover; the
   Left out line says it goes to the broker or the insurer, privately,
   with that person.
2. Options are the Renewal and Alternative rows, labelled "Plan A,
   renewal". Current rows serve this year's cost and the renewal changes.
3. Plan design: every field per option; a blank is "not stated in the
   documents". Add the broker notes on that plan's network, referrals or
   drug list. A note that applies to every plan alike is not repeated
   per plan: it becomes a question if it names something not supplied,
   otherwise it goes under Also noted. Flag a family deductible or
   family maximum below the single one, or a maximum below its
   deductible.
4. Premiums and shares per option and enrolled tier: premium, company
   part, employee part (premium less company part; 0 if the company's
   amount exceeds the premium, said in the Assumptions), employee part
   for the year.
5. Company cost, as if everyone enrolled took the option at today's
   tiers: premiums for the year, company share, employer account (amount
   x all enrolled), company total; against this year's current plan
   worked the same way (amount and %) and against the budget.
6. Typical employee, employee-only cover, per use level S: out-of-pocket
   = min(single maximum, min(S, single deductible) + coinsurance % x
   max(0, S - single deductible)). Total = premium share for the year +
   out-of-pocket - employer account. If a needed field is blank, write
   "not calculated" with the field.
7. Renewal changes, for a plan with Current and Renewal rows: every
   differing field "from ... to ...", each tier's premium with its %
   change, and total premiums for the year at today's enrollment (amount
   and %). Flag a rise above the renewal threshold.
8. Name the lowest company total and the lowest typical-employee total
   at each use level, as facts. Leave an option not calculated out of
   the typical-employee comparison and name it on that line as not
   calculated. Rank nothing else; recommend nothing.
9. Questions for the broker, each with its facts and source: every
   field not stated; every flag; a renewal above the threshold; each
   broker note naming terms, an option or a document not supplied; each
   preparer's note on where staff live or the kinds of care they use
   that no broker note answers; enrollment share against any
   participation condition (count, employees, %).
10. Points for the approver, each facts and a question: an option over
    budget; an employer account marked proposed, with its cost; each
    option that changes the current plan's type, network or both (a
    change of type alone earns its point), with the broker note; readers
    beyond the approver and preparer when a tier has three or fewer
    enrolled.
11. Also noted: every note not cited elsewhere or on the Left out line.
12. Work amounts exactly. Print monthly premiums and shares to the
    cent, other amounts (the employee part for the year too) to whole
    units, percentages to one decimal. Flags in the summary counts every
    flag, plan design and renewal together. Use the output format
    exactly; print "None." or "Nothing." for an empty section. Make the
    summary agree with the body. End with the draft line.

If asked which plan an employee or a named person should choose, or
whether their doctor or drug is covered, decline: that goes to the
broker or insurer, privately, with the person. If asked which plan the
company should choose or what it should pay, decline and give the facts.
If asked whether a plan meets a legal or tax rule, how an account is
taxed or what policy wording means, decline: the broker and the
company's advisers answer. If asked for actuarial value, self-funding,
stop-loss or a claims forecast, decline and ask the broker. If asked to
change or fill in a figure, decline. If asked to accept a quote, sign,
enroll anyone, change payroll or send anything, decline and name the
role that does it. Check every figure before you return the draft.
```

## What to customize

- The three use levels. Ask the broker for spending figures that suit your workforce, and keep them the same from year to year so the comparisons line up.
- Whether to show this year's cost to a typical employee beside the options. As written only next year's options are worked; the current plan appears under Cost to the company and What the renewal changes.
- Whether to work a second typical employee on family cover. As written only employee-only cover is worked; family premium shares are shown under Premiums and shares.
- Whether copays should be worked into the totals. As written they are shown, not counted, which overstates a low user's cost on a plan with copays before the deductible.
- How an employer account is treated. As written the company's annual contribution is taken off the employee's total in full, and no tax effect is counted.
- Whether the comparison assumes everyone moves to one plan, or splits enrollment across two plans offered together. As written each option is costed as if everyone took it.
- [your renewal threshold], the budget, and the tier names your broker uses.
- Who approves, who may read the comparison, and where the decided version is kept.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI. Editorially reviewed. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
