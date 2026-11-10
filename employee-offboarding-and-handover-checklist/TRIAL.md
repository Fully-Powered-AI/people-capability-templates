# Trial: Employee offboarding and handover checklist, run on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-09

The inputs are the invented example in `public/example.md` (the departure record, access register, equipment list, handover list, offboarding standard and notes). No client data was used. The run followed the instruction block and the output format in `member/template.md`. The model read only the inputs first, produced the full checklist, and only then read the example's output and compared.

The model did not write this template.

## What came out

The full checklist, as produced before the comparison:

```
OFFBOARDING AND HANDOVER CHECKLIST: Senior project coordinator, Delivery team

For: HR lead and Head of delivery. Status: draft for the HR lead's approval.
Last working day: Friday 4 December 2026. Departure confirmed: Friday 6 November 2026. Prepared: Monday 9 November 2026.
Working days left: 17, from Monday 9 November to Friday 4 December. Not working: Thursday 26 and Friday 27 November (office closed); Monday 30 November (booked leave).
Handover document due: Tuesday 17 November (10 working days before the last day). Handover complete by: Tuesday 1 December.
From: access register (7 rows); equipment list (4 items); handover list (4 items); offboarding standard, defaults used for: the items wiped after return (laptop, desktop computer, tablet, mobile phone, external drive); no notes missing.
Lines: 17 (4 handover, 8 access, 5 equipment). Lines flagged: 9. Decisions: 9.
Left out: the reason for leaving.

Handover (owner: Head of delivery)
The departing Senior project coordinator writes the handover document by Tuesday 17 November, covering: where every file and record is kept; each piece of unfinished work and how far it has got; the calendar of recurring work; the people who depend on the role and what each expects; unresolved problems; and the know-how that lives only in their head. The Head of delivery reviews it.
H1 Weekly client status reports for three accounts · Recurring, every Friday · Kept in: shared drive, Delivery/Status reports · Relied on by: three client leads · Receiver: Project coordinator · Hand over by: Tuesday 1 December.
H2 Monthly resource plan · Recurring, first Monday of the month, next on Monday 7 December · Kept in: project tracker · Relied on by: Head of delivery, Finance manager · Receiver: not named · Hand over by: Tuesday 1 December. FLAG, receiver not named: the manager's list says "not decided yet". See decision 1.
H3 Harbour Road project close-out · Open, due Friday 18 December · Kept in: project tracker and shared drive · Relied on by: Harbour Road client lead, client's facilities manager · Receiver: Senior consultant · Hand over by: Friday 11 December. FLAG, after the last day: the manager's hand-over date is a week after the last working day, Friday 4 December. See decision 2.
H4 Supplier invoice approvals for Harbour Road · Open, until close-out · Kept in: not stated · Relied on by: Finance manager · Receiver: Senior consultant · Hand over by: Tuesday 1 December. FLAG, kept in not stated: the handover list gives no location. See decision 3.

Access (removed at 17:30 on Friday 4 December)
A1 Email and calendar · Own mailbox · Standard user · Removed by: IT lead. Before removal: the mailbox is transferred to the Project coordinator, confirmed by the Head of delivery.
A2 Shared drive · Delivery folder · Editor · Removed by: IT lead. Before removal: the files are transferred to the Project coordinator, confirmed by the Head of delivery.
A3 Project tracker · Own account · Admin · Removed by: Head of delivery. FLAG, admin rights: the access level is Admin. See decision 4.
A4 Time and billing system · Own account · Approver · Removed by: Finance manager.
A5 Client file-sharing site · Delivery team login · Editor · Removed by: not named. Shared account: removal means the admin owner, once named, changes the shared sign-in at that time and gives the new one to the remaining users by the company's usual route. FLAG, no admin owner: the register's Admin owner column is empty for this shared account. See decision 5.
A6 Video meetings · Own account · Host · Removed by: IT lead. Before removal: the recordings are transferred to a receiver not named, confirmed by the Head of delivery. FLAG, data receiver not named: the account holds recordings, and the handover list names a receiver only for the mailbox and the shared-drive files. See decision 6.
A7 Travel booking · Own account · Booker · Removed by: Office manager.
A8 Supplier invoicing portal (named in the notes, not on the register) · Account: not stated · Access: not stated · Removed by: not named. FLAG, not on the register: the notes say the coordinator approves supplier invoices for Harbour Road in this portal. See decision 7.
Mail: out-of-office and forwarding to the Head of delivery for 30 days after the last working day, until Sunday 3 January 2027, set by the IT lead.

Equipment (returned to the Office manager on Friday 4 December)
E1 IT-0412 Laptop · Kept at: Home · Return: method to set. Wiped after return, once every data transfer is confirmed, by the IT lead. FLAG, return method to set: the laptop is kept at home. See decision 8.
E2 IT-0519 Mobile phone · Kept at: Carried · Return: to the Office manager on Friday 4 December. Wiped after return, once every data transfer is confirmed, by the IT lead.
E3 IT-0233 Monitor · Kept at: Office · Return: to the Office manager on Friday 4 December.
E4 FAC-118 Building pass · Kept at: Carried · Return: to the Office manager on Friday 4 December.
E5 Plan room keys (named in the notes, not on the equipment list) · Kept at: not stated · Return: method to set. FLAG, not on the equipment list: the notes say the coordinator holds keys to the plan room. See decision 9.

People to tell (owner: Head of delivery)
Team: told by the departing Senior project coordinator on Monday 16 November, at the stand-up, as the notes say. The Head of delivery agrees how and when with the departing Senior project coordinator.
H1: the three client leads told that the Project coordinator takes over, by the Head of delivery, by Tuesday 1 December.
H2: the Finance manager told who takes over, by the Head of delivery, once decision 1 is settled.
H3: the Harbour Road client lead and the client's facilities manager told that the Senior consultant takes over, by the Head of delivery, by Friday 4 December.
H4: the Finance manager told that the Senior consultant takes over, by the Head of delivery, by Tuesday 1 December.

Last working day, Friday 4 December, in this order
1. Handover confirmed complete: H1, H2, H3, H4 (Head of delivery).
2. Data transfers confirmed: A1, A2, A6 (Head of delivery).
3. Equipment returned: E1, E2, E3, E4, E5 (Office manager).
4. Access removed at 17:30: A1 (IT lead), A2 (IT lead), A3 (Head of delivery), A4 (Finance manager), A5 (not named; shared account), A6 (IT lead), A7 (Office manager), A8 (not named).
5. Mail out-of-office and forwarding on (IT lead).
6. After return, devices wiped: E1, E2 (IT lead).

Decisions before this checklist is shared: 9
1. H2, receiver not named. For: Head of delivery. The monthly resource plan is relied on by the Head of delivery and the Finance manager, is next due on Monday 7 December, after the last working day, and the manager's list says the receiver is not decided yet. Who receives it?
2. H3, after the last day. For: Head of delivery. The receiver is the Senior consultant and the hand-over date given is Friday 11 December, a week after the last working day, Friday 4 December. What hand-over date, on or before Friday 4 December, does the Head of delivery set?
3. H4, kept in not stated. For: Head of delivery. The invoice approvals have no location on the handover list; the notes mention a supplier invoicing portal where the coordinator approves them. Where is the work kept?
4. A3, admin rights. For: IT lead. The coordinator has Admin on the project tracker, and the register lists the Head of delivery as its admin owner. Is another admin in place before removal?
5. A5, no admin owner. For: IT lead. The client file-sharing site is a shared account (Delivery team login, Editor) and the register's Admin owner is empty. Who is the admin owner who changes the shared sign-in?
6. A6, data receiver not named. For: Head of delivery. The video meetings account holds recordings, and the handover list names a receiver only for the mailbox and the shared-drive files. Who receives the recordings?
7. A8, not on the register. For: IT lead. The notes name a supplier invoicing portal, where the coordinator approves supplier invoices for Harbour Road; it is not on the access register, so its account, access level and admin owner are not stated. Who is its admin owner, and what are the account and access level?
8. E1, return method to set. For: HR lead. The laptop (IT-0412) is kept at home. How will it be returned to the Office manager: collected, or brought in?
9. E5, not on the equipment list. For: HR lead. The notes say the coordinator holds keys to the plan room; the equipment list does not include them and no location or return method is stated. Where are the keys kept, and how are they returned?

Outside this checklist: pay, benefits, leaving paperwork, references, the exit conversation and any agreement with the departing Senior project coordinator stay with the HR lead's own process. The reason for leaving is not recorded here.

Draft for the HR lead's approval. Nothing has been removed, transferred, returned, sent or changed.
```

## What was observed

Every required part of the output format was produced: header with counts, handover, access with the mail line, equipment, people to tell, the last-day sequence, decisions, the "Outside this checklist" line and the draft line. Nothing in the template made the run stop: all six inputs were present and every header matched. The reason for leaving was in the departure record and was named by kind on the Left out line only. No sign-in detail appeared in the inputs or the output. The counts agree: 17 lines, 9 flagged, 9 decisions, and no checklist-wide issues.

The result matches the published example on every date, count, line, flag and decision number. The differences are small:

- The From line. This run wrote "defaults used for: the items wiped after return", because the standard in the example does not say which items hold company data and the template's default list sits in "What to customize". The example's From line says nothing about defaults.
- The Left out line. The example adds "given in the departure record".
- A8, the invoicing portal. This run wrote "Access: not stated" and one flag kind. The example writes the access as "approves supplier invoices for Harbour Road" and adds a second flag kind, "no admin owner".
- E5, the plan room keys. This run wrote "Return: method to set", because the location is not stated. The example says the keys go to the office manager on Friday 4 December.
- People to tell. This run added the sentence that the Head of delivery agrees how and when with the departing person, as step 6 says. The example leaves it out.
- Decisions 7 and 9 are worded differently (this run asked who the admin owner is and where the keys are kept and how they come back; the example asked who removes the access and whether the keys join the list). Decision 3 in the example points to A8; this run mentions the portal in words.
- Layout. This run used the plain format block; the example uses Markdown bullets and bold.

No fact appears in this run's output that is not in the inputs or the template's own defaults. In the example's output, two points go slightly past the inputs: E5 is given a return date although the template says to flag an unknown location and set no method, and decision 1 says Monday 7 December is "the first working day after the last day", which is true but not stated in the inputs.

Where the instructions left room to guess:

1. How to write a system named in the notes that gives no account or access level. The template says "not stated" for any field the inputs do not give, but the notes do say what the person does there. This run followed the template literally.
2. Whether an item named in the notes but missing from the equipment list, with no location, gets a return date. Step 5 flags only "any other location" and says never to choose a method; for a missing location the template is silent. This run flagged it with "method to set".
3. Which flag kinds apply to an unlisted system. The format allows "not on the register[, kind]", but the kinds defined for access lines (such as no admin owner) are written for register rows.
4. The mail forwarding end date. 30 days after Friday 4 December is Sunday 3 January 2027. Reviewer item 6 says every date is a working day, which cannot hold here, and the template does not say whether to move the date.
5. The instruction block contains unfilled placeholders (such as the day counts and the list of devices to wipe). Most are supplied by the standard in input 5, but the list of items wiped is not part of that standard in this example, so the default had to be taken from "What to customize", which sits outside the pasted block.
6. How to count back for the due dates. This run counted the working days before the last day, not including it, which gives 17 November and 1 December. The text says "counting back from it", which can be read either way. The example agrees with this reading.
7. The people to tell include people outside the company (the client's facilities manager). The template does not say whether the manager may tell an outside person or whether that needs a decision.
8. H3 is on the last-day sequence as "handover confirmed complete" although its hand-over date is after the last day. The template does not say how to treat a flagged item there.
9. The H4 item is "open, until close-out", which gives no due date. The format has a slot for "due [date]" and this run wrote the words as given.
10. The Team line says "told by [role]" while the notes name the departing person; this run used the departing person's role.

Limits of this record: it is one run by one model, on one invented example. It is not a test in a client environment and not a test in other AI products.

## Changed after this run, and not run again

Changed on 9 November 2026 after an independent review of the published template, and not run again. The output and the observations above are as recorded and describe the template and the example as they stood at the run:

- **Counting back** (place 6 above). The procedure and the pasted instructions now say the last working day itself is not counted, the reading this run and the example both used.
- **A system not on the register** (places 1 and 3). The procedure and the pasted instructions now say a description from the notes does not fill the account or access field, which read "not stated", and that such a line carries the one flag "not on the register". The example's A8 and decision 7 now follow this, as the run did.
- **An item with no stated location** (place 2). The procedure and the pasted instructions now say it gets "Return: method to set" and no return date; for an item not on the equipment list, the one flag "not on the equipment list" covers it. The example's E5 and decision 9 now follow this, as the run did.
- **The mail-forwarding end date** (place 4). The procedure and the pasted instructions now say it is counted in calendar days and not moved; reviewer item 6 excludes it.
- **Bracketed placeholders** (place 5). The template now says they are filled in from "What to customize" before pasting and are not reported as defaults, and that the items wiped after return are not part of the offboarding standard. Under this rule the From line would not name a default for the items wiped, as this run's did; the example's From line already matches the rule.
- **People outside the company** (place 7). The procedure and the pasted instructions now say the manager tells them through the company's usual route for that contact.
- **Flagged handover lines on the last day** (place 8). The procedure, the pasted instructions and the output format now show a flagged H line with its decision, such as "H3 (see decision 2)". This run listed H1 to H4 plainly; the example now lists H2, H3 and H4 with their decisions. This part has not been tried.
- **An open item with no due date** (place 9). The output format now allows "Open, as the manager wrote it", as this run and the example wrote H4.
- **The Team line** (place 10 and the People to tell difference). The output format and the pasted instructions now carry the sentence that the manager agrees how and when with the departing person, as this run wrote it; the example now carries it too.
- **The example's decision 1** now says Monday 7 December is after the last working day, as this run wrote it, instead of calling it the first working day after the last day.
