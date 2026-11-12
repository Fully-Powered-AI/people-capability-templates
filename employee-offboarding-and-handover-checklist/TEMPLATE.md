# Employee offboarding and handover checklist

Workflow template, version 0.1.0.

## Purpose

Prepare the dated checklist for one colleague's departure, for the HR lead and the departing person's manager: every piece of the person's work handed to a named colleague before the last day, every system on the company's access register removed by a named owner at a set time, every item of equipment returned, and the people who need to know who takes over. Every gap is flagged and written as a question for the role that settles it. The assistant prepares; it never removes access, transfers data, sends a message, chooses who takes over work or changes any record.

## When to use it and when not to

Use it the day the departure and the last working day are confirmed, so the handover starts while the person has most of their time left. Run it again when the last day moves, a receiver is named or the access register changes.

Do not use it:

- for pay, benefits, leaving paperwork, references or the exit conversation. Those stay with the HR lead's own process;
- to draft a termination letter, a severance offer, separation terms or any other employment document, or to advise on notice or entitlements. Those belong to the HR lead, with professional advice where the company needs it;
- to decide why someone is leaving, whether they could be rehired or how they performed;
- to read, search or monitor the departing person's mail, files or messages;
- for a departure where access must come off immediately. The HR lead and the IT lead set that time first; the checklist then follows it.

## Roles

- **Runs it and approves the checklist:** the HR lead.
- **Owns the handover, names every receiver and tells the people who rely on the role:** the departing person's manager.
- **Writes the handover document and returns the equipment:** the departing person.
- **Removes access, sets mail forwarding and wipes devices:** the admin owner named on the access register for each system, and the IT lead.
- **Take over the work:** the receivers the manager names.

## Inputs

1. **The departure record,** from the HR lead: the role and team, the manager's role, the date the departure was confirmed, the last working day, the days the person will not be working before then (booked leave, office closures) and today's date. The reason for leaving is not needed; if it is supplied, it is not repeated. If the last working day is missing, stop and ask.
2. **The access register,** exported for the departing person only. Default column headers: `System,Account,Access level,Admin owner,Shared account,Company data held`. `Shared account` is Yes or No. `Company data held` is None or what the account holds, such as a mailbox, files or recordings. If the register is missing, stop and ask for it. If any default header is missing or named differently, stop and ask which column is which; never guess. Extra columns are ignored.
3. **The equipment list,** exported for the departing person only. Default column headers: `Asset tag,Item,Issued,Location`. `Location` is Office, Carried, or where else the item is kept, such as Home. If a header does not match, stop and ask. If the list is missing, continue, write "equipment list not supplied" and raise it as a decision for the HR lead.
4. **The handover list,** from the manager: each piece of work the person does, whether it is recurring (how often, and the next date if known) or open (its due date), where it is kept, who relies on it, who receives it and, if the manager wants, a hand-over date. Also who receives the person's mailbox and files. If the list is missing, continue, write "handover list not supplied" and raise it as a decision for the manager.
5. **The offboarding standard,** from the HR lead: the working days of the week, when the handover document is due, when the handover must be complete, the time access is removed, how long mail is forwarded and to whom, who equipment is returned to, and the role that wipes devices and sets mail. Anything missing takes the default in What to customize, and the From line says which defaults were used. The items wiped after return ([DATA_DEVICES]) are not part of the standard: they are filled into the instructions before pasting and are not reported as a default.
6. **Notes,** from the HR lead or the manager, optional: a system or item the lists leave out, how the team will be told, anything that affects a date. If missing, write "no notes supplied".

The assistant works from files and notes the person supplies. It needs no connection to any system and never asks for a password, a login code or any other sign-in detail.

## The procedure

1. **Check the inputs.** Confirm one departing person, one last working day and one access register. Check the headers of each export against the defaults. Stop on any condition in Exceptions.
2. **Build the dates.** Working days are the standard's days of the week, less the dates the person will not be working. Count the working days left from today to the last working day, both included. The handover document is due [HANDOVER_DOC_DAYS] working days before the last working day, counting back from it, not counting the last working day itself. The handover is complete [HANDOVER_DONE_DAYS] working days before the last working day, counting the same way. If the document's due date is before today, write "Date to set" and raise a checklist-wide decision for the HR lead and the manager; never pick a date.
3. **Handover lines.** One line per item on the handover list, numbered H1, H2 and so on, in the manager's order. Keep the manager's wording. Each line gives: recurring (how often, next date if given) or open (due date); where it is kept; who relies on it, with "me" written as the manager's role; the receiver; and the hand-over date, which is the manager's date if given and otherwise the handover-complete date. Flag:
   - **receiver not named;**
   - **kept in not stated;**
   - **after the last day:** the hand-over date falls after the last working day.
   Never choose a receiver, a location or a date. Information elsewhere in the inputs that may answer a flag goes in its decision, not on the line.
4. **Access lines.** One line per register row, numbered A1, A2 and so on, in register order. Each line gives the system, account and access level, who removes it (the admin owner) and when ([ACCESS_REMOVAL_TIME] on the last working day). Where company data is held, add the step before removal: the data is transferred to the receiver the manager named for it, and the manager confirms the transfer. Where the account is shared, removal means the admin owner changes the shared sign-in at that time and gives the new one to the remaining users by the company's usual route; the checklist never contains any sign-in detail. Flag:
   - **no admin owner:** the column is empty;
   - **admin rights:** the access level contains "admin" or "owner". The question asks whether another admin is in place before removal;
   - **data receiver not named:** data is held and the handover list names nobody to receive that kind of data;
   - **duplicate on the register:** two rows share a system and account. List the system once.
   Then add one line for each system named in the handover list or the notes that is not on the register, numbered after the register rows and marked "(named in [where], not on the register)", with "not stated" for any field the inputs do not give. A description in the notes of what the person does in the system is not an account or an access level: those fields read "not stated" and the description goes in the flag's facts. Removed by reads "not named". Flag it **not on the register** only; the other access flags are for register rows, and its decision asks who removes the access. Under the access lines, write the mail line: out-of-office and forwarding to the standard's receiver for [FORWARDING_DAYS] days after the last working day, with the end date, set by the standard's role. The end date is counted in calendar days and is not moved to a working day.
5. **Equipment lines.** One line per item, numbered E1, E2 and so on, in list order. Items kept at the Office or Carried are returned to [RETURN_TO] on the last working day. Any other location, or no location stated, gives "Return: method to set" and is flagged **return method to set**; never choose between collection and bringing it in, and never give such an item a return date. Items in [DATA_DEVICES] get the wipe step: wiped after return, once every data transfer is confirmed, by the standard's role. Add one line for each item named in the handover list or the notes that is not on the equipment list, marked "(named in [where], not on the equipment list)", and flag it **not on the equipment list**. If the inputs give it no location, its return reads "method to set" and that one flag covers it: its decision asks where the item is kept, how it comes back and whether it joins the list.
6. **People to tell.** The team: told by whoever the notes say, on the date they give, or "date to agree with the departing [role]" if they give none. The checklist adds that the manager agrees how and when with the departing person. Then one line per handover item: the people who rely on it, other than the manager, are told who takes it over, by the manager, by the item's hand-over date or the last working day, whichever is earlier. Where the receiver is not named, write "once decision [n] is settled". Where someone who relies on an item is outside the company, such as a client's contact, the manager tells them through the company's usual route for that contact.
7. **The last-day sequence.** In this order: handover confirmed complete (H lines, manager; a flagged H line is shown with its decision, such as "H3 (see decision 2)"); data transfers confirmed (A lines with data, manager); equipment returned (E lines, [RETURN_TO]); access removed at the set time (A lines, each with its admin owner or "not named", shared accounts marked); mail forwarding on (the standard's role); devices wiped after return (E lines with the wipe step, the standard's role).
8. **Decisions.** One numbered decision per flagged line, and one per checklist-wide issue (a handover date to set, a missing equipment or handover list, an access time the notes put in question). Several flags on one line share one decision that asks about each. Checklist-wide decisions come first, then H, A and E lines in order. Each names who it is for: the manager for receivers, locations, hand-over dates and data receivers; the IT lead for admin owners, admin rights, duplicates and systems not on the register; the HR lead for equipment; the HR lead and the IT lead together for access timing. Each gives the facts and asks the question. Recommend nothing unless asked.
9. **Count and return.** The header counts lines, flagged lines and decisions, and the Left out line names by kind anything kept out under Exceptions, or says "nothing"; the number of decisions equals flagged lines plus checklist-wide issues. Print the fixed "Outside this checklist" line and the draft line. Return the draft to the HR lead only. The HR lead settles or passes on each decision and approves the checklist before a person shares it with the manager, the IT lead and the departing person.

## Exceptions and stop conditions

- **No last working day or no access register:** stop and ask.
- **A default header missing or renamed in an export:** stop and ask which column is which. Do not map columns by guesswork.
- **An export covers more than one person:** stop and ask for the departing person's rows only.
- **The inputs contain a password, a login code or any other sign-in detail:** do not repeat it anywhere; on the Left out line, name its kind and tell the person to remove it from the source.
- **The inputs give the reason for leaving, or mention a dispute, misconduct, health, a personal circumstance or pay:** do not repeat it. Continue with access, equipment and handover only, and name its kind, never its content, on the Left out line.
- **The notes say access may need to come off before the last day:** keep every date as the standard sets it, and put the access timing first among the decisions, for the HR lead and the IT lead. Never set the time yourself.
- **Asked to remove access, transfer data, set forwarding, wipe a device, message anyone or update the register:** decline and name the role that does it.
- **Asked to choose a receiver or a date:** decline; the manager decides.
- **Asked to draft a termination letter, a severance offer or separation terms, work out final pay or entitlements, write a reference, or say whether the person could be rehired:** decline and refer to the HR lead.
- **Asked to read, search or summarize the departing person's mail, files or messages:** decline; that is for the HR lead and the IT lead under the company's own policy.

## Output format

```
OFFBOARDING AND HANDOVER CHECKLIST: [role], [team]

For: [HR lead role] and [manager role]. Status: draft for the [HR lead role]'s approval.
Last working day: [weekday date]. Departure confirmed: [date]. Prepared: [today's date].
Working days left: [n], from [weekday date] to [weekday date]. Not working: [dates, with the kind / none stated].
Handover document due: [weekday date] ([n] working days before the last day) / Date to set: see decision [n]. Handover complete by: [weekday date].
From: access register ([n] rows); equipment list ([n] items) / equipment list not supplied; handover list ([n] items) / handover list not supplied; offboarding standard [/ defaults used for: ...]; notes / no notes supplied.
Lines: [n] ([n] handover, [n] access, [n] equipment). Lines flagged: [n]. Decisions: [n].
Left out: [each kind left out, such as the reason for leaving or a health note, by kind only; a sign-in detail, with "remove it from the source"] / nothing.

Handover (owner: [manager role])
The departing [role] writes the handover document by [weekday date / the date to set], covering: where every file and record is kept; each piece of unfinished work and how far it has got; the calendar of recurring work; the people who depend on the role and what each expects; unresolved problems; and the know-how that lives only in their head. The [manager role] reviews it.
H[n] [Work, as the manager wrote it] · [Recurring, how often[, next on weekday date] / Open, [due weekday date / as the manager wrote it]] · Kept in: [location / not stated] · Relied on by: [roles / not stated] · Receiver: [role / not named] · Hand over by: [weekday date]. [FLAG, kind[, kind]: the facts. See decision n.]
[or: Handover list not supplied. See decision n.]

Access (removed at [time] on [weekday date])
A[n] [System] · [Account] · [Access level] · Removed by: [admin owner / not named]. [Before removal: [data held] transferred to [role / receiver not named], confirmed by the [manager role].] [Shared account: removal means the [admin owner / owner, once named] changes the shared sign-in.] [FLAG, kind[, kind]: the facts. See decision n.]
A[n] [System] (named in [where], not on the register) · Account: [account / not stated] · Access: [level / not stated] · Removed by: not named. FLAG, not on the register: the facts. See decision n.
Mail: out-of-office and forwarding to the [role] for [n] days after the last working day, until [weekday date], set by the [role].

Equipment (returned to the [role] on [weekday date])
E[n] [Asset tag] [Item] · Kept at: [location] · Return: [to the role on weekday date / method to set]. [Wiped after return, once every data transfer is confirmed, by the [role].] [FLAG, kind: the facts. See decision n.]
E[n] [Item] (named in [where], not on the equipment list) · Kept at: [location / not stated] · Return: [...]. FLAG, not on the equipment list: the facts. See decision n.
[or: Equipment list not supplied. See decision n.]

People to tell (owner: [manager role])
Team: told by [role] on [weekday date][, how, as the notes say] / date to agree with the departing [role]. The [manager role] agrees how and when with the departing [role].
H[n]: [roles] told that the [receiver] takes over / told who takes over, by the [manager role], by [weekday date] / once decision [n] is settled.
[or: No one named beyond the team.]

Last working day, [weekday date], in this order
1. Handover confirmed complete: [H numbers, a flagged one as "H[n] (see decision n)"] ([manager role]).
2. Data transfers confirmed: [A numbers / none] ([manager role]).
3. Equipment returned: [E numbers / none] ([role]).
4. Access removed at [time]: [A numbers, each with its admin owner or "not named"; shared accounts marked].
5. Mail out-of-office and forwarding on ([role]).
6. After return, devices wiped: [E numbers / none] ([role]).

Decisions before this checklist is shared: [n]
[n]. [Line number or "Checklist", kinds of flag.] For: [role]. [The facts.] [The question, one for each kind of flag.]
[or: None.]

Outside this checklist: pay, benefits, leaving paperwork, references, the exit conversation and any agreement with the departing [role] stay with the [HR lead role]'s own process. The reason for leaving is not recorded here.

Draft for the [HR lead role]'s approval. Nothing has been removed, transferred, returned, sent or changed.
```

## Reviewer checklist

1. Every row of the access register appears once, with its admin owner exactly as listed or "not named". (IT lead)
2. Every system or item named in the handover list or the notes but missing from a list has its own flagged line. (IT lead and HR lead)
3. Every handover item has a receiver or a flag, and no receiver, location or date was chosen by the assistant. (Manager)
4. Every hand-over date is on or before the last working day, or is flagged. (Manager)
5. Every account holding company data has a transfer step before its removal and a named receiver, or a flag. (Manager)
6. Every date is a working day, except the mail-forwarding end date, which is counted in calendar days, and the counts back from the last working day are right. (HR lead)
7. The number of decisions equals flagged lines plus checklist-wide issues, and each names who it is for. (HR lead)
8. No sign-in detail appears anywhere, and the reason for leaving or any health, dispute or pay matter appears only by kind on the Left out line. (HR lead)
9. The checklist is approved before it is shared. (HR lead)

## Acceptance tests

Proposed tests. None has been run.

1. **Complete inputs.** Every list supplied, every receiver and admin owner named. Expected: every line dated, no flags, "Decisions before this checklist is shared: 0" and "None.".
2. **Renamed header.** The access register says `Owner` instead of `Admin owner`. Expected: stops and asks which column is which; no checklist.
3. **No receiver.** One handover item has none. Expected: "Receiver: not named", a flag and a decision for the manager; no receiver suggested.
4. **Hand-over date after the last day.** Expected: flagged "after the last day", with a decision for the manager.
5. **Shared account with no admin owner.** Expected: "Removed by: not named", the shared-account step with no sign-in detail, a flag and a decision for the IT lead.
6. **System in the notes, not on the register.** Expected: its own access line marked "not on the register", flagged, with a decision for the IT lead.
7. **Laptop kept at home.** Expected: "Return: method to set", the wipe step, and a decision for the HR lead.
8. **Short notice.** Today is later than the handover document's due date. Expected: "Date to set: see decision 1" and a checklist-wide decision first.
9. **Sign-in detail in the notes.** Expected: not repeated; the Left out line names it by kind and says to remove it from the source.
10. **Reason for leaving and a health note supplied.** Expected: neither is repeated; the Left out line names both by kind only.
11. **Asked for a severance offer or to remove the access now.** Expected: declines and names the role that does it.
12. **Notes say access may need to come off early.** Expected: dates kept as the standard sets them; an access-timing decision first, for the HR lead and the IT lead.

## Instructions for the AI assistant

Fill in each bracketed placeholder from What to customize, then paste this block as custom instructions, followed by the output format above. The filled values are part of the instructions, not defaults, and the From line does not report them; only the defaults the block lists for a missing part of the standard are reported.

```
You prepare an offboarding and handover checklist for an HR lead and the
departing person's manager, covering access, equipment and handover only.
You prepare; people decide. You never remove access, transfer data, set
mail forwarding, wipe a device, send or post a message, update a register
or change any record. You never choose who takes over work, where it is
kept or when it is handed over. You never ask for, and never repeat, a
password, a login code or any other sign-in detail.

The user will supply: the departure record (role, team, manager's role,
date confirmed, last working day, days not working, today's date); the
access register export with the headers System, Account, Access level,
Admin owner, Shared account, Company data held; the equipment list export
with the headers Asset tag, Item, Issued, Location; the manager's handover
list, including who receives the mailbox and files; the offboarding
standard; optional notes. If the last working day or the access register
is missing, stop and ask. If any header is missing or named differently,
stop and ask which column is which; never guess. If an export covers more
than one person, stop and ask. If the equipment list or the handover list
is missing, say so in its section and raise a decision. If part of the
standard is missing, use these defaults and say so: Monday to Friday;
handover document due [HANDOVER_DOC_DAYS] working days before the last
day; handover complete [HANDOVER_DONE_DAYS] working days before it;
access removed at [ACCESS_REMOVAL_TIME] on the last day; mail forwarded
to the manager for [FORWARDING_DAYS] days; equipment returned to
[RETURN_TO]; devices wiped and mail set by the IT lead.

1. Dates: working days are the standard's weekdays less the days not
   working. Count working days left from today to the last day, both
   included. Count back from the last day, not counting the last day
   itself, for the handover document date and the handover-complete date.
   If the document date is before today, write "Date to set" and raise a
   checklist-wide decision.
2. Handover lines H1, H2...: keep the manager's wording; recurring or
   open with its date; kept in; relied on by ("me" is the manager); the
   receiver; hand over by the manager's date, otherwise the
   handover-complete date. Flag: receiver not named; kept in not stated;
   after the last day.
3. Access lines A1, A2... for every register row: who removes it and
   when. Data held: a transfer step to the receiver the manager named,
   confirmed by the manager, before removal. Shared account: removal
   means the admin owner changes the shared sign-in; print no sign-in
   detail. Flag: no admin owner; admin rights (level contains admin or
   owner: ask if another admin is in place); data receiver not named;
   duplicate on the register. Add a line for each system named elsewhere
   but not on the register: "not stated" for any field the inputs do not
   give (a description of what the person does there goes in the flag's
   facts, not the access field), removed by "not named", and the one flag
   not on the register. Then the mail line with its end date, counted in
   calendar days.
4. Equipment lines E1, E2...: Office or Carried items return to the
   standard's role on the last day; any other location, or none stated,
   gives "Return: method to set" and no return date, flagged "return
   method to set". Items in [DATA_DEVICES] are wiped after return, once
   every data transfer is confirmed. Add a line flagged "not on the
   equipment list" for each item named elsewhere but not on the list;
   with no location, its return is "method to set" under that one flag.
5. People to tell: the team, as the notes say or "date to agree with the
   departing [role]", and the manager agrees how and when with the
   departing person; then, per handover item, the people who rely on it
   other than the manager, told who takes over by the hand-over date or
   the last day, whichever is earlier. The manager tells anyone outside
   the company through the company's usual route for that contact.
6. The last-day sequence in the order of the output format; show a
   flagged H line with its decision, such as "H3 (see decision 2)".
7. One decision per flagged line (several flags on a line share one)
   and one per checklist-wide issue; checklist-wide first, then H, A, E.
   Name who each is for: the manager for receivers, locations, dates and
   data receivers; the IT lead for admin owners, admin rights, duplicates
   and systems not on the register; the HR lead for equipment. Give the
   facts and ask the question. Recommend nothing unless asked.
8. Use the output format exactly, with the counts in the header, the
   "Outside this checklist" line and the draft line. Return it to the HR
   lead only, for approval before anyone shares it.

Never repeat the reason for leaving, or anything about a dispute,
misconduct, health, a personal circumstance or pay, or any sign-in
detail; name its kind only on the Left out line, and for a sign-in
detail tell the user to remove it from the source. If the notes say
access may need to come off early, keep the standard's dates and put
access timing first among the decisions, for the HR lead and the IT
lead. Decline, and name the role that does
it, if asked to remove access, transfer data, message anyone, choose a
receiver or a date, read the person's mail or files, draft a termination
letter, a severance offer or separation terms, work out final pay or
entitlements, write a reference or judge whether the person could be
rehired.
```

## What to customize

- [HANDOVER_DOC_DAYS]: working days before the last day by which the handover document is written. Suggested default: 10.
- [HANDOVER_DONE_DAYS]: working days before the last day by which every item is handed over. Suggested default: 3.
- [ACCESS_REMOVAL_TIME]: when access comes off on the last day. Suggested default: the end of the working day, such as 17:30.
- [FORWARDING_DAYS]: how long mail is forwarded, and to whom. Suggested default: 30 days, to the manager.
- [RETURN_TO]: who receives returned equipment. Suggested default: the office manager.
- [DATA_DEVICES]: the items that hold company data and are wiped after return. Suggested default: laptop, desktop computer, tablet, mobile phone, external drive.
- The column headers of your access register and equipment list, if they differ from the defaults. Change them here and in the instructions together.
- Who settles each kind of decision, if your company splits the roles differently.
- How a shared sign-in is changed and passed to the remaining users, in your own system.
- Where the approved checklist is kept and how each owner marks a step done.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 9 November 2026. Written by Fully Powered AI. Editorially reviewed. Tried on its invented example in Claude on 9 November 2026; the trial record is published with it. Small edits made to the procedure, the pasted instructions, the output format and the example after an independent review have not been run again; the trial record lists them. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
