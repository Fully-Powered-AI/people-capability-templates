# Exit interview themes summary: an invented example

*Illustrative example with invented data.* The company, the teams, the leavers, their words and the dates below are all invented. The company is an invented 120-person software company with Customer Support, Engineering, Product, Sales and Finance teams. Its HR lead runs the summary for the third quarter of 2026. First come the inputs the HR lead supplied (last period's summary as the extract that was supplied, which is all the summary uses), then the summary the workflow template returned.

## The inputs

### 1. Settings

```
Period: 1 July to 30 September 2026
Today: Monday 5 October 2026
Leaving types in scope: Resigned
Smallest group: 5
Smallest count: 2
Quotes per theme: 2
Question threshold: 3
Theme list: we have none of our own
Reason mapping: not set
```

### 2. Leaver list (exported from the HR system)

```
Leaver ref,Team,Leaving date,Leaving type,Recorded reason
L-01,Customer Support,2026-07-10,Resigned,Career move
L-02,Customer Support,2026-07-24,Resigned,Better pay elsewhere
L-03,Engineering,2026-07-31,Resigned,Career move
L-04,Customer Support,2026-08-07,Resigned,Personal reasons
L-05,Sales,2026-08-14,Resigned,Better pay elsewhere
L-06,Customer Support,2026-08-21,Resigned,Career move
L-07,Engineering,2026-08-28,Resigned,Relocation
L-08,Customer Support,2026-09-04,Resigned,Career move
L-09,Customer Support,2026-09-11,Resigned,Not stated
L-10,Product,2026-09-18,Resigned,Career move
L-11,Engineering,2026-09-25,Resigned,Work-life balance
L-12,Customer Support,2026-09-30,Fixed term ended,End of contract
L-13,Sales,2026-08-31,Company decision,Not stated
```

### 3. Exit interview notes

```
Leaver ref: L-01
Interviewed by the HR lead, 8 July.
Joining a competitor as a team lead. Said the weekend rota had been changed
three times since the spring, each time with a week's notice. Said:
"Nobody ever told us what senior support even meant here."

Leaver ref: L-02
Interviewed by the Customer Support manager, 21 July.
Leaving for a role with a 12% higher salary.
Main reason in their words: "I was doing two people's work since March."
Said they enjoyed the team and would miss their colleagues.

Leaver ref: L-04
Interviewed by the HR lead, 4 August.
Moving abroad with their partner.
Main reason in their words: "We're moving abroad for my partner's work."
Also mentioned recovering from an operation earlier this year, and said the
weekend rota made it hard to keep the follow-up appointments.

Leaver ref: L-05
Interviewed by the HR lead, 11 August.
Joining Company R.
Main reason in their words: "The April commission change took a fifth off
my earnings."
Also said this year's targets were set without asking the team.

Leaver ref: L-06
Interviewed by the Customer Support manager, 18 August.
Going to a smaller company at the same level.
Main reason in their words: "There was always more work than people."
Said: "When two people left in spring we were told cover was coming and it
never came." Said they had not had a one-to-one since March.

Leaver ref: L-08
Interviewed by the HR lead, 1 September.
Moving into an operations role at a logistics company.
Main reason in their words: "Every other weekend on the rota, and the queue
never got shorter."
Said they reported a customer who was abusive on calls in July and heard
nothing back.

Leaver ref: L-10
Interviewed by the HR lead, 15 September.
Joining a larger company as a senior product manager.
Main reason in their words: "There was no next step for me here."
Said the reorganisation in May left them unsure who decides the roadmap.

Leaver ref: L-11
Interviewed by the Engineering manager, 22 September.
Taking a role at another company.
Main reason in their words: "On-call every third week was too much on top
of everything else."
Said the on-call rota grew after two engineers left.
```

### 4. Leaver forms (exported from the exit survey)

```
Leaver ref,Main reason,Would recommend,Comments
L-01,Moving to a team lead role elsewhere,Unsure,"The weekend rota made it hard to plan anything. I'd have stayed for a path to senior."
L-02,The hours,No,"Covering two queues for most of the year after Person M left. The pay rise elsewhere was nice but I'd have stayed for normal hours."
L-03,No route to staff engineer,Yes,"Great colleagues. After the reorganisation in May nobody could tell me what the senior track looks like now."
L-05,Commission plan,Unsure,"The new commission plan in April cut what I could earn on renewals."
L-06,Too much work for too long,No,"Queues have been over target every week since the spring. My manager tried but couldn't get us cover."
L-07,Moving to another city,Yes,"Would have stayed if remote was allowed. The office-first policy from June ruled it out."
L-08,Workload,Unsure,"Weekend rota every other week since June."
L-10,Wanted to lead a product area,Yes,"Decisions about the roadmap changed every quarter after the reorganisation."
```

### 5. Last period's summary (the extract supplied, with the HR lead's marks)

```
EXIT INTERVIEW THEMES SUMMARY: 1 April to 30 June 2026
With an exit record: 7.
Themes: Pay and benefits, raised by 3. Career growth, raised by 3.
Workload and hours, raised by 2. Personal circumstances, raised by 2.
Questions for leadership:
1. Pay and benefits. When is the next pay review?
   [HR lead: answered at the July leadership meeting]
2. Career growth. What path is there from support to senior support, and
   is it written down? [HR lead: open]
```

## The summary the workflow template returned

```
EXIT INTERVIEW THEMES SUMMARY: 1 July to 30 September 2026

For: HR lead. Status: draft for the HR lead's approval before anyone else reads it.
Prepared: Monday 5 October 2026, from the leaver list (13 rows), 8 exit notes, 8 leaver forms, last period's summary.
Settings: smallest group 5, smallest count 2, quotes per theme 2, question threshold 3, leaving types Resigned. Defaults used for: the starter theme list, and a proposed reason mapping.
Anonymity: no group under 5 leavers with an exit record is shown, small teams are combined or the team view withheld, no theme raised by fewer than 2 leavers is named, and no quote carries a name, team, role or personal detail.

1. Coverage
Leavers in the period: 13. In scope (Resigned): 11. Out of scope: 2 (Fixed term ended 1, Company decision 1).
With an exit record: 10 of 11 (6 note and form, 2 note only, 2 form only). No exit record: 1.
All records matched.

2. Themes (raised by, of 10 leavers with an exit record)
Workload and hours: raised by 6; main reason for 4; recorded as the reason for 1.
  "The weekend rota made it hard to plan anything."
  "Covering two queues for most of the year after [a colleague] left."
Career growth: raised by 3; main reason for 3; recorded as the reason for 5.
  "I'd have stayed for a path to senior."
  "After the reorganisation in May nobody could tell me what the senior track looks like now."
Company direction and change: raised by 3; main reason for 0; recorded as the reason for 0.
  "Decisions about [our plans] changed every quarter after the reorganisation."
Personal circumstances: raised by 2; main reason for 2; recorded as the reason for 2.
  Not quoted: personal circumstances are counted, never quoted.
Pay and benefits: raised by 2; main reason for 1; recorded as the reason for 2.
  "The pay rise elsewhere was nice but I'd have stayed for normal hours."
  Withheld: 2 comments that could not be made anonymous.
Other: 2 topics raised by one leaver each, named in the HR note only.
Main reason not stated: 0.

3. What leavers said beside what was recorded
Recorded at the time: Workload and hours 1, Career growth 5, Personal circumstances 2, Pay and benefits 2, not stated 0.
Leavers' own main reasons: Workload and hours 4, Career growth 3, Personal circumstances 2, Pay and benefits 1, not stated 0.
Compared: 10. Same theme: 7. Different: 3.
Recorded as Career growth, main reason Workload and hours: 2. Other differences: 1.
Reason mapping proposed, for the HR lead to confirm: Career move → Career growth; Better pay elsewhere → Pay and benefits; Personal reasons → Personal circumstances; Relocation → Personal circumstances; Work-life balance → Workload and hours; Not stated → not stated.

4. By team (leavers with an exit record)
Customer Support: 6 in scope, 5 with an exit record. Raised by 2 or more: Workload and hours 5.
Engineering, Product and Sales (combined): 5 in scope, 5 with an exit record. Raised by 2 or more: Career growth 2; Company direction and change 3.
Teams combined because each had fewer than 5: Engineering, Product, Sales.

5. Recommend and spoken well of
Would recommend working here: Yes 3, Unsure 3, No 2, of 8 forms.
Spoken well of: Team and colleagues 2.

6. Since last period
Workload and hours: 2 of 7 then, 6 of 10 now.
Career growth: 3 of 7 then, 3 of 10 now.
Company direction and change: not shown last period, 3 of 10 now.
Personal circumstances: 2 of 7 then, 2 of 10 now.
Pay and benefits: 3 of 7 then, 2 of 10 now.

7. Questions for leadership
1. Workload and hours. Raised by 6 of 10 leavers and the main reason for 4; recorded as the reason for 1. In Customer Support, all 5 leavers with an exit record raised it. What does leadership know about staffing, cover and rotas in Customer Support?
2. Career growth. Raised by 3 of 10 and the main reason for 3; recorded as the reason for 5. How would someone here find a route to a more senior role?
3. Company direction and change. Raised by 3 of 10, all in Engineering, Product and Sales (combined), and the main reason for none. How were recent changes in those teams decided and explained to the people in them?
4. Recorded reasons. For 3 of 10, the reason recorded at the time is in a different theme from the leaver's own main reason; for 2 recorded as Career growth, the leaver gave Workload and hours. How is the leaving reason recorded at the time, and by whom?
Carried from last period: Career growth. What path is there from support to senior support, and is it written down? (open). Answered, not carried: 1.

Left out: names of people and companies; where leavers are going and what they were offered; health and family detail. Matters passed to the HR lead outside this summary: 1.
This summary decides nothing about any person and names no one.

NOTE FOR THE HR LEAD ONLY: remove before sharing
Matters for your own process: L-08: a report of abuse by a customer.
Topics raised by one leaver: Manager (L-06). Flexibility and place of work (L-07).
Quotes withheld: L-05, Pay and benefits: 2, each with more than one identifying detail: a pay arrangement that points to a team smaller than 5, with a kind of work in one and the leaver's own pay change in the other.
Words replaced in quotes: L-02: a colleague's name replaced with [a colleague]. L-10: a word that points to a team smaller than 5 replaced with [our plans].
Main reasons that differ between form and note: None.
Records not used: None.
No exit record: L-09.
To confirm: the proposed reason mapping; the default theme list.
```

## How the figures were reached

- **Coverage.** Thirteen rows, all dated inside the period. L-12 and L-13 are out of scope by leaving type. Of the eleven resignations, L-01, L-02, L-05, L-06, L-08 and L-10 have a note and a form, L-04 and L-11 a note only, L-03 and L-07 a form only, and L-09 neither: 6 + 2 + 2 = 10 with an exit record.
- **Themes raised.** Workload and hours: L-01, L-02, L-04, L-06, L-08, L-11 (6). Career growth: L-01, L-03, L-10 (3). Company direction and change: L-03, L-05, L-10 (3). Personal circumstances: L-04, L-07 (2). Pay and benefits: L-02, L-05 (2). Remarks the leaver raised in the exit conversation count as pushes to leave (L-04's rota, L-05's targets, L-06's missing one-to-ones, L-10's reorganisation). Manager: L-06 only, and Flexibility and place of work: L-07 only, so both go under Other. Some codings are judgement calls a reader could make differently: L-05's targets set without asking the team could be Manager; L-07's office-first policy is coded to Flexibility only, and coding it also to Company direction and change would make that theme 4; L-01's rota changed three times is coded to Workload and hours only. None changes a rule, and the HR lead can recode. Career growth and Company direction tie at 3; Career growth has 3 main reasons to none, so it comes first. Personal circumstances and Pay tie at 2; Personal has 2 main reasons to 1.
- **Main reasons.** From the forms where there is one, otherwise the note's line. Workload and hours: L-02, L-06, L-08, L-11 (4). Career growth: L-01, L-03, L-10 (3). Personal circumstances: L-04, L-07 (2). Pay and benefits: L-05 (1). 4 + 3 + 2 + 1 = 10.
- **Recorded reasons, for the ten.** Career growth: L-01, L-03, L-06, L-08, L-10 (5). Pay and benefits: L-02, L-05 (2). Personal circumstances: L-04, L-07 (2). Workload and hours: L-11 (1). 5 + 2 + 2 + 1 = 10. Different from the main reason: L-02 (Pay, said workload), L-06 and L-08 (Career growth, said workload). The pairing shared by two is shown; L-02's falls under Other differences.
- **Teams.** Customer Support has five leavers with an exit record (L-09 has none), so it stands alone. Engineering (3), Product (1) and Sales (1) are each under five and combine to five. Workload and hours: all five in Customer Support. In the combined group, Career growth: L-03, L-10 (2); Company direction and change: L-03, L-05, L-10 (3).
- **Forms.** Yes: L-03, L-07, L-10. Unsure: L-01, L-05, L-08. No: L-02, L-06. 3 + 3 + 2 = 8. Team and colleagues spoken well of by L-02 (note) and L-03 (form).
- **Quotes.** Workload: the first usable sentence from L-01, then L-02's first sentence with the name replaced. Career growth: L-01's second sentence, then L-03's second. Company direction: L-03's sentence is coded to Career growth only, being first in the theme list, so it was never a candidate here; L-05 has none in their own words, and L-10's sentence is used with "the roadmap" replaced, because it points to a team of one. Pay: L-02's second sentence, which names both pay and hours and so goes to Pay, the theme first in the list. It is the closest call among the quotes: it says a pay rise was offered but gives no figure and no employer, so it carries no identifying detail under the rule; L-05's two Pay candidates, the form sentence and the quotation on the note's main reason line, are both withheld because "commission" points to a team of one and each carries a second detail.
- **Questions.** Workload (6), Career growth (3) and Company direction (3) reach the threshold of 3; Personal circumstances and Pay (2 each) do not. One pairing is shown, so a fourth question asks about recorded reasons.
