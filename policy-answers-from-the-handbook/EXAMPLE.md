# Policy answers from the handbook: an invented example

*Illustrative example with invented data.* The company, its handbook, its memo, its staff and their questions are all invented. The company is an invented 140-person food wholesaler with a head office and a depot. Its office manager handles HR administration and answers staff questions; its HR manager decides anything the handbook does not settle. First come the inputs the office manager supplied, in full, then the answers the workflow template returned.

## The inputs

### 1. Company settings

```
Today: Monday 12 October 2026
Run by: Office manager
HR contact for referrals: HR manager
Employee groups the handbook uses: full-time, part-time; office staff,
  depot staff
Locations: head office; depot
Policy memos: a memo counts as current only when it says which handbook
  section it replaces. Otherwise quote both and refer.
Topics always referred and topics raised the same day: the defaults.
Replies signed: Office manager
```

### 2. The handbook (the whole document)

```
STAFF HANDBOOK. Version 3, effective 1 January 2025.

1 About this handbook
1.1 This handbook applies to all employees of the company unless a
section says otherwise.
1.2 Where this handbook refers to your manager, it means the person you
report to day to day.

2 Hours and working pattern
2.1 Office staff work 37.5 hours a week, Monday to Friday.
2.2 Depot staff work the shift pattern set by the depot rota, published
two weeks ahead.

3 Annual leave
3.1 Full-time staff receive 25 days of annual leave per leave year, plus
public holidays. Part-time staff receive a pro-rata amount based on their
contracted hours.
3.2 The leave year runs from 1 January to 31 December.
3.3 Requests for five or more consecutive working days must be made at
least four weeks before the first day of leave.
3.4 Requests for leave in July and August are considered in the order
they are received from 1 March. Depot requests are also subject to the
minimum staffing level on the depot rota.
3.5 Full-time staff may carry up to five days of unused annual leave into
the next leave year. Carried days must be taken by 31 March, after which
they are lost.

4 Parental leave
4.1 Employees with at least 12 months' continuous service at the start of
their leave receive six weeks of parental leave at full pay.
4.2 Any further parental leave is unpaid and is provided in line with the
law.
4.3 Tell the HR manager in writing at least 15 weeks before the expected
week of birth or placement.

5 Working from home
5.1 Office staff may work from home up to two days a week with their
manager's agreement.
5.2 In this section, home means the address held for you in the HR
system.
5.3 Depot roles cannot be done from home.

6 Expenses
6.1 Business expenses are reimbursed when claimed within 30 days with
receipts.
6.2 Business mileage in a personal car is reimbursed at 60 cents per
mile.
6.3 Travel between home and your normal place of work is not business
mileage.

7 Raising a concern
7.1 If you are treated unfairly, harassed or bullied at work, or have a
concern about safety, raise it with your manager or, if you prefer,
directly with the HR manager.
7.2 You can raise a concern in confidence. The company will not tolerate
anyone being treated badly for raising a concern in good faith.
```

### 3. The policy memo in force

```
FINANCE MEMO: Mileage rate. 1 September 2026.
From 1 October 2026, business mileage in a personal car is paid at 67
cents per mile. Claims for journeys before 1 October use the old rate.
```

### 4. The question export (names removed before it was supplied)

```
question_id,received,employee_group,location,question
Q1,2026-10-05,full-time office,head office,How far ahead do I need to book two weeks off in August next year?
Q2,2026-10-06,part-time depot,depot,Can I carry my unused holiday into next year? I'm part-time.
Q3,2026-10-07,full-time office,head office,Can I work from my parents' house in Spain for two weeks in September?
Q4,2026-10-08,full-time depot,depot,I've been here 11 months and my partner is due in March. How much paid parental leave will I get?
Q5,2026-10-08,full-time office,head office,Is mileage still paid at 60 cents a mile?
Q6,2026-10-09,part-time office,head office,Who do I talk to if my supervisor keeps making comments about my age?
```

## The output

```
POLICY ANSWERS: 6 questions, prepared Monday 12 October 2026

For: Office manager. HR contact for referrals: HR manager.
Documents read: Staff handbook, version 3, effective 1 January 2025, whole document; Finance memo: Mileage rate, issued 1 September 2026, effective 1 October 2026, whole document.
Questions: 6 from the question export. Answered 1 · Partly answered 1 · Handbook silent 1 · Referred to HR 2 · Conflict 1.
Raise today: Q6, a concern about a supervisor's comments.

Q1. "How far ahead do I need to book two weeks off in August next year?"
Asked by: full-time office, head office. Received 5 October 2026.
Status: ANSWERED
Short answer: Reading two weeks off as five or more consecutive working days: the request is due at least four weeks before the first day of leave, and requests for July and August are considered in the order they are received from 1 March.
What the handbook says:
- "Requests for five or more consecutive working days must be made at least four weeks before the first day of leave." (Staff handbook, section 3.3, Annual leave)
- "Requests for leave in July and August are considered in the order they are received from 1 March." (Staff handbook, section 3.4, Annual leave)
Conditions and exceptions in the text: depot requests are also subject to the minimum staffing level on the depot rota (section 3.4).
Applies to: the text names no group; section 1.1 applies it to all staff. The depot condition in section 3.4 does not cover this asker, who is at head office.
Not covered: nothing
Looked under: 1 About this handbook; 3 Annual leave.
For the HR contact: nothing to decide
Reply for the employee, for Office manager to review and send:
Hi, thanks for your question. Taking two weeks off as five or more consecutive working days, the handbook asks for your request at least four weeks before your first day of leave: "Requests for five or more consecutive working days must be made at least four weeks before the first day of leave." (staff handbook, section 3.3). For August, requests for July and August are considered in the order they are received from 1 March (section 3.4).
Office manager

Q2. "Can I carry my unused holiday into next year? I'm part-time."
Asked by: part-time depot, depot. Received 6 October 2026.
Status: PARTLY ANSWERED
Short answer: Full-time staff may carry up to five unused days into the next leave year, to be taken by 31 March. The handbook does not say whether part-time staff may carry any over.
What the handbook says:
- "Full-time staff may carry up to five days of unused annual leave into the next leave year. Carried days must be taken by 31 March, after which they are lost." (Staff handbook, section 3.5, Annual leave)
- "The leave year runs from 1 January to 31 December." (Staff handbook, section 3.2, Annual leave)
Conditions and exceptions in the text: carried days must be taken by 31 March and are lost after that (section 3.5).
Applies to: section 3.5 names full-time staff only. The asker is part-time, so it does not answer for them.
Not covered: whether part-time staff may carry unused leave into the next leave year, and how much.
Looked under: 1 About this handbook; 3 Annual leave, sections 3.1 to 3.5.
For the HR contact: Decide whether part-time staff may carry unused leave into the next leave year, and how much. Section 3.5 names full-time staff only; section 3.1 gives part-time staff a pro-rata amount and says nothing about carrying it over.
Reply for the employee, for Office manager to review and send:
Hi, thanks for asking. The handbook's carry-over rule is written for full-time staff: "Full-time staff may carry up to five days of unused annual leave into the next leave year. Carried days must be taken by 31 March, after which they are lost." (staff handbook, section 3.5). It does not say how this works for part-time staff, so I am asking the HR manager to confirm, and I will come back to you.
Office manager

Q3. "Can I work from my parents' house in Spain for two weeks in September?"
Asked by: full-time office, head office. Received 7 October 2026.
Status: HANDBOOK SILENT
Short answer: The handbook does not cover this.
What the handbook says:
- Nothing found. Nearest passage: "Office staff may work from home up to two days a week with their manager's agreement." and "In this section, home means the address held for you in the HR system." (Staff handbook, sections 5.1 and 5.2, Working from home), which covers working from the address held in the HR system, not from any other address or from another country.
Conditions and exceptions in the text: none stated for working away from home.
Applies to: sections 5.1 and 5.2 name office staff, and the asker is office staff, but the passage covers the home address only.
Not covered: working from an address other than the one held in the HR system, and working from another country.
Looked under: 1 About this handbook; 2 Hours and working pattern; 5 Working from home; 6 Expenses.
For the HR contact: Decide whether office staff may work from another address or from another country, for how long and on what terms. The handbook covers the home address held in the HR system only.
Reply for the employee, for Office manager to review and send:
Hi, thanks for asking. The handbook covers working from home, meaning the address we hold for you, but it does not cover working from another address or from abroad. I am asking the HR manager to confirm, and I will come back to you.
Office manager

Q4. Question not repeated: it carries health or family details. See Q4 in the questions supplied.
Asked by: full-time depot, depot. Received 8 October 2026.
Status: REFER TO HR
Short answer: The general rule is in section 4.1. Whether it applies to this employee turns on their service at the start of their leave, which the HR contact confirms.
What the handbook says:
- "Employees with at least 12 months' continuous service at the start of their leave receive six weeks of parental leave at full pay." (Staff handbook, section 4.1, Parental leave)
- "Any further parental leave is unpaid and is provided in line with the law." (Staff handbook, section 4.2, Parental leave)
- "Tell the HR manager in writing at least 15 weeks before the expected week of birth or placement." (Staff handbook, section 4.3, Parental leave)
Conditions and exceptions in the text: at least 12 months' continuous service at the start of the leave (section 4.1); written notice to the HR manager at least 15 weeks before the expected week of birth or placement (section 4.3).
Applies to: the text names no group; section 1.1 applies it to all staff.
Not covered: section 4.2 refers to the law for further unpaid leave and does not state the rule itself. No view is given on it.
Looked under: 1 About this handbook; 4 Parental leave.
For the HR contact: A question about one person's own parental leave, which turns on their service at the start of their leave. Confirm what applies to them, and answer the part about further unpaid leave, which section 4.2 leaves to the law. No date or figure has been worked out for them.
Reply for the employee, for Office manager to review and send:
Hi, thanks for your question. The general rule is in section 4.1 of the staff handbook: "Employees with at least 12 months' continuous service at the start of their leave receive six weeks of parental leave at full pay." Section 4.3 also asks you to "Tell the HR manager in writing at least 15 weeks before the expected week of birth or placement." I have passed your question to the HR manager, who will confirm what applies to you.
Office manager

Q5. "Is mileage still paid at 60 cents a mile?"
Asked by: full-time office, head office. Received 8 October 2026.
Status: CONFLICT
Short answer: The handbook and a later finance memo give different rates, and the memo does not say which section it replaces. The HR contact confirms which is current.
What the handbook says:
- "Business mileage in a personal car is reimbursed at 60 cents per mile." (Staff handbook, section 6.2, Expenses)
- "From 1 October 2026, business mileage in a personal car is paid at 67 cents per mile. Claims for journeys before 1 October use the old rate." (Finance memo: Mileage rate, 1 September 2026, no numbered sections)
Conditions and exceptions in the text: expenses are reimbursed when claimed within 30 days with receipts (section 6.1); travel between home and the normal place of work is not business mileage (section 6.3); the memo's rate starts on 1 October 2026, and journeys before then use the old rate (memo).
Applies to: the text names no group; section 1.1 applies it to all staff. Finance memo: Mileage rate names no group.
Not covered: which of the two rates is current.
Looked under: 1 About this handbook; 6 Expenses; Finance memo: Mileage rate.
For the HR contact: Confirm whether the finance memo of 1 September 2026 replaces section 6.2 of the staff handbook. The memo does not say which section it replaces, and the settings count a memo as current only when it does.
Reply for the employee, for Office manager to review and send:
Hi, thanks for asking. The staff handbook and a finance memo from September give different mileage rates, so I am asking the HR manager to confirm which applies, and I will come back to you.
Office manager

Q6. "Who do I talk to if my supervisor keeps making comments about my age?"
Asked by: part-time office, head office. Received 9 October 2026.
Status: REFER TO HR
Short answer: The handbook's route is the employee's manager or, if they prefer, the HR manager, in confidence. The concern itself goes to the HR contact today.
What the handbook says:
- "If you are treated unfairly, harassed or bullied at work, or have a concern about safety, raise it with your manager or, if you prefer, directly with the HR manager." (Staff handbook, section 7.1, Raising a concern)
- "You can raise a concern in confidence." (Staff handbook, section 7.2, Raising a concern)
Conditions and exceptions in the text: none stated
Applies to: the text names no group; section 1.1 applies it to all staff.
Not covered: the concern itself, which is for the HR contact.
Looked under: 1 About this handbook; 7 Raising a concern.
For the HR contact: A concern about a supervisor's repeated comments about an employee's age, listed under Raise today. Decide today how to respond to the employee. The handbook's route runs through the employee's manager, who may be the supervisor concerned, so the reply leads with the HR manager. No details beyond the question are recorded here, and no view is given on the concern.
Reply for the employee, for Office manager to review and send:
Hi, thank you for telling me. You can raise this directly with the HR manager, and you can do so in confidence (staff handbook, sections 7.1 and 7.2). The handbook also names your manager as a route. If you would like, I can put you in touch with the HR manager.
Office manager

Gaps for the HR contact: whether part-time staff may carry unused leave into the next leave year (Q2); working from an address other than home, including from another country (Q3).
Conflicts between documents: Q5: Finance memo: Mileage rate, 1 September 2026, against Staff handbook, section 6.2.
Quotes checked word for word against the documents supplied: all match.

Draft for Office manager to review. Nothing has been sent, no request approved and no record changed.
```

Every answer above traces to the handbook, the memo, the settings and the question export shown here. The office manager reads and edits each reply before sending it; the HR manager takes Q2, Q3, Q4, Q5 and Q6.
