# Employee health plan comparison: an invented example

*Illustrative example with invented data.* The company, the broker, the insurers, the plans, the people, the premiums and the dates below are all invented. Company A is an invented 38-person design and fit-out firm whose health plan renews on 1 January 2027. Its broker, called Broker D here, has sent the renewal terms for the current plan and quotes for two others from invented insurers called Insurer X and Insurer Y. The office and people manager prepares the comparison for the owner. First come the inputs the office and people manager supplied, in full, then the comparison the workflow template returned.

## The inputs

### 1. Scope brief

```
Company: Company A, an invented 38-person design and fit-out firm
First day of the plan year: 1 January 2027
Decision due: 1 December 2026
Currency: US dollars
Today: Tuesday 10 November 2026
Why now: Broker D has sent the renewal and two alternative quotes
```

### 2. Plan list (typed from Broker D's plan summaries)

```
Plan,Status,Insurer,Type,Network,Deductible single,Deductible family,Coinsurance %,Out-of-pocket max single,Out-of-pocket max family,Primary care visit,Specialist visit,Generic drugs,Out-of-network
Plan A,Current,Insurer X,PPO,Insurer X broad network,1000,2000,20,4500,9000,$30,$60,$10,40% after a separate $2000 deductible
Plan A,Renewal,Insurer X,PPO,Insurer X broad network,1500,3000,20,5000,10000,$30,$60,$10,40% after a separate $3000 deductible
Plan B,Alternative,Insurer Y,HMO,Insurer Y regional network,500,1000,20,5500,,$25,$50,$10,No (emergencies only)
Plan C,Alternative,Insurer X,High-deductible,Insurer X broad network,3300,6600,10,6000,12000,after deductible,after deductible,after deductible,30% after deductible
```

### 3. Premium list (from Broker D's quotes)

```
Plan,Status,Tier,Monthly premium
Plan A,Current,Employee only,620
Plan A,Current,Employee + one,1302
Plan A,Current,Family,1798
Plan A,Renewal,Employee only,688
Plan A,Renewal,Employee + one,1445
Plan A,Renewal,Family,1996
Plan B,Alternative,Employee only,590
Plan B,Alternative,Employee + one,1239
Plan B,Alternative,Family,1711
Plan C,Alternative,Employee only,495
Plan C,Alternative,Employee + one,1040
Plan C,Alternative,Family,1436
```

### 4. Contribution list

```
Tier,Employer pays
Employee only,80%
Employee + one,50%
Family,50%
```

### 5. Enrollment list (counts only)

```
Tier,Enrolled
Employee only,18
Employee + one,5
Family,7
```

### 6. Broker's notes (from Broker D's covering email)

```
B1. Plan A renewal: premiums are up about 11%. Insurer X will hold the
    rise at 8% if Plan A's single deductible moves to $2,000. Full terms
    on request.
B2. Plan B is an HMO: a specialist visit needs a referral from the
    member's primary care doctor. The children's hospital downtown is in
    the network; the university medical center is not.
B3. Plan C uses the same broad network as Plan A.
B4. Quotes are valid until 1 December 2026. We need the decision by
    then for a 1 January start.
B5. Each plan has its own drug list. We can send them on request.
B6. All rates assume at least 70% of eligible employees enroll.
```

### 7. Preparer's notes (typed by the office and people manager)

```
N1. Almost all of our staff live within 20 miles of the office.
N2. Several families on the team use the children's hospital downtown,
    which is in our current network.
N3. Maya in the design team is partway through treatment at the
    university medical center and has asked whether a change of plan
    would affect her.
N4. The owner wants to keep paying 80% of employee-only cover and half
    of the other tiers, whichever plan we choose.
```

### 8. Settings

```
Approver: Owner
Prepared by: Office and people manager
Use levels: low 800; middle 6000; high 40000 (from Broker D)
Employer account contribution: Plan C, alternative: 750 a year for each
  enrolled employee (proposed)
Budget: 235000 for health benefits in the plan year
Number of employees: 38
Renewal threshold: 10%
Read by: Owner, Office and people manager
```

## The output

**HEALTH PLAN COMPARISON: Company A, plan year from 1 January 2027**

For: Owner. Prepared by: Office and people manager. Prepared: 10 November 2026. Decision due: 1 December 2026. Currency: US dollars. Why now: Broker D has sent the renewal and two alternative quotes.

From: plan list (4 rows), premium list (12 rows), contribution list (3 tiers), enrollment list (30 enrolled), broker's notes (6), preparer's notes (4), settings.

Read by: Owner, Office and people manager.

Left out: a person's name, their treatment and their question about their own cover (N3). The question in N3 about a person's own cover goes to the broker or the insurer, privately, with that person.

**SUMMARY**

Options compared: 3 (Plan A, renewal; Plan B, alternative; Plan C, alternative). Enrolled today: 30 of 38 employees (78.9%).

Cost to the company for the year: Plan A, renewal \$246,068; Plan B, alternative \$210,984; Plan C, alternative \$199,548. This year: \$221,712. Budget: \$235,000.

Lowest cost to the company: Plan C, alternative. Lowest cost to a typical employee: low use Plan C, alternative; middle use Plan B, alternative; high use Plan C, alternative.

Renewal: total premiums up 11.0%. Flags: 1. Questions for the broker: 7. Points for the Owner: 4.

**PLAN DESIGN**

Plan A, renewal: Insurer X. PPO. Network: Insurer X broad network. Deductible \$1,500 single, \$3,000 family. Coinsurance 20%. Out-of-pocket maximum \$5,000 single, \$10,000 family. Primary care \$30. Specialist \$60. Generic drugs \$10. Out-of-network: 40% after a separate \$3000 deductible.

Plan B, alternative: Insurer Y. HMO. Network: Insurer Y regional network (B2: a specialist visit needs a referral from the member's primary care doctor; the children's hospital downtown is in the network, the university medical center is not). Deductible \$500 single, \$1,000 family. Coinsurance 20%. Out-of-pocket maximum \$5,500 single, not stated in the documents family. Primary care \$25. Specialist \$50. Generic drugs \$10. Out-of-network: No (emergencies only).

Plan C, alternative: Insurer X. High-deductible. Network: Insurer X broad network (B3: the same broad network as Plan A). Deductible \$3,300 single, \$6,600 family. Coinsurance 10%. Out-of-pocket maximum \$6,000 single, \$12,000 family. Primary care after deductible. Specialist after deductible. Generic drugs after deductible. Out-of-network: 30% after deductible.

**PREMIUMS AND SHARES, per month**

*Plan A, renewal*

- Employee only · Premium \$688.00 · Company \$550.40 · Employee \$137.60 · Employee for the year \$1,651
- Employee + one · Premium \$1,445.00 · Company \$722.50 · Employee \$722.50 · Employee for the year \$8,670
- Family · Premium \$1,996.00 · Company \$998.00 · Employee \$998.00 · Employee for the year \$11,976

*Plan B, alternative*

- Employee only · Premium \$590.00 · Company \$472.00 · Employee \$118.00 · Employee for the year \$1,416
- Employee + one · Premium \$1,239.00 · Company \$619.50 · Employee \$619.50 · Employee for the year \$7,434
- Family · Premium \$1,711.00 · Company \$855.50 · Employee \$855.50 · Employee for the year \$10,266

*Plan C, alternative*

- Employee only · Premium \$495.00 · Company \$396.00 · Employee \$99.00 · Employee for the year \$1,188
- Employee + one · Premium \$1,040.00 · Company \$520.00 · Employee \$520.00 · Employee for the year \$6,240
- Family · Premium \$1,436.00 · Company \$718.00 · Employee \$718.00 · Employee for the year \$8,616

**COST TO THE COMPANY FOR THE YEAR, at today's enrollment**

- Plan A, renewal · Premiums \$402,972 · Company share \$246,068 · Employer account none · Company total \$246,068 · Against this year +\$24,356 (+11.0%) · Against budget over \$11,068
- Plan B, alternative · Premiums \$345,504 · Company share \$210,984 · Employer account none · Company total \$210,984 · Against this year −\$10,728 (−4.8%) · Against budget under \$24,016
- Plan C, alternative · Premiums \$289,944 · Company share \$177,048 · Employer account \$22,500 · Company total \$199,548 · Against this year −\$22,164 (−10.0%) · Against budget under \$35,452
- This year, Plan A, current · Premiums \$363,072 · Company share \$221,712 · Company total \$221,712

**COST TO A TYPICAL EMPLOYEE FOR THE YEAR, employee-only cover**

Use levels: low \$800, middle \$6,000, high \$40,000 of covered in-network spending.

- Plan A, renewal · Premium share \$1,651 · Low: out-of-pocket \$800, total \$2,451 · Middle: out-of-pocket \$2,400, total \$4,051 · High: out-of-pocket \$5,000, total \$6,651
- Plan B, alternative · Premium share \$1,416 · Low: out-of-pocket \$560, total \$1,976 · Middle: out-of-pocket \$1,600, total \$3,016 · High: out-of-pocket \$5,500, total \$6,916
- Plan C, alternative · Premium share \$1,188 · Low: out-of-pocket \$800, total \$1,238 · Middle: out-of-pocket \$3,570, total \$4,008 · High: out-of-pocket \$6,000, total \$6,438 · Employer account \$750 taken off each total

**WHAT THE RENEWAL CHANGES**

Plan A: Deductible single from \$1,000 to \$1,500; Deductible family from \$2,000 to \$3,000; Out-of-pocket max single from \$4,500 to \$5,000; Out-of-pocket max family from \$9,000 to \$10,000; Out-of-network from "40% after a separate \$2000 deductible" to "40% after a separate \$3000 deductible". Employee only premium from \$620.00 to \$688.00 (+11.0%); Employee + one premium from \$1,302.00 to \$1,445.00 (+11.0%); Family premium from \$1,798.00 to \$1,996.00 (+11.0%). Total premiums for the year at today's enrollment from \$363,072 to \$402,972 (+\$39,900, +11.0%). FLAG: above the renewal threshold of 10%.

**QUESTIONS FOR THE BROKER**

1. Plan B, alternative: the family out-of-pocket maximum is not stated in the documents (plan list). What is it?
2. Plan A, renewal: total premiums for the year at today's enrollment rise from \$363,072 to \$402,972, up \$39,900 or 11.0%, above the renewal threshold of 10% (settings). The single deductible also rises from \$1,000 to \$1,500 and the single out-of-pocket maximum from \$4,500 to \$5,000 (plan list). What is behind the increase?
3. B1 says Insurer X will hold the rise at 8% if Plan A's single deductible moves to \$2,000, but those terms are not in the plan list or the premium list. Can you send them in full, with the family deductible, both out-of-pocket maximums and the premium for each tier, so they can be compared as another option?
4. B5 says each plan has its own drug list; none was supplied. Can you send the drug lists for Plans A, B and C?
5. N1 says almost all staff live within 20 miles of the office, and no broker note says how far either network reaches. How many in-network primary care doctors and hospitals do the Insurer X broad network (Plan A, renewal, and Plan C, alternative) and the Insurer Y regional network (Plan B, alternative) each have within 20 miles of the office?
6. N2 says several families on the team use the children's hospital downtown, which is in the current network. B2 says it is in Plan B's network; no broker note says whether it stays in the Insurer X broad network that Plan A, renewal, and Plan C, alternative, use (B3). Is it in that network for next year?
7. B6 says the rates assume at least 70% of eligible employees enroll; 30 of 38 employees are enrolled today, 78.9% (enrollment list, settings). How does each insurer count eligible employees, and does the condition apply to all three plans?

**POINTS FOR THE OWNER**

1. Plan A, renewal: the company total of \$246,068 is over the budget of \$235,000 by \$11,068 (settings). Which should move: the plan, the company's contribution or the budget?
2. Plan C, alternative: the employer account of \$750 a year for each enrolled employee is marked proposed (settings). At today's enrollment it costs \$22,500, included in Plan C's company total of \$199,548. Is the contribution decided at that amount?
3. Plan B, alternative, is an HMO where Plan A, current, is a PPO: a specialist visit needs a referral, out-of-network care is covered only in an emergency (plan list), and the university medical center is not in its network while the children's hospital downtown is (B2), which several families use (N2). Does the company want to offer Plan B?
4. Plan C, alternative, is a high-deductible plan where Plan A, current, is a PPO. It uses the same network as Plan A (B3), and primary care, specialist visits and generic drugs are paid after the deductible (plan list). Does the company want to offer Plan C?

**ASSUMPTIONS**

- Every employee enrolled today takes the option, at today's tier.
- Premiums: monthly figures times 12. Company shares: Employee only 80%; Employee + one 50%; Family 50% (contribution list).
- Typical employee: employee-only cover, in-network care only, spending of \$800, \$6,000 and \$40,000 a year (settings), through the deductible, then coinsurance, up to the out-of-pocket maximum.
- Copays: shown under Plan design for Plan A, renewal and Plan B, alternative, not counted in the totals; a copay charged before the deductible means a low user may pay less than shown.
- Employer account: \$750 a year for each enrolled employee on Plan C, alternative, proposed, taken off the typical employee's total in full, with no tax effect counted.
- Rounding: monthly premiums and shares to the cent, other amounts to the whole dollar.

**ALSO NOTED**

- B4: quotes are valid until 1 December 2026; the decision is needed by then for a 1 January start.
- N4: the owner wants to keep paying 80% of employee-only cover and half of the other tiers, whichever plan is chosen.

Draft for the Owner's decision. It compares plans from the documents supplied and gives no advice on insurance, tax or the law. It says nothing about which plan any employee should choose. No quote has been accepted, no application signed, no one enrolled, nothing sent or paid, and no payroll or record changed.

## How the figures were worked

So that every figure can be checked against the inputs:

- Plan A, renewal, for the company: employee only 18 × \$688 × 80% = \$9,907.20 a month; employee + one 5 × \$1,445 × 50% = \$3,612.50; family 7 × \$1,996 × 50% = \$6,986. Together \$20,505.70 a month, \$246,068.40 a year. Total premiums: (18 × \$688 + 5 × \$1,445 + 7 × \$1,996) × 12 = \$33,581 × 12 = \$402,972.
- This year's Plan A, worked the same way at today's enrollment: \$18,476 a month to the company, \$221,712 a year; \$30,256 a month in premiums, \$363,072 a year.
- Plan C: company share \$14,754 a month, \$177,048 a year, plus \$750 × 30 enrolled = \$22,500, giving \$199,548.
- Against this year: \$246,068.40 − \$221,712 = \$24,356.40, which is 11.0% of \$221,712. Against the budget: \$246,068.40 − \$235,000 = \$11,068.40.
- Typical employee on Plan B at middle use: \$500 deductible + 20% × (\$6,000 − \$500) = \$1,600 out-of-pocket, plus \$118 × 12 = \$1,416 premium share: \$3,016. At high use, \$500 + 20% × \$39,500 = \$8,400, capped at the \$5,500 maximum: \$6,916.
- Typical employee on Plan C at middle use: \$3,300 + 10% × \$2,700 = \$3,570, plus \$1,188, less the \$750 account: \$4,008. At low use, the \$800 is all under the deductible: \$800 + \$1,188 − \$750 = \$1,238.
- Lowest cost to a typical employee: at low use Plan C, alternative, \$1,238 (Plan B \$1,976, Plan A, renewal \$2,451); at middle use Plan B, alternative, \$3,016 (Plan C \$4,008, Plan A, renewal \$4,051); at high use Plan C, alternative, \$6,438 (Plan A, renewal \$6,651, Plan B \$6,916).
- Renewal premiums: \$68 on \$620 is 11.0%; \$143 on \$1,302 is 11.0%; \$198 on \$1,798 is 11.0%. Total premiums: \$39,900 on \$363,072 is 11.0%.
- Enrollment share: 30 ÷ 38 = 78.9%.
