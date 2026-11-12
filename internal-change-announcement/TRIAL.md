# Internal change announcement: a trial on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-10

This is one run of the workflow template on its own invented example. The inputs are the invented example's inputs (the Tallowmere Supply and Fenbrook Fixings example in [public/example.md](example.md)); no client data was used.

Earlier runs. A first run on 9 November, by Claude Sonnet 5.5 on the first version of the template, raised five questions as needing an answer from the decision owner. Two of them (why the change starts on 7 December, and who covers the purchasing approvals when someone is away) had no basis in the brief, and the drafted staff messages told people those points were "not settled yet". An independent review failed the template, and the rules for open questions, facts, settings, checks and the size line were revised. A second run the same day, by Claude Opus 5.5 on the revised template, produced a complete pack and passed an independent review with minor points: the rule did not say whether an open question "bears on a group" by the question's "asked by" list (that run's message to the purchasing team carried no note for a question about smaller orders, while the published example's did); that run's reminder carried the confirm-before-sending note where the published example carried a note to add the answer; its manager briefing asked the branch manager to send the reminder, an instruction the record did not list among phrases beyond the brief; and two edits made after that run had not been run again. The template now says which groups an open question bears on and which note a reminder carries; the instruction block now also says to confirm one change, one brief and one list, and to write "not stated" for a missing sender or channel; and the published example's invented ordering system was renamed Brindlestock and its question list given "What stays the same?". This record is of a fresh run on the edited template and replaces the earlier records.

How it was run: the instruction block from the member template, followed by its output format, was given as the system instructions of a new Claude Code session in print mode, with every tool switched off and Claude Code's own instructions replaced; the three inputs were pasted as the one message. Claude Code may also have added the general account notes it loads for every session; they say nothing about this task. That session had not seen the rest of the template or the published example's output. The person who set up the run had edited the template and the example beforehand.

## Inputs used

The three inputs listed under "The inputs" in [public/example.md](example.md): the company settings, the change brief and the audience list, in full. Nothing else was supplied.

## What came out

The assistant did not stop for anything. The inputs were complete, the headers matched, every row had a sender and a channel, the effective date was after the announcement date, the decision was final, and nothing in the change removes or creates a position or alters anyone's job, pay or hours. It produced every part of the output format. This is the full pack as returned.

```
INTERNAL CHANGE ANNOUNCEMENT: The Fenbrook branch keeps its stock and places and receives stock orders in Brindlestock from Monday 7 December 2026

For: People and operations coordinator. Decided by: Dana Okafor, operations director, Tallowmere. Announced Tuesday 17 November 2026; takes effect Monday 7 December 2026.
Prepared Monday 9 November 2026 from the change brief, the audience list (3 groups) and the settings, with defaults for the manager lead time (2 working days), reminder lead time (2 working days) and check-in delay (10 working days), as the settings ask, and for the briefing channel (email), which was not supplied.
Messages drafted: 6. Questions answered: 9. Answers needed: 2. Held out: 2. Checks: 4.
Scope: In scope: the change alters how work is done, and the brief states that "Nobody's job, pay or hours change" (F16). Held out: 2 items; see below.

THE FACTS
F1. From Monday 7 December 2026, the Fenbrook branch keeps its stock in Brindlestock, Tallowmere's ordering system.
F2. From Monday 7 December 2026, the Fenbrook branch places and receives stock orders in Brindlestock.
F3. Tallowmere bought Fenbrook in August.
F4. Since then, the two companies have kept stock records in different places.
F5. Tallowmere's depots cannot see Fenbrook's stock, and Fenbrook cannot see Tallowmere's.
F6. Customers are sometimes told an item is out of stock when the other company has it.
F7. One system lets both companies see all the stock.
F8. Fenbrook's order spreadsheet takes its last orders on Friday 4 December.
F9. Tallowmere's purchasing team approves branch orders over $2,500 in Brindlestock, instead of the branch manager.
F10. Tallowmere's purchasing team approves those orders within one working day.
F11. Tallowmere's depots see Fenbrook's stock in Brindlestock from 7 December.
F12. The branch team and its manager stay as they are.
F13. The counter stays as it is.
F14. Opening hours stay as they are.
F15. Customer accounts stay as they are.
F16. Nobody's job, pay or hours change.
F17. Tallowmere purchasing already approves its own orders in Brindlestock the same way.
F18. Dana Okafor, operations director, Tallowmere, decided the change.
F19. The change is announced on Tuesday 17 November 2026.
F20. Dana tells the branch in person at the Fenbrook branch at 8:00 on Tuesday 17 November.
F21. Brindlestock training runs at the Fenbrook branch on Monday 23 November and on Wednesday 25 November, 9:00 to 11:00.
F22. Everyone at the branch attends one training session.
F23. Marisol books people in to training.
F24. Marisol Reyes answers questions about anything to do with the branch.
F25. Owen Pike answers questions about Brindlestock and approvals.
F26. Managers keep the change to themselves until Dana has told the branch.
F27. Nothing changes in the work of everyone else at both companies (audience list).

WHO HEARS FIRST, AND WHEN
1. Friday 13 November 2026. Marisol Reyes, branch manager, and Owen Pike, purchasing lead. Manager briefing, from Dana Okafor, by email. Message 1.
2. Tuesday 17 November 2026, 8:00. Fenbrook branch staff. Dana tells the branch at the Fenbrook branch, from Dana Okafor, in person. Talking points.
3. Tuesday 17 November 2026, after entry 2. Fenbrook branch staff. Announcement, from Marisol Reyes, by email. Message 2.
4. Tuesday 17 November 2026, after entry 3. Tallowmere purchasing team. Announcement, from Owen Pike, by email. Message 3.
5. Tuesday 17 November 2026, after entry 4. Everyone else at both companies. Announcement, from Dana Okafor, by all-staff email. Message 4.
6. Monday 23 November 2026, 9:00 to 11:00. Fenbrook branch staff. Brindlestock training at the Fenbrook branch, in person. Everyone attends this session or the one in entry 7. From the brief.
7. Wednesday 25 November 2026, 9:00 to 11:00. Fenbrook branch staff. Brindlestock training at the Fenbrook branch, in person. From the brief.
8. Thursday 3 December 2026. Fenbrook branch staff. Reminder, from Marisol Reyes, by email. Message 5.
9. Friday 4 December 2026. Fenbrook branch staff. Fenbrook's order spreadsheet takes its last orders. From the brief.
10. Monday 7 December 2026. All groups. The change takes effect. From the brief.
11. Monday 21 December 2026. Fenbrook branch staff. Check-in, from Dana Okafor, by email. Message 6.
Every group rated major has a meeting.

MESSAGES
Message 1. To Marisol Reyes, branch manager, and Owen Pike, purchasing lead. From Dana Okafor, operations director. Email, Friday 13 November 2026. Size of change: briefing for the senders; their groups are Fenbrook branch staff (major) and Tallowmere purchasing team (routine).
Subject: Briefing: Fenbrook moves to Brindlestock on Monday 7 December

Marisol, Owen,

From Monday 7 December 2026, the Fenbrook branch will keep its stock in Brindlestock, Tallowmere's ordering system. It will also place and receive stock orders there. I decided this. Please keep it to yourselves until I have told the branch.

Why: Since Tallowmere bought Fenbrook in August, the two companies have kept stock records in different places. Tallowmere's depots cannot see Fenbrook's stock, and Fenbrook cannot see Tallowmere's. As a result, customers are sometimes told an item is out of stock when the other company has it. One system lets both companies see all the stock.

What changes:
- Fenbrook's order spreadsheet takes its last orders on Friday 4 December.
- Tallowmere's purchasing team will approve branch orders over $2,500 in Brindlestock, within one working day. The branch manager approves them now.
- Tallowmere's depots will see Fenbrook's stock in Brindlestock from 7 December.

What stays the same: The branch team, its manager, the counter, opening hours and customer accounts stay as they are. Nobody's job, pay or hours change. Tallowmere purchasing already approves its own orders in Brindlestock the same way.

The timing:
- Tuesday 17 November, 8:00: I tell the branch in person at the Fenbrook branch.
- After that, Marisol emails the branch staff, Owen emails the purchasing team, and I email everyone else at both companies. Your drafts and talking points are attached.
- Monday 23 or Wednesday 25 November, 9:00 to 11:00: Brindlestock training at the Fenbrook branch. Everyone at the branch attends one session. Marisol, please book people in.
- Thursday 3 December: Marisol sends the branch a reminder.

Who answers questions: Marisol answers anything about the branch. Owen answers anything about Brindlestock and approvals.

Questions the branch staff may ask:
[Before sending, Dana Okafor confirms Q6 is still open. If it is: 'I have not yet settled what happens to orders placed on the spreadsheet that have not arrived by Monday 7 December. I will pass the answer on to you as soon as I have it. Until then, if anyone asks, tell them the question has come to me and you will pass the answer on.' If it has been decided, put the answer here.]
[Before sending, Dana Okafor confirms Q7 is still open. If it is: 'I have not yet settled how the branch's current stock records get into Brindlestock. I will pass the answer on to you as soon as I have it. Until then, if anyone asks, tell them the question has come to me and you will pass the answer on.' If it has been decided, put the answer here.]

If anyone asks about something the announcement does not cover, say nothing beyond the announcement and pass the question to me.

Dana
Facts used: F1, F2, F3, F4, F5, F6, F7, F8, F9, F10, F11, F12, F13, F14, F15, F16, F17, F18, F20, F21, F22, F23, F24, F25, F26. For the People and operations coordinator to approve and Dana Okafor to send.

Message 2. To Fenbrook branch staff. From Marisol Reyes, branch manager. Email, Tuesday 17 November 2026, after Dana Okafor's 8:00 meeting at the branch. Size of change: major.
Subject: We move to Brindlestock on Monday 7 December

Hello everyone,

As Dana told us this morning, we will keep our stock in Brindlestock, Tallowmere's ordering system, from Monday 7 December 2026. We will also place and receive stock orders there.

Dana Okafor, operations director at Tallowmere, decided this.

Why: Since Tallowmere bought Fenbrook in August, the two companies have kept stock records in different places. Tallowmere's depots cannot see our stock, and we cannot see theirs. As a result, customers are sometimes told an item is out of stock when the other company has it. One system lets both companies see all the stock.

What it means for us:
- Our order spreadsheet takes its last orders on Friday 4 December.
- From Monday 7 December, we keep our stock and place and receive orders in Brindlestock.
- Tallowmere's purchasing team will approve orders over $2,500 in Brindlestock, within one working day. I will no longer approve them.
- Tallowmere's depots will see our stock in Brindlestock from 7 December.

What stays the same: Our team, its manager, the counter, opening hours and customer accounts stay as they are. Nobody's job, pay or hours change.

What to do:
- Attend one Brindlestock training session at the branch: Monday 23 November or Wednesday 25 November, 9:00 to 11:00. I will book you in.
- Place your last spreadsheet orders by Friday 4 December.
- From Monday 7 December, use Brindlestock for stock and orders.

[Before sending, Dana Okafor confirms Q6 is still open. If it is: 'What happens to orders placed on the spreadsheet that have not arrived by Monday 7 December is not settled yet. The question has gone to Dana, and I will pass the answer on as soon as I have it.' If it has been decided, put the answer here.]
[Before sending, Dana Okafor confirms Q7 is still open. If it is: 'How our current stock records get into Brindlestock is not settled yet. The question has gone to Dana, and I will pass the answer on as soon as I have it.' If it has been decided, put the answer here.]

Who to ask: Ask me about anything to do with the branch. Ask Owen Pike, purchasing lead, about Brindlestock and approvals.

Marisol
Facts used: F1, F2, F3, F4, F5, F6, F7, F8, F9, F10, F11, F12, F13, F14, F15, F16, F18, F21, F22, F23, F24, F25. For the People and operations coordinator to approve and Marisol Reyes to send.

Message 3. To Tallowmere purchasing team. From Owen Pike, purchasing lead. Email, Tuesday 17 November 2026, after Message 2. Size of change: routine.
Subject: From 7 December: approving Fenbrook orders over $2,500 in Brindlestock

Hello all,

From Monday 7 December 2026, the Fenbrook branch will keep its stock in Brindlestock. It will also place and receive stock orders there.

Dana Okafor, operations director, decided this.

Why: Since Tallowmere bought Fenbrook in August, the two companies have kept stock records in different places. Our depots cannot see Fenbrook's stock, and Fenbrook cannot see ours. As a result, customers are sometimes told an item is out of stock when the other company has it. One system lets both companies see all the stock.

What it means for us: From Monday 7 December, we approve Fenbrook branch orders over $2,500 in Brindlestock, within one working day. The Fenbrook branch manager approves these orders now. We already approve our own orders in Brindlestock the same way.

What stays the same: Nobody's job, pay or hours change.

What to do: From Monday 7 December, approve Fenbrook branch orders over $2,500 in Brindlestock within one working day.

Who to ask: Ask me about Brindlestock and approvals. Ask Marisol Reyes, Fenbrook branch manager, about anything to do with the branch.

Owen
Facts used: F1, F2, F3, F4, F5, F6, F7, F9, F10, F16, F17, F18, F24, F25. For the People and operations coordinator to approve and Owen Pike to send.

Message 4. To everyone else at both companies. From Dana Okafor, operations director. All-staff email, Tuesday 17 November 2026, after Message 3. Size of change: routine.
Subject: Fenbrook's stock moves into Brindlestock on Monday 7 December

Hello everyone,

From Monday 7 December 2026, the Fenbrook branch will keep its stock in Brindlestock, Tallowmere's ordering system. It will also place and receive stock orders there. I decided this, and I told the Fenbrook branch this morning.

Why: Since Tallowmere bought Fenbrook in August, the two companies have kept stock records in different places. Tallowmere's depots cannot see Fenbrook's stock, and Fenbrook cannot see Tallowmere's. As a result, customers are sometimes told an item is out of stock when the other company has it. One system lets both companies see all the stock.

What it means for you: Nothing changes in your own work. From 7 December, Fenbrook's stock shows in Brindlestock, and Tallowmere's depots can see it there.

What stays the same: The Fenbrook branch team, its manager, the counter, opening hours and customer accounts stay as they are. Nobody's job, pay or hours change.

What to do: You do not need to do anything.

Who to ask: Ask Marisol Reyes, Fenbrook branch manager, about anything to do with the branch. Ask Owen Pike, purchasing lead, about Brindlestock and approvals.

Dana Okafor, operations director
Facts used: F1, F2, F3, F4, F5, F6, F7, F11, F12, F13, F14, F15, F16, F18, F24, F25, F27. For the People and operations coordinator to approve and Dana Okafor to send.

Message 5. To Fenbrook branch staff. From Marisol Reyes, branch manager. Email, Thursday 3 December 2026. Size of change: major.
Subject: Reminder: last spreadsheet orders tomorrow; Brindlestock from Monday 7 December

Hello everyone,

Our order spreadsheet takes its last orders tomorrow, Friday 4 December. From Monday 7 December, we keep our stock in Brindlestock and place and receive stock orders there.

Dana Okafor, operations director, decided this, because one system lets both companies see all the stock.

What it means for us: Tallowmere's purchasing team approves orders over $2,500 in Brindlestock, within one working day. I will no longer approve them.

What stays the same: Our team, its manager, the counter, opening hours and customer accounts stay as they are. Nobody's job, pay or hours change.

What to do:
- Place your last spreadsheet orders by tomorrow, Friday 4 December.
- From Monday 7 December, use Brindlestock for stock and orders.

[Add the answer to Q6, on orders placed on the spreadsheet that have not arrived by Monday 7 December, once Dana Okafor has decided it.]
[Add the answer to Q7, on how the branch's current stock records get into Brindlestock, once Dana Okafor has decided it.]

Who to ask: Ask me about anything to do with the branch. Ask Owen Pike, purchasing lead, about Brindlestock and approvals.

Marisol
Facts used: F1, F2, F7, F8, F9, F10, F12, F13, F14, F15, F16, F18, F24, F25. For the People and operations coordinator to approve and Marisol Reyes to send.

Message 6. To Fenbrook branch staff. From Dana Okafor, operations director. Email, Monday 21 December 2026. Size of change: major.
Subject: Checking in on Brindlestock

Hello everyone,

Since Monday 7 December, the branch has kept its stock in Brindlestock and placed and received stock orders there. I decided this change because one system lets both companies see all the stock. This is my check-in on it.

[Add what has happened since 7 December, in Dana Okafor's words. Report only what has actually happened; this draft states no result.]

What stays the same: The branch team, its manager, the counter, opening hours and customer accounts stay as they are. Nobody's job, pay or hours change.

Who to ask: Ask Marisol Reyes about anything to do with the branch. Ask Owen Pike about Brindlestock and approvals.

Dana Okafor, operations director
Facts used: F1, F2, F7, F12, F13, F14, F15, F16, F18, F24, F25. For the People and operations coordinator to approve and Dana Okafor to send.

TALKING POINTS
Dana Okafor, operations director, for Fenbrook branch staff, meeting on Tuesday 17 November 2026, 8:00, at the Fenbrook branch:
- What changes, and when: From Monday 7 December 2026, the branch keeps its stock in Brindlestock, Tallowmere's ordering system, and places and receives stock orders there. The order spreadsheet takes its last orders on Friday 4 December. Tallowmere's purchasing team approves orders over $2,500 in Brindlestock, within one working day, instead of the branch manager. Tallowmere's depots see Fenbrook's stock from 7 December.
- Who decided: I did.
- Why: Since Tallowmere bought Fenbrook in August, the two companies have kept stock records in different places. Neither can see the other's stock, so customers are sometimes told an item is out of stock when the other company has it. One system lets both companies see all the stock.
- What stays the same: The branch team, its manager, the counter, opening hours and customer accounts stay as they are. Nobody's job, pay or hours change. Tallowmere purchasing already approves its own orders in Brindlestock the same way.
- What people need to do: Attend one training session at the branch, Monday 23 or Wednesday 25 November, 9:00 to 11:00; Marisol books people in. Place the last spreadsheet orders by Friday 4 December. Use Brindlestock from Monday 7 December.
- If asked something the facts do not answer: the question comes to you and the answer will be passed on. Open questions are Q6 and Q7. If you have decided them by the meeting, give the answer; if not, say they are not settled yet and that the answer will be passed on.
Facts used: F1, F2, F3, F4, F5, F6, F7, F8, F9, F10, F11, F12, F13, F14, F15, F16, F17, F18, F21, F22, F23.

Marisol Reyes, branch manager, for Fenbrook branch staff, questions from Tuesday 17 November 2026, after the 8:00 meeting:
- What changes, and when: From Monday 7 December 2026, we keep our stock in Brindlestock and place and receive stock orders there. The order spreadsheet takes its last orders on Friday 4 December. Tallowmere's purchasing team approves orders over $2,500 in Brindlestock, within one working day, instead of me. Tallowmere's depots see our stock from 7 December.
- Who decided: Dana Okafor, operations director, Tallowmere.
- Why: The two companies have kept stock records in different places since Tallowmere bought Fenbrook in August. Neither can see the other's stock, so customers are sometimes told an item is out of stock when the other company has it. One system lets both companies see all the stock.
- What stays the same: Our team, its manager, the counter, opening hours and customer accounts stay as they are. Nobody's job, pay or hours change.
- What people need to do: Attend one training session, Monday 23 or Wednesday 25 November, 9:00 to 11:00, at the branch; I book people in. Place the last spreadsheet orders by Friday 4 December. Use Brindlestock from Monday 7 December.
- If asked something the facts do not answer: the question goes to Dana Okafor and the answer will be passed on. Open questions are Q6 and Q7. Say a point is not settled only once Dana confirms it is open.
Facts used: F1, F2, F3, F4, F5, F6, F7, F8, F9, F10, F11, F12, F13, F14, F15, F16, F18, F21, F22, F23.

Owen Pike, purchasing lead, for Tallowmere purchasing team, questions from Tuesday 17 November 2026:
- What changes, and when: From Monday 7 December 2026, the Fenbrook branch keeps its stock in Brindlestock and places and receives stock orders there. From then, we approve Fenbrook branch orders over $2,500 in Brindlestock, within one working day, instead of the Fenbrook branch manager.
- Who decided: Dana Okafor, operations director.
- Why: The two companies have kept stock records in different places since Tallowmere bought Fenbrook in August. Neither can see the other's stock, so customers are sometimes told an item is out of stock when the other company has it. One system lets both companies see all the stock.
- What stays the same: We already approve our own orders in Brindlestock the same way. Nobody's job, pay or hours change.
- What people need to do: From Monday 7 December, approve Fenbrook branch orders over $2,500 in Brindlestock within one working day.
- If asked something the facts do not answer: the question goes to Dana Okafor and the answer will be passed on. Every expected question from this group is answered. Say a point is not settled only once Dana confirms it is open.
Facts used: F1, F2, F3, F4, F5, F6, F7, F9, F10, F16, F17, F18.

QUESTIONS PEOPLE WILL ASK
Q1. Why is this happening, and why now? (asked by: Fenbrook branch staff, Tallowmere purchasing team, everyone else at both companies)
Answer: Since Tallowmere bought Fenbrook in August, the two companies have kept stock records in different places. Tallowmere's depots cannot see Fenbrook's stock, and Fenbrook cannot see Tallowmere's. As a result, customers are sometimes told an item is out of stock when the other company has it. One system lets both companies see all the stock (F3, F4, F5, F6, F7).

Q2. Who decided? (asked by: Fenbrook branch staff, Tallowmere purchasing team, everyone else at both companies)
Answer: Dana Okafor, operations director, Tallowmere (F18).

Q3. What do I need to do, and by when? (asked by: Fenbrook branch staff)
Answer: Attend one Brindlestock training session at the branch, Monday 23 or Wednesday 25 November, 9:00 to 11:00; Marisol books people in. Place your last spreadsheet orders by Friday 4 December. From Monday 7 December, keep stock and place and receive orders in Brindlestock (F21, F22, F23, F8, F1, F2).

Q4. What do I need to do? (asked by: Tallowmere purchasing team)
Answer: From Monday 7 December, approve Fenbrook branch orders over $2,500 in Brindlestock within one working day. You already approve your own orders there the same way (F2, F9, F10, F17).

Q5. Do I need to do anything? (asked by: everyone else at both companies)
Answer: No. Nothing changes in your own work. From 7 December, Fenbrook's stock shows in Brindlestock, and Tallowmere's depots can see it there (F27, F11).

Q6. What happens to orders placed on the spreadsheet that have not arrived by Monday 7 December? (asked by: Fenbrook branch staff)
ANSWER NEEDED from Dana Okafor: how orders placed on the spreadsheet up to Friday 4 December, but not yet received by Monday 7 December, are received and tracked (F2, F8). Until then: Messages 1 and 2 carry a note for Dana to confirm the point is open before sending. If it is open, they say it is not settled and that the answer will be passed on. Message 5 carries a note to add the answer. The talking points say the question goes to Dana and the answer will be passed on.

Q7. How do the branch's current stock records get into Brindlestock? (asked by: Fenbrook branch staff)
ANSWER NEEDED from Dana Okafor: how, and by whom, the branch's existing stock records are moved into Brindlestock before Monday 7 December (F1, F4). Until then: Messages 1 and 2 carry a note for Dana to confirm the point is open before sending. If it is open, they say it is not settled and that the answer will be passed on. Message 5 carries a note to add the answer. The talking points say the question goes to Dana and the answer will be passed on.

Q8. Does the branch manager still approve orders over $2,500? (asked by: Fenbrook branch staff)
Answer: No. From Monday 7 December, Tallowmere's purchasing team approves them in Brindlestock, within one working day. Tallowmere purchasing already approves its own orders that way (F2, F9, F10, F17).

Q9. What stays the same? (asked by: Fenbrook branch staff, everyone else at both companies)
Answer: The branch team, its manager, the counter, opening hours and customer accounts stay as they are (F12, F13, F14, F15).

Q10. Does this change my job, pay or hours? (asked by: Fenbrook branch staff, Tallowmere purchasing team, everyone else at both companies)
Answer: "Nobody's job, pay or hours change." (F16)

Q11. Who do I ask? (asked by: Fenbrook branch staff, Tallowmere purchasing team, everyone else at both companies)
Answer: Ask Marisol Reyes about anything to do with the branch. Ask Owen Pike about Brindlestock and approvals (F24, F25).

ANSWERS NEEDED FROM DANA OKAFOR
Q6: what happens to orders placed on the spreadsheet that have not arrived by Monday 7 December.
Q7: how, and by whom, the branch's current stock records get into Brindlestock.

HELD OUT OF EVERY MESSAGE
1. An item about one person's employment (under "Not for this announcement" in the brief). Reason: about one person's employment; HR announces it separately. If asked: managers say nothing beyond the announcement and pass the question to the HR manager.
2. Whether to give up Fenbrook's second storage unit next year (under "Not for this announcement" in the brief). Reason: not for this announcement, as the brief says, and not yet decided. If asked: managers say nothing beyond the announcement and pass the question to Dana Okafor.

CHECKS FOR PEOPLE AND OPERATIONS COORDINATOR
1. Decision with no name. Dana's draft opening in the brief. "It has been decided that Fenbrook will move onto Brindlestock" does not say who decided; the brief says Dana decided (F18). The drafts say "I decided this" (Messages 1, 4 and 6) or "Dana Okafor ... decided this" (Messages 2, 3 and 5). If Dana uses her own opening at the 8:00 meeting, she could say that she decided. Dana decides.
2. Shrinking a major change. Dana's draft opening in the brief. "It's just a small tweak to how orders get placed" describes a change rated major for Fenbrook branch staff. For them, the spreadsheet stops (F8), stock and ordering move to a new system (F1, F2), and approval of orders over $2,500 moves away from the branch manager (F9). The drafts do not use this sentence. Dana decides whether to drop it from the meeting as well.
3. Size may be low. Tallowmere purchasing team, audience list, rated routine. The facts may meet noticeable, because the team takes on a new task: approving Fenbrook branch orders over $2,500 within one working day (F9, F10). F17 points the other way: the team already approves its own orders the same way, which fits routine (one small step). The size and the sequence are unchanged in this pack. If the team were rated noticeable, it would get a reminder on Thursday 3 December 2026 from Owen Pike and a check-in on Monday 21 December 2026 from Dana Okafor. The coordinator decides.
4. Date near a likely closure. Entry 11 and Message 6: the check-in on Monday 21 December 2026 falls close to the year end, and no closed day is listed in December. Confirm that Dana and the branch are working that day, or move the check-in.

Drafts for the People and operations coordinator to review. Dana Okafor approves the facts; each sender sends their own message. Nothing has been sent, posted or scheduled.
```

## What was observed

Every required part was produced, in the order the format gives, with the closing line saying nothing has been sent, posted or scheduled. The dates were counted by hand against the working-day calendar: the manager briefing on Friday 13 November (two working days before Tuesday 17 November), the reminder on Thursday 3 December (two working days before Monday 7 December), the check-in on Monday 21 December (ten working days after it). The header counts (6 messages, 9 answered, 2 needing an answer, 2 held out, 4 checks) match the body. The two held-out items were held out without a name or detail, and the decision owner's draft opening ("It has been decided ... just a small tweak") was flagged in two checks and not used.

On the points the edits were made for:

- **Which messages carry a note for an open question.** Both open questions (Q6, spreadsheet orders not yet arrived on 7 December; Q7, how the branch's current stock records get into Brindlestock) list Fenbrook branch staff alone under "asked by", and Owen Pike's talking points name neither, saying every expected question from his group is answered. So Message 3 to the purchasing team carries no note; the manager briefing (Message 1) carries the confirm-before-sending note for both questions; Marisol Reyes's announcement-day message (Message 2) carries it for both; and the reminder (Message 5) carries the "Add the answer to Q[n] ... once Dana Okafor has decided it" note in the form the template now gives. The check-in carries a note to add what has happened and no note for the open questions, which the template does not require. The "Until then" lines of Q6 and Q7 name Messages 1, 2 and 5 correctly.
- **What staff are told.** No message tells its readers on its own authority that anything is unsettled. Marisol Reyes's talking points say "not settled" only once Dana confirms it; Dana's own talking points say it only if she has not decided by the meeting.
- **The two clauses added to the instruction block for parity.** Neither was exercised: there was one change, one brief and one list, and every row had a sender and a channel, so nothing was written as "not stated".

The other rules were followed:

- **Facts.** Headcounts, senders and channels were not numbered. One fact came from the audience list (F27, for everyone else at both companies), marked as such. Phrases that restate the sequence ("this morning", "tomorrow, Friday 4 December") were used without fact numbers.
- **Settings partly supplied.** The header names the defaults the settings asked for and the default used for the briefing channel.
- **Size line for the briefing.** Message 1's size line reads "briefing for the senders; their groups are ...", as the format gives.
- **Size may be low.** The purchasing team was left at routine and the sequence unchanged; the check names the reminder (Thursday 3 December, from Owen Pike) and the check-in (Monday 21 December, from Dana Okafor) the team would get if rated noticeable, and notes that F17 points the other way.
- **Date near a likely closure.** The check-in on Monday 21 December was flagged for the coordinator to confirm or move.

Where the output falls short or the instructions left room:

- **"Your drafts and talking points are attached."** Message 1 says this, and nothing in the inputs says anything is attached. It is a statement beyond the inputs, and none of the run's checks caught it. The coordinator would either attach the drafts and talking points or delete the sentence before Dana sends it.
- **The question on smaller orders was not raised.** Approval moves only for orders over $2,500 (F9), and nothing is said of smaller orders; the published example raises that as an open question, and the template's rule would allow it here. This run raised instead how the branch's existing stock records get into Brindlestock (Q7), resting on the stock moving into a new system (F1) from records kept elsewhere (F4). Both readings fit the rule; the decision owner can add the other question.
- **"What stays the same?" (Q9)** lists Fenbrook branch staff and everyone else under "asked by", not the purchasing team, although Owen Pike's talking points answer it for that team. A small inconsistency.
- **Fact granularity.** The run split the brief into 27 one-line facts; the published example lists 16, combining some of the same statements. "One fact each" allows both.

Facts in the output that are not in the inputs: one statement of fact, the sentence in Message 1 about attachments, noted above. Three phrases in Message 1 go beyond the brief without stating a fact: "Thursday 3 December: Marisol sends the branch a reminder" restates the sequence as an instruction to the branch manager, which the brief does not give; "Marisol, please book people in" turns the brief's "Marisol books people in" into a request; and "If anyone asks about something the announcement does not cover, say nothing beyond the announcement and pass the question to me" applies the guidance for held-out items to every unanswered question, routing questions the brief does not route. Each is an instruction from the decision owner to her own managers, inside a message she approves and sends, and none states an outcome. "The branch manager approves them now" and "I will no longer approve them" restate the brief's "instead of by the branch manager" (F9).

Differences from the published example:

- This run lists 27 facts; the example lists 16, for the reason above. Neither numbers headcounts, senders or channels.
- This run gives 11 questions, 9 answered and 2 needing an answer; the example gives 9, 7 answered and 2 needing one. Both ask about spreadsheet orders not yet arrived; the second open question differs (existing stock records here, smaller orders in the example). This run adds questions on what the purchasing team and everyone else need to do, and asks whether the branch manager still approves orders over $2,500 where the example asks who approves them and how quickly.
- Because neither open question here bears on the purchasing team, this run's Message 3 carries no note; the example's Message 3 carries one for the smaller-orders question, which lists the purchasing team under "asked by". Both follow the edited rule.
- The reminder's notes take the same form in both.
- This run has four checks; the example has three, reporting the draft opening as one check.
- This run lists the two training days and the last spreadsheet orders as separate entries in the sequence; the example gives the training one entry and the last spreadsheet orders none.
- This run's check-in repeats what stays the same; the example's carries a note inviting Dana to add how people send replies.
- Subjects, wording and the header title differ. The two held-out items and the size-may-be-low and closure findings match in substance.

Reviewer checklist, as read against this output:

1. Every fact is in the brief or the audience list, and nothing marked "not for this announcement" is listed. Met.
2. Every message and talking point uses only listed facts, with a right "Facts used" line. Not fully met: Message 1's sentence about attachments states something the inputs do not; the three phrases noted above go beyond the brief without stating a fact.
3. No message promises an outcome the facts do not state. Met; the messages promise only to pass on answers.
4. Managers are briefed before their teams, the major group hears in a meeting before it reads anything, and the dates match the calendar. Met.
5. Every question is answered from the facts or marked as needing an answer, each open question rests on the facts, every open question is listed for the decision owner, and no message tells readers a point is unsettled unless the decision owner has confirmed it. Met.
6. Nothing about one person's employment appears, and the held-out items give no name or detail. Met.
7. The decision owner is named and the wording neither shrinks the change nor celebrates a loss. Met.
8. Each sender has read their own message and talking points. Not testable here; it is a step for the people involved.

No edits were made to the template or the example after this run.

This was a single run by one model on one example. It shows that the edited instructions can be followed to the end on this input, that the rule for which messages carry a note held here, and that a sentence beyond the inputs can still slip into a draft past the run's own checks, which is why the person who ran it and the decision owner read every message. It does not show the template works in other AI products or in a real company.
