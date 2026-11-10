# Training needs analysis: one run on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-10

The inputs are the invented example in [`example.md`](example.md): the scope brief, the requirements list, the coverage list, the eight notes and the settings, as printed there. No client data was used.

This is the third run. The first, on 9 November 2026 with Claude Sonnet 5.5, was done by an assistant that had not written the template; it matched the then-published example in every figure and found ambiguities that a review confirmed. Its output is not published. The template was revised after it (among other things: done-by dates taken from the scope brief or the notes, the pasted instructions given the rules the procedure already had, an absence named as a personal detail, a reason for a zero count accepted as evidence, a vendor's session treated as an outside course, and a question asking whether a course brings people to the level needed). A second run the same day, by the assistant that made those revisions, was recorded here and passed an independent review, which raised minor points. The template was revised again after that review: a start or leaving date is now a personal detail; a role of one or two people keeps Read by to the approver and the team manager, and its single-holder line carries no note; a new question asks whether the one person who can teach an in-house item has the time; Short is never more than Needed when there are more expiry dates than people at level; and the pasted instructions now carry the coverage-list definitions and the exception for a note left out entirely.

This run was done by the assistant that made the second set of revisions, which had read the earlier runs, the review and the published example before it ran. It is therefore not an independent run. It followed the revised instruction block and output format on the example's inputs only, produced the analysis below, and the published example's output was then brought into line with it.

## What came out

```
TRAINING NEEDS ANALYSIS: Service team

For: HR lead. Run by: Service manager. Prepared: 9 November 2026. Horizon: 30 April 2027. Why now: the new scheduling and dispatch system goes live on 1 February 2027, and repeat visits are up.
From: requirements list (8 rows), coverage list (8 rows), manager's notes (8 notes), settings; defaults used: level scale.
Read by: HR lead and Service manager.
Roles: Service coordinator (4 people); Field technician (6 people); Parts clerk (2 people). Abilities: 8. Shortfalls: 7 (1 required by a rule). Single holders: 2. Training items: 6. Questions: 7.
Left out: a person's name (note 3); an absence (note 3); a start date (note 6); a health detail (note 8).

ROLE BY ABILITY
Levels: 1 Knows what it is · 2 Does it with help · 3 Does it alone · 4 Can teach it

Service coordinator (4 people)
- Book and reschedule jobs in the new scheduling system · Essential · Level 3 · Needed 4 · At level now 0 · Expiring by 30 April 2027: none · Short 4 · Evidence: System not live yet
- Find the likely fault by phone before booking a visit · Important · Level 3 · Needed 2 · At level now 1 · Expiring by 30 April 2027: none · Short 1 · Evidence: Manager observation · FLAG: check first
- Handle a warranty claim from start to finish · Essential · Level 3 · Needed 2 · At level now 1 · Expiring by 30 April 2027: none · Short 1 · Evidence: Training record · FLAG: single holder

Field technician (6 people)
- Refrigerant handling certificate · Essential · Level 3 · Needed 6 · At level now 6 · Expiring by 30 April 2027: 2 · Short 2 · Evidence: Certificate register · Required by: Manufacturer warranty terms
- Use the job app in the new scheduling system · Essential · Level 3 · Needed 6 · At level now 0 · Expiring by 30 April 2027: none · Short 6 · Evidence: System not live yet
- Repair induction hobs · Important · Level 3 · Needed 3 · At level now 2 · Expiring by 30 April 2027: none · Short 1 · Evidence: Repeat-visit log

Parts clerk (2 people)
- Order parts through the two main distributors' portals · Essential · Level 3 · Needed 2 · At level now 1 · Expiring by 30 April 2027: none · Short 1 · Evidence: not evidenced · FLAG: single holder, not evidenced
- Run the monthly stock count · Useful · Level 2 · Needed 1 · At level now 2 · Expiring by 30 April 2027: none · Short 0 · Evidence: Training record

SHORTFALLS IN PRIORITY ORDER
1. Field technician, refrigerant handling certificate: short 2 of 6 by 30 April 2027. Why here: required by Manufacturer warranty terms. Closed by: Course that meets Manufacturer warranty terms (note 2: the training centre's one-day renewal course).
2. Field technician, use the job app in the new scheduling system: short 6 of 6. Why here: Essential. Closed by: Course (note 1: the vendor's session for technicians).
3. Service coordinator, book and reschedule jobs in the new scheduling system: short 4 of 4. Why here: Essential. Closed by: Course (note 1: the vendor's session for coordinators).
4. Service coordinator, handle a warranty claim from start to finish: short 1 of 2. Why here: Essential. Closed by: Taught in-house (coverage list: 1 can teach it).
5. Parts clerk, order parts through the two main distributors' portals: short 1 of 2. Why here: Essential. Closed by: Supervised practice (note 6).
6. Service coordinator, find the likely fault by phone before booking a visit: short 1 of 2. Why here: Important. Closed by: Check first (note 4).
7. Field technician, repair induction hobs: short 1 of 3. Why here: Important. Closed by: Taught in-house (coverage list: 1 can teach it).

SINGLE HOLDERS
- Service coordinator, handle a warranty claim from start to finish: one person at the level needed (note 3: warranty claims wait for that one person). Priority 4.
- Parts clerk, order parts through the two main distributors' portals: one person at the level needed. Priority 5.

CERTIFICATES RUNNING OUT BY 30 APRIL 2027
- Field technician, refrigerant handling certificate: 2 of 6 expire, on 18 December 2026 and 26 February 2027. Renew by 18 November 2026 and 27 January 2027. Priority 1.

CHECK BEFORE TRAINING
- Service coordinator, find the likely fault by phone before booking a visit: the call script still covers the old product range, not the induction hob and heat pump models sold since spring (note 4). See question 6.

TRAINING TO ARRANGE
T1 Refrigerant handling certificate: 2 field technicians to level 3. How: the training centre's one-day renewal course (note 2). Arranged by: HR lead. Done by: 18 November 2026 and 27 January 2027 (30 days before each certificate expires). Cost: 2 x $240 = $480. Closes priority 1; subject to question 1.
T2 Use the job app in the new scheduling system: 6 field technicians to level 3. How: the vendor's two-hour online session for technicians, one session of up to 8 (note 1). Arranged by: HR lead. Done by: 1 February 2027 (the system goes live, scope brief). Cost: 6 x $95 = $570. Closes priority 2; subject to question 2.
T3 Book and reschedule jobs in the new scheduling system: 4 service coordinators to level 3. How: the vendor's two-hour online session for coordinators, one session of up to 8 (note 1). Arranged by: HR lead. Done by: 1 February 2027 (the system goes live, scope brief). Cost: 4 x $95 = $380. Closes priority 3; subject to question 3.
T4 Handle a warranty claim from start to finish: 1 service coordinator to level 3. How: taught in-house by the person who can teach it (coverage list). Arranged by: Service manager. Done by: 30 April 2027 (horizon end). Cost: not supplied. Closes priority 4; subject to question 4.
T5 Order parts through the two main distributors' portals: 1 parts clerk to level 3. How: supervised practice placing orders (note 6). Arranged by: Service manager. Done by: 30 April 2027 (horizon end). Cost: not supplied. Closes priority 5; subject to question 5.
T6 Repair induction hobs: 1 field technician to level 3. How: taught in-house by the person who can teach it (coverage list). Arranged by: Service manager. Done by: 30 April 2027 (horizon end). Cost: not supplied. Closes priority 7; subject to question 7.
Who attends each item is the Service manager's choice.
Costs supplied: $1,430 for 3 items, against a budget of $3,000 (note 7). Items without a cost: 3.

QUESTIONS FOR THE HR LEAD
1. Priority 1: two field technicians' refrigerant handling certificates expire on 18 December 2026 and 26 February 2027 (coverage list), and the requirements list says the manufacturer warranty terms require the certificate. Note 2 names the training centre's one-day renewal course. Does that course meet the warranty terms? The first renewal is due by 18 November 2026.
2. Priority 2: note 1 describes the vendor's two-hour online session for technicians on the job app. The requirements list asks for level 3, Does it alone; the coverage list counts no one at that level, because the system is not live yet. Note 1 does not say what level the session brings people to. Does it bring the six technicians to level 3 by go-live on 1 February 2027 (scope brief), and if not, what follows it?
3. Priority 3: note 1 describes the vendor's two-hour online session for coordinators on booking and rescheduling. The requirements list asks for level 3, Does it alone; the coverage list counts no one at that level, because the system is not live yet. Note 1 does not say what level the session brings people to. Does it bring the four coordinators to level 3 by go-live on 1 February 2027 (scope brief), and if not, what follows it?
4. Priority 4: the coverage list counts one person in the team who can teach a warranty claim from start to finish, and T4 rests on that person. The inputs do not say how much time that person has. Can they teach one more coordinator to level 3 by 30 April 2027 (horizon end)?
5. Priority 5: the coverage list counts one parts clerk as placing distributor orders alone, with evidence given as "None". What supports that count?
6. Priority 6: note 4 says the coordinators cannot find the likely fault by phone because the call script still covers the old product range. Should the script be updated before anyone is trained, and who updates it?
7. Priority 7: the coverage list counts one person in the team who can teach induction hob repairs, and T6 rests on that person. The inputs do not say how much time that person has. Can they teach one more field technician to level 3 by 30 April 2027 (horizon end)?

ALSO NOTED
- Note 5: repeat visits on induction hobs have gone up since the company started selling more of them (relates to priority 7).

Draft for the HR lead's approval. No one has been named, rated, enrolled or booked; nothing has been bought or sent; no record has been changed.
```

## What was observed

- **Every required part was produced.** All sections of the output format are present, every one of the eight rows in each list was matched once, and the header counts agree with the body: 8 abilities, 7 shortfalls (1 required by a rule), 2 single holders, 6 training items, 7 questions. Nothing in the inputs triggered a stop: three named roles, today's date given, default headers in both lists, no role and ability repeated, no sign-in details.
- **What the revisions changed in the output, compared with the second run:**
  - Questions rose from 5 to 7. T4 and T6, each taught in-house with one person who can teach it, are now subject to a question asking whether that person has the time by the done-by date. The second run had relied on the unstated inference that the person was free. The other questions were renumbered: the not-evidenced question is now 5 and the check-first question 6.
  - The Left out line now names the start date in note 6, which the second run neither repeated nor listed.
  - The Parts clerk role has two people, so its single-holder line carries no note. The second run had added what note 6 says about the other clerk.
  - The warranty-claims single-holder line now reads "warranty claims wait for that one person". The second run wrote "claims wait when that person is away", which restated the absence it had put on the Left out line.
  - Every other figure is the same as the second run: the shortfalls, the seven-item priority order, the two renewal dates (18 November 2026 and 27 January 2027), the six items, the costs ($480, $570, $380; $1,430 for three items against a $3,000 budget, three items without a cost).
- **Facts not in the inputs.** The output adds no figure or name. The two new questions do not say who the person who can teach is; the coverage list counts people in the team, which may include someone outside the role.
- **Where the template still left a judgment:**
  - Note 8 says a coordinator was off sick. It was named once on the Left out line as a health detail, not also as an absence.
  - Question 5 still concerns the one parts clerk counted at the level needed, in a role of two people. That is the count itself; Read by stays with the HR lead and the Service manager, as the settings already gave.
  - Two pairs tied on every rule up to the last (priorities 4 and 5; priorities 6 and 7). The order of the requirements list settled both, as in the second run.
  - Question 1 concerns a course that must meet a rule; the level question was not also asked for T1, because the template says that course has its own question.
- **Nothing was stopped for and nothing was declined,** because the example asks for nothing the template refuses. The refusal rules and the stop conditions, and the rules for unnumbered notes, sign-in details, per-session prices and more expiry dates than people at level, were not exercised by this run.
