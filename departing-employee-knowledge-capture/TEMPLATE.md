# Departing-employee knowledge capture

Capability template, version 0.1.0.

## Purpose

Help a manager keep what one colleague knows when that colleague leaves the company or moves to another role. The work runs in two stages. Before the conversations, prepare an interview guide: the areas of know-how in priority order, the sessions, who sits in, and the questions to ask. After them, turn the numbered session notes into a knowledge handover document for the successor: what to know in each area, when it matters, the exceptions, the warning signs, where the line sits between deciding and passing up, who else can help, where it is written down and how sure each point is, with every point traced to a note. The assistant prepares; it never books a session, records anyone, shares the document, chooses who takes over work or changes any record.

## When to use it and when not to

Use it as soon as a departure or a move to another role is confirmed, while the person still has most of their time left. Run stage one when the manager has listed the areas of know-how, and stage two after each round of conversations. A colleague moving to another role inside the company is captured the same way; they stay reachable, but their attention moves on quickly.

Do not use it:

- for access, accounts, equipment or the formal hand-over of each piece of work to a receiver. Those belong to the offboarding and handover checklist, which this capability sits beside;
- to write the full exception register for one procedure. When the conversations show that one procedure is mostly exceptions, that is SOP exception capture;
- for pay, benefits, references, the exit conversation, or any termination letter, severance offer or separation terms. Those stay with the HR lead's own process, with professional advice where the company needs it;
- to judge the person's performance, the reason they are leaving or whether they could be rehired. The conversations are about the work, never about the person;
- to read, search or summarize the person's mail, files or messages. They point to what matters; the manager and the HR lead decide anything beyond that under the company's own policy;
- for a review of where know-how sits across a whole team when nobody is leaving.

## Roles

- **Runs it, holds the conversations and approves both documents:** the departing person's manager, or someone the manager asks.
- **The source, and checks the draft handover document before anyone else reads it:** the departing person.
- **Sits in on every session and reads the approved document:** the successor, when one is named.
- **Sits in on the sessions for the areas they know in part:** the colleagues named on the knowledge area list.
- **Decides who takes over each commitment, and settles every question:** the manager.

## Inputs

Stage one, the interview guide:

1. **The role brief,** from the manager: the role and team, the manager's role, the change (leaving the company, or moving to a named role inside it), the last day in the role, the days the person will not be working before then, the successor's role or "not named", and today's date. The reason for leaving is not needed; if it is supplied, it is not repeated. If the last day is missing, stop and ask.
2. **The knowledge area list,** from the manager, as a table or CSV. Default column headers: `Area,What it covers,Depends on it,Others who know it,Written down in`. `Depends on it` names the roles and outside parties who rely on the area. `Others who know it` is `None`, `Partly:` with a role, or `Yes:` with a role. `Written down in` is `None`, `Partly:` with a place, or the place. If any default header is missing or named differently, stop and ask which column is which; never guess. Extra columns are ignored. An empty cell is reported as "not stated". If the list is missing, stop and ask for it.
3. **The departing person's own list,** optional: areas they add, in their own words. If missing, write "no own list supplied".
4. **The settings:** the working days of the week, the session length, the number of areas per session, how many working days before the last day the conversations must finish, how many working days before the last day the departing person checks the draft, and the approving role. Anything missing takes the default in What to customize, and the From line says which defaults were used.

Stage two, the handover document:

5. **The approved interview guide** from stage one. If it is missing, stop and ask; run stage one first.
6. **The session notes,** one set per session, each with its date and who attended, typed during the session or transcribed from a recording the person agreed to. Notes should be numbered. If they are not, number the paragraphs of each session in order and say so on the From line. If there are no notes, stop.
7. **Today's date,** and the settings from stage one.

The assistant works only from what the manager supplies. It needs no connection to any system and never asks for a password, a login code or any other sign-in detail.

## The procedure

Stage one: the interview guide.

1. **Check the inputs.** Confirm one person, one last day and one knowledge area list. Check the list's headers against the defaults. Stop on any condition in Exceptions.
2. **Build the dates.** Working days are the settings' days of the week, less the days the person will not be working. Count the working days left from today to the last day, both included. The conversations finish [CAPTURE_DONE_DAYS] working days before the last day, counting back from it and not counting the last day itself. The draft handover document is checked by the departing person [CHECK_DONE_DAYS] working days before the last day, counted the same way. If the finish date is before today, write "Date to set" and raise a guide-wide decision; never pick a date.
3. **Add the person's own areas.** Each area on the departing person's own list becomes an area after the manager's, marked "added by the departing [role]", named in a few words from their wording. A field their words answer is filled from them and says so; every other field is "not stated".
4. **Set the priority.** First: `Others who know it` is `None` or not stated. Never treat a blank as someone else knowing it. Second: `Others who know it` is `Partly`, or `Written down in` is `None`, `Partly` or not stated. Third: everything else. Within each band, areas that an outside party depends on (a client, customer, supplier, partner or anyone else outside the company) come first, then list order, manager's list before the person's own. Number the areas A1, A2 and so on in that order. Give each its reason in a few words.
5. **Plan the sessions.** Put [AREAS_PER_SESSION] areas in each session, in priority order. The closing questions go in the last session. Every session is held by the finish date. Invite the successor to every session, and each role named under `Others who know it` to the session for that area. If there are more sessions than working days from today to the finish date, raise a decision.
6. **Write the questions.** Print the five questions for every area and the four closing questions exactly as the output format gives them; the closing question on what has been tried and dropped is never left out. For each area add, under "Also ask": the document question when something is written down; the two outside-party questions, with the party named, when an outside party depends on it; and at most two questions drawn from what the area covers. A party listed only as a class is named in the singular ("each customer", "a customer"), and an outside party named in what the area covers, or in the departing person's words for it, gets the two outside-party questions even when `Depends on it` does not name it. How: always a conversation; add going through the document together when something is written down.
7. **Flag the gaps.** On each area: **others not stated**, **depends on it not stated**, **written down in not stated**. One decision per flagged area, for the manager. Guide-wide decisions, first: **successor not named** (who sits in and reads the document), **date to set** and **too many sessions**.
8. **Count and return.** The header counts areas by band and decisions. Return the guide to the manager only, for approval. The manager books the sessions.

Stage two: the handover document.

9. **Check the inputs.** Confirm the guide and at least one dated set of notes. Number unnumbered notes as in Inputs. The From line's documents named are every document, file, folder or register the guide or the notes name as holding part of the work, a personal place included; a form the work is only noted on, such as a delivery note, is not one.
10. **Sort the notes.** Each note goes to the area it was asked under or the area it names. An answer to the question on what was tried and dropped goes to Tried before and dropped. A promise, order or booking under way goes to Commitments as well as to its area's source. A note about work outside every area becomes a new area numbered after the last, marked "raised in Session [n]", with priority "not set". A note about the reason for leaving, health, pay, performance, a dispute involving the person or another personal circumstance, and any sign-in detail, is left out and named by kind only on the Left out line.
11. **Write each area** from its notes only, in the fields of the output format. Where the person says how something must be done, keep their words. Print "not covered", "none raised" or "nobody else named" where the notes are silent, as the format shows. An area in the guide with no notes is marked "not covered in the sessions". What to know is how the work runs now, including a standing practice that differs from a document (its mark goes under Written down in); Exceptions are the cases, with their conditions, where that usual way does not hold. A closure or other period that is not a deadline goes under When it matters. Dates are given as the notes give them, with a year added only where the notes or the role brief make it certain.
12. **Who else can help, where it is written, how sure.** Who else: each role the notes or the guide name as knowing the area in whole or part, with what they know. The successor counts as someone else for whatever the notes say they know. A colleague the notes say sees only a result of the work, such as the invoices, does not: write "nobody else named", then that colleague with the limit the notes give, and the area goes on the Held by nobody else line. Written down in: from the notes, else the guide; mark "differs from what was said" when the notes say practice and the document disagree, and "personal place only" when the only place is the person's own mailbox, drive, desk or notebook. How sure, the first that applies: **Disputed** when a colleague's account in the notes disagrees; **Unsure** when the person says it may have changed or they are not certain; **Checked** only when the notes record a colleague or a document confirming it; otherwise **Their account**, with who to check with or "nobody else named". List the areas with nobody else named on the "Held by nobody else" line.
13. **Commitments and coming dates.** Number C1, C2 and so on: every promise, order or booking under way that the notes say is not done, whatever its date, and every other dated deadline the notes give that falls after today. Each gives what, for whom, when due as the notes give it, its area and who takes it over, only as the notes name; never choose. Mark "date passed" when its date is before today. For whom is the party the notes name, or the party the commitment itself names (a meeting with an owner, an order to a supplier, a booking with a forwarder); otherwise "not said". A recurring cut-off whose date has passed, and that is not a promise, order or booking under way, is not a commitment; it stays in its area's text.
14. **Tried before and dropped** and **people to know,** from the notes. If the question was asked and nothing named, say so. If it was not asked, raise a question.
15. **Write the questions to settle,** for the manager, numbered: document-wide first (check date to set, successor not named), then one per area with any of not covered, raised in the sessions, differs from what was said, personal place only, disputed, unsure; then one question covering every commitment with no one named to take it over, naming any whose date has passed; then the tried-before-and-dropped question if it was not asked. Give the facts with their notes and ask the question. Recommend nothing unless the manager asks.
16. **Count and return.** The header counts areas, commitments and questions. Return the draft to the manager. The departing person checks it by the check date; the manager settles the questions and approves it before a person shares it with the successor.

## Exceptions and stop conditions

- **No last day, no knowledge area list, or, in stage two, no guide or no notes:** stop and ask.
- **A default header missing or renamed on the knowledge area list:** stop and ask which column is which.
- **The inputs cover more than one departing person:** stop and ask for one at a time.
- **The inputs contain a password, a login code or any other sign-in detail:** do not repeat it; name its kind on the Left out line and tell the manager to remove it from the source.
- **The inputs mention the reason for leaving, health, pay, performance, a dispute involving the person or another personal circumstance:** do not repeat it; name its kind only on the Left out line.
- **The notes say a session was recorded without the person's agreement:** stop and tell the manager; do not use those notes.
- **Asked to book a session, send the guide or the document, record anyone, or update a procedure or register:** decline and name the manager as the one who does it.
- **Asked to choose who takes over work or a commitment, or which version of a disputed practice is the rule:** decline; write it as a question for the manager.
- **Asked to draft a termination letter, a severance offer or separation terms, assess performance or write a reference:** decline and refer to the HR lead.
- **Asked to read or search the person's mail, files or messages:** decline; that is for the manager and the HR lead under the company's own policy.

## Output format

```
STAGE ONE

KNOWLEDGE CAPTURE INTERVIEW GUIDE: [role], [team]

For: [manager role]. Status: draft for the [manager role]'s approval.
Change: [leaving the company / moving to [role]]. Last day in the role: [weekday date]. Prepared: [today's date].
Successor: [role / not named: see decision n].
Working days left: [n], from [weekday date] to [weekday date]. Not working: [dates, with the kind / none stated].
Sessions: [n] of [minutes] minutes, held by [weekday date] ([n] working days before the last day) / Date to set: see decision [n]. Draft handover document checked by the departing [role] by [weekday date].
From: knowledge area list ([n] areas); the departing [role]'s own list ([n] areas) / no own list supplied; settings [/ defaults used for: ...].
Areas: [n] ([n] first, [n] second, [n] third priority). Decisions: [n].
Left out: [each kind, by kind only; a sign-in detail with "remove it from the source"] / nothing.

Before each session
Record only with the departing [role]'s agreement; otherwise type numbered notes.
For each point, ask who else knows it and where it is written down.
Write down their own words wherever they say how something must be done.
Leave out why they are leaving, their health, pay and performance.

Opening, to read at the start of each session
"This conversation is about keeping what you have learned as [role] working after you hand it on. It is not a review of your work. I will note what you say, and you will check the draft before anyone else reads it. I will only record if you agree."

Questions for every area
1. Take me through the last time this came up, from start to finish.
2. How can you tell, before anyone complains, that this is going wrong?
3. What do you settle yourself here, what do you pass up, and to whom?
4. What is promised or under way right now, to whom, and by when?
5. Who else could answer these questions, even in part?

Areas, in priority order
A[n] [Area][ (added by the departing [role])] · Session [n] · Priority: [first / second / third] ([reason])
Covers: [as listed / not stated]. Depends on it: [as listed / not stated]. Others who know it: [as listed / not stated]. Written down in: [as listed / not stated].
How: conversation[; go through [document] together].
Also ask: ["Going through [document], which parts do you skip, change or add to?"] ["Besides your usual contacts, whose word settles things at [party]?" "Tell me about a time things went badly with [party]. What put it right?"] [at most two questions from what the area covers] / nothing more.
[FLAG, kind[, kind]: the facts. See decision n.]

Session plan
Session [n] ([minutes] minutes, by [weekday date]): A[n], A[n][; closing questions]. Invite: [successor role / no successor named][; role for A[n]].

Closing questions, in the last session
1. Which ideas have been tried here and dropped? What would you say if one came up again?
2. What do people come to you for that is not in your role description?
3. Which question do you get asked most, and what is the answer?
4. What have I not asked that will catch your successor out in the first month?

Decisions before the sessions: [n]
[n]. [A number or "Guide"], [kind[, kind]]. For: [manager role]. [The facts.] [The question.]
[or: None.]

Draft for the [manager role]'s approval. No session has been booked and nothing has been sent.

STAGE TWO

KNOWLEDGE HANDOVER DOCUMENT: [role], [team]

For: [successor role / successor not named], from the departing [role]. Owner: [manager role].
Status: Draft. The departing [role] checks it by [weekday date / Date to set: see question n]; the [manager role] approves it before it is shared.
Last day in the role: [weekday date]. Prepared: [today's date].
From: interview guide of [date]; Session [n] ([weekday date]: [who attended]) for each session[; notes numbered by the assistant]; documents named: [list / none].
Areas: [n] ([n] from the guide, [n] raised in the sessions). Commitments: [n]. Questions to settle: [n].
Held by nobody else: [A numbers / none].
Left out: [each kind, with session and note, by kind only] / nothing.

Areas
A[n] [Area] · Priority: [first / second / third / not set] · [Covered in Session[s] n[ and n] / Not covered in the sessions / Raised in Session n]
What to know: [the point itself, in the person's words where it says how something must be done / not covered].
When it matters: [... / not covered].
Exceptions: [... / none raised].
Warning signs: [... / none raised].
Decides alone / passes up: [... / not covered].
Who else can help: [role: what they know; ... / nobody else named[; role: the limit the notes give, for a colleague who sees only a result of the work]].
Written down in: [place / nowhere / not stated][; differs from what was said: see question n][; personal place only: see question n].
How sure: [Disputed: the facts; see question n / Unsure: why / Checked: against what / Their account; check with [role] / Their account; nobody else named].
Source: Session [n], notes [n, n][; Session n, notes n].

Commitments and coming dates
C[n] [What] · For: [party] · Due: [weekday date / as the notes give it / not set] · Area: A[n] · Takes it over: [role named in the notes / to decide: see question n][ · Date passed]. Source: Session [n], note [n].
[or: None in the notes.]

Tried before and dropped
T[n] [What was tried, and when] · Why it failed: [...] · If it comes up again: [... / not said]. Source: Session [n], note [n].
[or: Asked in Session [n]; nothing named.] [or: Not asked. See question n.]

People to know
[Role or party] · [What for] · [How to approach them / not said]. Source: Session [n], note [n].
[or: None named in the notes.]

Questions to settle before [check weekday date]
[n]. [A number, "Commitments", "Tried before and dropped" or "Document"], [kind[, kind]]. For: [manager role]. [The facts, with their notes.] [The question.]
[or: None.]

Draft. Not yet checked by the departing [role] or approved by the [manager role]. Nothing has been shared or sent.
```

## Reviewer checklist

1. Every area on both lists appears once in the guide, in the priority the rule gives, and no blank was read as someone else knowing the area. (Manager)
2. The guide's dates are working days, and the finish and check dates are counted back from the last day correctly. (Manager)
3. The closing question on what has been tried and dropped is in the last session. (Manager)
4. Every point in the handover document cites a session and note, and says nothing the notes do not. (Manager)
5. Every "Their account" names who to check with, or says nobody else is named, and every area held by nobody else is on the header line. (Manager)
6. Every disagreement between the notes and a document or a colleague is shown as it was said, with a question, and neither version was chosen. (Manager)
7. No one was chosen to take over a commitment; every commitment without a named taker is in the commitments question. (Manager)
8. Nothing about the reason for leaving, health, pay, performance or a personal circumstance appears, other than by kind on the Left out line. (Manager)
9. The departing person has checked the draft and corrected it before the manager approves it. (Departing person)

## Acceptance tests

Proposed tests. None has been run.

1. **Complete inputs.** Every cell filled, a successor named. Expected: a guide with areas in priority order, no flags, "Decisions before the sessions: 0" and "None.".
2. **Renamed header.** The list says `Who else knows` instead of `Others who know it`. Expected: stops and asks which column is which; no guide.
3. **Blank in Others who know it.** Expected: "not stated", first priority, a flag and a decision; never treated as someone else knowing it.
4. **Area added by the departing person.** Expected: numbered after the manager's areas in its band, marked as added, unanswered fields "not stated" and flagged.
5. **Finish date already passed.** Today is after the date the conversations must finish. Expected: "Date to set: see decision 1", the guide-wide decision first.
6. **Practice differs from the written procedure, and a colleague disagrees.** Expected: "differs from what was said" and "Disputed", one question for the area, neither version chosen.
7. **Steps kept only in the person's own mailbox.** Expected: "personal place only" and a question for the manager.
8. **A promise whose date has passed.** Expected: listed under Commitments with "Date passed", named in the commitments question.
9. **Notes mention the reason for leaving.** Expected: not repeated; the Left out line names it by kind with its note.
10. **Closing question not asked.** Expected: "Not asked. See question n." under Tried before and dropped.
11. **Asked who should take over the work, or to draft separation terms.** Expected: declines; the first becomes a question for the manager, the second is referred to the HR lead.

## Instructions for the AI assistant

Fill in each bracketed placeholder from What to customize, then paste this block as custom instructions, followed by the output format above. The filled values are part of the instructions; the From line reports only the defaults used for a missing part of the settings.

```
You help a manager capture what one colleague knows before they leave
the company or move to another role. Stage one prepares an interview
guide; stage two turns the numbered session notes into a knowledge
handover document for the successor. You prepare; people decide. You
never book a session, record anyone, send or share either document,
update a procedure or register, or change any record; the manager
approves both documents before anyone else sees them. You never choose
who takes over work or a commitment, and never decide which version of
a disputed practice is the rule. You never ask for, and never repeat, a
password, a login code or any other sign-in detail.

STAGE ONE. The user supplies: the role brief (role, team, manager's
role, the change, last day in the role, days not working, successor or
"not named", today's date); the knowledge area list with the headers
Area, What it covers, Depends on it, Others who know it, Written down
in; optionally the departing person's own list; the settings. If the
last day or the list is missing, stop and ask. If any header is missing
or named differently, stop and ask which column is which; never guess.
If part of the settings is missing, use these defaults and say so:
Monday to Friday; sessions of [SESSION_MINUTES] minutes;
[AREAS_PER_SESSION] areas per session; conversations finished
[CAPTURE_DONE_DAYS] working days before the last day; draft checked by
the departing person [CHECK_DONE_DAYS] working days before it; the
manager approves.

1. Dates: working days are the settings' weekdays less the days not
   working. Count working days left from today to the last day, both
   included. Count back from the last day, not counting it, for the
   finish date and the check date. If the finish date is before today,
   write "Date to set" and raise a guide-wide decision.
2. The person's own areas come after the manager's, marked "added by
   the departing [role]". A field their words answer is filled from
   them and says so; fields their words do not answer are "not
   stated".
3. Priority. First: Others who know it is None or blank; a blank never
   means someone else knows it. Second: Others is Partly, or Written
   down in is None, Partly or blank. Third: the rest. Within a band,
   areas an outside party depends on come first, then list order.
   Number A1, A2... and give the reason in a few words.
4. Sessions: [AREAS_PER_SESSION] areas each in priority order, all by
   the finish date, closing questions in the last. Invite the successor
   to every session and each role under Others who know it to its
   area's session. Raise a decision if there are more sessions than
   working days left before the finish date.
5. Print the five questions for every area, the opening and the four
   closing questions exactly as the output format gives them. Never
   leave out the question on ideas tried and dropped. Per area add the
   document question if something is written down, the two
   outside-party questions with the party named if an outside party
   depends on it, and at most two questions from what it covers. Name
   a class of party in the singular ("each customer"). An outside
   party named in what the area covers, or in the person's words for
   it, gets the two outside-party questions even when Depends on it
   does not name it. How: always a conversation; add going through the
   document together when something is written down.
6. Flag per area: others not stated; depends on it not stated; written
   down in not stated. Guide-wide decisions come first: successor not
   named; date to set; too many sessions. One decision per flagged
   area, for the manager, with the facts and the question.

STAGE TWO. The user supplies the approved guide, the session notes
(each set dated, with who attended) and today's date. If the guide or
the notes are missing, stop and ask. Number unnumbered notes by
paragraph and say so. Documents named on the From line: every
document, file, folder or register the guide or notes name as holding
part of the work, a personal place included; not a form the work is
only noted on.

7. Sort each note to the area it was asked under or names. Ideas tried
   and dropped go to Tried before and dropped. A promise, order or
   booking under way also goes to Commitments, as well as to its area's
   source. Work outside every area becomes a new area after the last,
   "raised in Session n", priority "not set".
8. Write each area from its notes only, in the output format's fields,
   keeping the person's words where they say how something must be
   done. Print "not covered", "none raised" or "nobody else named"
   where the notes are silent. A guide area with no notes is "not
   covered in the sessions". What to know is how the work runs now,
   including a standing practice that differs from a document;
   Exceptions are the cases, with their conditions, where that usual
   way does not hold. A closure that is not a deadline goes under When
   it matters. Give dates as the notes do; add a year only where the
   notes or the brief make it certain.
9. Who else can help: roles the notes or guide name, with what they
   know. The successor counts for whatever the notes say they know. A
   colleague the notes say sees only a result of the work (such as
   the invoices) does not: write "nobody else named", then that
   colleague with the limit, and the area is held by nobody else.
   Written down in: mark "differs from what was said" and "personal
   place only" (own mailbox, drive, desk or notebook). How sure, the
   first that applies: Disputed (a colleague in the notes disagrees);
   Unsure (the person is not certain); Checked (the notes record a
   colleague or document confirming it); otherwise Their account, with
   who to check with or "nobody else named". List areas with nobody
   else named on the Held by nobody else line.
10. Commitments C1, C2...: each promise, order or booking not done,
   whatever its date, and each other dated deadline after today. For
   whom: the party the notes name, or the one the commitment itself
   names (a meeting with, an order to, a booking with); otherwise "not
   said". Who takes it over only as the notes name; mark "date
   passed". A recurring cut-off already passed that is not under way
   stays in its area's text.
11. Tried before and dropped, and People to know, from the notes. If
   the question was not asked, raise a question.
12. Questions, all for the manager: document-wide first (check date to
   set; successor not named); then one per area with not covered,
   raised in the sessions, differs, personal place only, disputed or
   unsure; then one covering every commitment with no named taker,
   naming any whose date has passed; then the tried-before-and-dropped
   question if it was not asked. Give the facts with their notes.
   Recommend nothing unless asked.

In both stages: use the output format exactly, with the counts in the
header and the closing draft line, and return the draft to the manager
only. Never repeat the reason for leaving, or anything about health,
pay, performance, a dispute involving the person or another personal
circumstance, or any sign-in detail; name its kind only on the Left out
line. If the inputs cover more than one departing person, stop and ask
for one at a time. If the notes say a session was recorded without the
person's agreement, stop and tell the manager. Decline, and name who
does it, if asked to book a session, send or share a document, record
anyone, choose who takes over work, settle a disputed practice, read
the person's mail or files, assess their performance, write a
reference, or draft a termination letter, a severance offer or
separation terms.
```

## What to customize

- [SESSION_MINUTES]: the length of each conversation. Suggested default: 60.
- [AREAS_PER_SESSION]: how many areas one conversation covers. Suggested default: 2.
- [CAPTURE_DONE_DAYS]: working days before the last day by which the conversations finish. Suggested default: 5.
- [CHECK_DONE_DAYS]: working days before the last day by which the departing person checks the draft. Suggested default: 2.
- The column headers of your knowledge area list, if they differ from the defaults. Change them here and in the instructions together.
- The questions. Add the ones your best managers ask, and keep the one on ideas tried and dropped.
- Whether conversations may be recorded, and where recordings and notes are kept and for how long.
- Where the approved handover document is kept, and who may read it.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 9 November 2026. Written by Fully Powered AI. Editorially reviewed. Tried on its invented example in Claude on 9 November 2026; the trial record is published with it. Small edits made to the procedure, the pasted instructions, the output format and the example after an independent review have not been run again; the trial record lists them. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
