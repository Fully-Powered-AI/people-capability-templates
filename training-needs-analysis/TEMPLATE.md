# Training needs analysis

Workflow template, version 0.1.0.

## Purpose

For one team, or a set of named roles, prepare the training needs analysis an HR lead approves: what each role has to be able to do and to what level, how many people in the role can do it now, where the team falls short today or will by a set date, and the training to arrange, in priority order, each item with how it is delivered, who arranges it, the date it must be done by and its cost where one is known. Everything is counted by role from what the team manager supplies; no person is named, rated or compared. The assistant prepares; it never chooses who attends, enrols or books anyone, buys a course, sends the analysis or changes a training record.

## When to use it and when not to

Use it when a team's work is about to change or has drifted: a new system or process going live, growth that adds people to a role, a run of errors or complaints in one kind of work, a single person holding something the team cannot do without, or certificates coming up for renewal. Run it again when the requirements change or before each training budget is set.

Do not use it:

- to judge a person. It works on counts per role and never rates, ranks or compares named people. A conversation about one person's work belongs to manager feedback preparation, run by their manager;
- for pay, promotion, discipline, dismissal or hiring decisions. It may show that a role needs more people than it has; what to do about that is the manager's decision, made elsewhere;
- to say what a law or a regulator requires. The manager names any rule that requires an ability; the HR lead confirms with whoever advises the company what training satisfies it;
- to design or write the training itself. It says what to arrange, not what the course contains;
- for a whole company at once. Run it one team at a time.

## Roles

- **Runs it and supplies the inputs:** the team manager, or the HR lead working with them.
- **Approves the analysis, the training items and the spend:** the HR lead, or whoever holds the training budget.
- **Arranges outside courses:** the role named in the settings; by default the HR lead. An outside course is any course run by someone outside the team, such as a training centre or a system vendor.
- **Arranges teaching inside the team and supervised practice:** the role named in the settings; by default the team manager.
- **Chooses who attends each item:** the team manager.
- **Confirms that a course satisfies a rule the manager named:** the HR lead, with whoever advises the company.

## Inputs

1. **The scope brief,** from the team manager: the team, the roles in scope, the team manager's role, why the analysis is being done now, and today's date. If no roles are named, or the scope is "everyone" or "the whole company", stop and ask for the named roles. If today's date is missing, stop and ask.
2. **The requirements list,** as a table or CSV, one row per role and ability. Default column headers: `Role,Ability,Importance,Level needed,People who need it,Required by`. `Importance` is `Essential`, `Important` or `Useful`. `Level needed` is a number on the level scale in the settings. `People who need it` is `All` or a number. `Required by` is `None`, or the rule, policy or customer term that requires the ability, in the manager's words. Set each level by what the work demands, not by what the people in the role can do today. If the list is missing, stop and ask for it.
3. **The coverage list,** as a table or CSV, one row per role and ability, in counts and never names. Default column headers: `Role,Ability,People in role,People at level needed,People who can teach it,Evidence,Expires`. `People at level needed` counts the people in the role who can do the ability at or above the level needed today, leaving out anyone known to be leaving before the horizon end. `People who can teach it` counts people in the team at the top level of the scale. `Evidence` says where the count comes from, such as a training record, a certificate register, the manager's observation or an error log. `Expires` is filled only for an ability that rests on a certificate with an end date: one date per holder, as YYYY-MM-DD, separated by semicolons. If the list is missing, stop and ask for it.
4. **The manager's notes,** numbered: what goes wrong and why, changes coming with their dates, courses known with their prices, lengths and session sizes, where people have been shown something but have not done it alone, and the budget. If they are not numbered, number the paragraphs in order and say so on the From line. If there are none, write "none supplied".
5. **The settings.** The approver; the horizon end date; who arranges outside courses; who arranges in-house teaching and practice; the renewal lead time in days; the level scale; who may read the analysis. Anything missing takes these defaults, and the From line names each default used: approver and course arranger, the HR lead; in-house arranger, the team manager; horizon end, six months from today; renewal lead time, 30 days; level scale, 1 Knows what it is, 2 Does it with help, 3 Does it alone, 4 Can teach it; read by, the approver and the team manager.

For either list: if any default header is missing or named differently, stop and ask which column is which; never guess. Extra columns are ignored. Rows in the two lists are matched on role and ability exactly as written.

The assistant works only from what the manager supplies. It needs no connection to the HR system or the training record and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Confirm one team, named roles, today's date and both lists. Check each list's headers against the defaults. Stop on any condition in Exceptions.
2. **Leave out personal details.** Wherever the inputs carry a person's name, an appraisal or performance score, health, pay, a disciplinary matter, a start or leaving date, or another personal circumstance such as an absence, do not repeat it. Use the rest of that note by role, and name each kind left out, with its note or row, on the Left out line. A note that holds nothing but such a detail goes on the Left out line only, not under Also noted.
3. **Match the rows.** Pair each requirement row with its coverage row. A requirement with no coverage row has an unknown count. A coverage row with no requirement row is listed under Also noted and not analysed.
4. **Work out each row,** in the order of the requirements list, grouped by role.
   - **Needed:** `People who need it`, or `People in role` when it says `All`.
   - **At level now:** `People at level needed`.
   - **Expiring by the horizon:** the number of `Expires` dates on or before the horizon end; "none" when `Expires` is blank.
   - **Short:** Needed minus (At level now minus Expiring), and never less than zero. At level now minus Expiring is never taken below zero, so Short is never more than Needed, even when there are more `Expires` dates than people at level. If At level now is blank, Short is "unknown".
   - **Evidence:** as given; "not evidenced" when blank or `None`. An entry that gives a reason for the count rather than a source, such as "System not live yet", is printed as given and is not marked not evidenced.
5. **Flag each row,** on its line in the role-by-ability section. A row may carry several flags, separated by commas.
   - **Single holder:** an Essential ability with exactly one person at level now, whether or not the row is short. A row that is both short and a single holder appears under both and counts in both header totals.
   - **Check first:** a note gives a cause for the shortfall that training will not fix, such as an out-of-date procedure or script, a missing tool, a system fault or too little time.
   - **Not evidenced,** and **unknown count.**
   - **Needs more than the role holds:** Needed is larger than People in role.
   - **Count larger than the role:** At level now is larger than People in role. Treat Short as unknown.
   - **Dates do not match the count:** the number of `Expires` dates differs from At level now. Use the dates given.
   - **Importance not stated,** treated as Important; **level not stated.**
6. **Put the shortfalls in priority order.** A shortfall is a row with Short above zero. An Essential single holder that is not short also takes a place in the order, so that a second person learns it, but is counted under single holders, not shortfalls. Bands, in order: required by a rule (`Required by` is not `None`); Essential; Essential single holder not short; Important; Useful. Within a band, the larger shortfall first, then the earlier done-by date from step 8 (a row with no training item is ordered as if done by the horizon end), then the order of the requirements list. Number them.
7. **Say what closes each one,** taking the first that applies and naming its source:
   - **Check first,** when the row carries that flag. It gets no training item until the approver answers.
   - **Course that meets [the rule],** when it is required by a rule. Name any course the notes give; the HR lead confirms it qualifies.
   - **Course,** when the notes name a course for the ability.
   - **Supervised practice,** when the notes say people have been shown it but have not done it alone.
   - **Taught in-house,** when People who can teach it is one or more.
   - **Not found in the inputs,** otherwise. Raise a question; propose no item.
8. **Write the training items,** one per shortfall in priority order, numbered T1, T2, except where step 7 gave Check first or Not found. Each item gives the ability, how many people in the role and to what level (the shortfall, or one for a single holder not short), how it is delivered, who arranges it (outside courses: the course arranger in the settings; teaching and practice: the in-house arranger), the date it must be done by and the cost.
   - **Done by:** for expiring certificates, each expiry date less the renewal lead time; else a date in the scope brief or the notes when the ability is first needed, such as a go-live; else the horizon end. A done-by date before today is written "already past".
   - **Cost:** only from a price in the notes. Per person: the price times the people. Per session: the price times the sessions needed, using the session size the notes give. Otherwise "not supplied". Never estimate a price.
   - Mark an item "subject to question [n]" when a question below concerns it.
9. **List the single holders,** the certificates running out by the horizon and the rows to check before training, each with its priority number.
10. **Total the costs** supplied, and compare them with the budget when the notes give one. Count the items without a cost.
11. **Write the questions** for the approver, numbered in the priority order of the rows they concern, then any about the whole analysis. One question for each: a course that must meet a rule; an item closed by Course whose notes do not say it brings people to the level needed (whether it does, and what follows if not; the inputs give the course, not its result; a course that must meet a rule has its own question); an item taught in-house when People who can teach it is exactly one (whether that person has the time to teach it by the done-by date; the inputs give the count, not the time); a Check first; a row not evidenced; an unknown count; a shortfall with no way found; needs more than the role holds; count larger than the role; dates that do not match the count; importance or level not stated; costs above the budget. Give the facts with their source and ask. Recommend nothing unless the approver asks.
12. **Also noted:** coverage rows with no requirement row, and any note not used elsewhere, with its number, except a note left out entirely under step 2.
13. **Count and return.** The header counts abilities, shortfalls (and how many are required by a rule), single holders, training items and questions. Return the draft to the person who ran it, for the approver. The approver decides; the manager chooses who attends; people book and buy.

## Exceptions and stop conditions

- **No named roles, the scope is "everyone", or today's date is missing:** stop and ask.
- **No requirements list or no coverage list:** stop and ask. Never supply a standard list of abilities for a role.
- **A default header missing or renamed in either list:** stop and ask which column is which.
- **The same role and ability appear twice in one list:** stop and ask which row stands.
- **The inputs carry names, scores, health, pay, a disciplinary matter or another personal circumstance:** do not repeat them; name the kind on the Left out line.
- **The inputs contain a password, a login code or any other sign-in detail:** do not repeat it; tell the manager to remove it from the source.
- **A role held by one or two people:** the counts can describe people who are easy to identify. Mark a one-person role "one person". For either, keep Read by to the approver and the team manager, and give a single-holder line in that role no note.
- **Asked to rate, rank or compare named people, say who is weakest, or choose who attends:** decline; the analysis describes roles, and the team manager chooses.
- **Asked to use the analysis for a pay, promotion, discipline, dismissal or hiring decision:** decline; those are made elsewhere, by people.
- **Asked what a law or regulator requires, or whether a course satisfies a rule:** decline; write it as a question for the HR lead to confirm with whoever advises the company.
- **Asked to enrol or book anyone, buy a course, send the analysis or update the training record or HR system:** decline and name the role that does it.

## Output format

```
TRAINING NEEDS ANALYSIS: [team]

For: [approver role]. Run by: [team manager role]. Prepared: [today's date]. Horizon: [horizon end date]. Why now: [reason / not stated].
From: requirements list ([n] rows), coverage list ([n] rows), manager's notes ([n] notes / none supplied[, numbered by the assistant]), settings[; defaults used: list].
Read by: [roles].
Roles: [Role] ([n] people[, one person]); [...]. Abilities: [n]. Shortfalls: [n] ([n] required by a rule). Single holders: [n]. Training items: [n]. Questions: [n].
Left out: [kind of detail (note or row); ... / nothing].

ROLE BY ABILITY
Levels: [1 name · 2 name · 3 name · 4 name]

[Role] ([n] people)
- [Ability] · [Importance] · Level [n] · Needed [n] · At level now [n] · Expiring by [horizon]: [n / none] · Short [n / unknown] · Evidence: [as given / not evidenced][ · Required by: [rule]][ · FLAG: [kinds]]

SHORTFALLS IN PRIORITY ORDER
[n]. [Role], [ability]: short [n] of [needed][ by [horizon]]. Why here: [band]. Closed by: [Course that meets [rule] / Course / Supervised practice / Taught in-house / Check first / Not found in the inputs] ([source]).
[None.]

SINGLE HOLDERS
- [Role], [ability]: one person at the level needed[ (note [n]: what it adds)]. Priority [n].
[None.]

CERTIFICATES RUNNING OUT BY [horizon]
- [Role], [ability]: [n] of [n] expire, on [dates]. Renew by [dates]. Priority [n].
[None.]

CHECK BEFORE TRAINING
- [Role], [ability]: [what the note says] (note [n]). See question [n].
[None.]

TRAINING TO ARRANGE
T[n] [Ability]: [n] [role] to level [n]. How: [delivery, with source]. Arranged by: [role]. Done by: [date(s) / already past] ([why]). Cost: [calculation / not supplied]. Closes priority [n][; subject to question [n]].
[None.]
Who attends each item is the [team manager role]'s choice.
Costs supplied: [total] for [n] items, against a budget of [amount] (note [n]) / budget not set. Items without a cost: [n].

QUESTIONS FOR THE [APPROVER ROLE]
[n]. [Priority [n]: ][the facts, with their source.] [The question.]
[None.]

ALSO NOTED
- [Coverage row not on the requirements list / note [n]: what it says.]
[Nothing.]

Draft for the [approver role]'s approval. No one has been named, rated, enrolled or booked; nothing has been bought or sent; no record has been changed.
```

## Reviewer checklist

1. Every row in both lists appears once, matched or listed under Also noted, and every count matches the coverage list. (Team manager)
2. Every Short figure is right: Needed minus (At level now minus Expiring), never below zero. (HR lead)
3. No person is named, rated or compared anywhere, and every kind of personal detail removed is on the Left out line. (HR lead)
4. Every ability marked Required by carries the manager's wording, and nothing says what a law requires. (HR lead)
5. The priority order follows the bands, and every single holder and expiring certificate is listed. (HR lead)
6. Every training item has a delivery with its source, an arranger, a done-by date and a cost or "not supplied", and no price is invented. (HR lead)
7. No training item is proposed for a row marked Check first. (Team manager)
8. Every flag has its question, and the counts in the header agree with the body. (HR lead)
9. The analysis is approved before anyone is enrolled, booked or told. (HR lead)

## Acceptance tests

Proposed tests. None has been run.

1. **Ordinary team.** Two roles, five abilities, two shortfalls, no certificates. Expected: every row worked out, two shortfalls in band order, two training items, no flags.
2. **Certificates expiring.** Six holders, two expiry dates before the horizon end, lead time 30 days. Expected: Expiring 2, Short 2, both renewal dates 30 days before expiry, placed first if required by a rule.
3. **Single holder.** An Essential ability needed by one person, with one at level. Expected: flagged, Short 0, placed in the single-holder band with an item for one more person.
4. **Not a training gap.** A note says errors come from an out-of-date checklist. Expected: Check first, no training item, a question about the checklist.
5. **Names in the notes.** A note names the only person who can do something and mentions sick leave. Expected: content used by role; name and health detail on the Left out line; neither repeated.
6. **Renamed header.** The coverage list says `Headcount` for `People in role`. Expected: stops and asks which column is which.
7. **Scope is everyone.** "Do a training needs analysis for everyone." Expected: stops and asks for named roles; supplies no standard abilities.
8. **Asked to rank people.** "Which of my coordinators is weakest?" Expected: declines; the analysis works on roles.
9. **Asked whether a course satisfies a rule.** Expected: declines; writes it as a question for the HR lead.
10. **No price known.** Taught in-house, no cost in the notes. Expected: "Cost: not supplied", counted under items without a cost.
11. **Over budget.** Supplied costs total more than the budget in the notes. Expected: a question naming both figures; no item dropped.
12. **More people needed than the role holds.** `People who need it` 5, `People in role` 3. Expected: flagged; a question; nothing said about hiring.
13. **Short course, higher level.** The notes name a two-hour session for an ability needed at level 3 and say nothing of what it achieves. Expected: a Course item marked subject to a question asking whether the session brings people to level 3.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare a training needs analysis for one team, for the approver
(by default the HR lead), from what the team manager supplies. You
work on roles and counts. You never name, rate, rank or compare a
person, choose who attends, enrol or book anyone, buy a course, send
anything or change any record. You never ask for a password or a
login code and need no access to any system.

The user will supply: a scope brief (team, roles, team manager, why
now, today's date); a requirements list with the headers
Role,Ability,Importance,Level needed,People who need it,Required by;
a coverage list with the headers Role,Ability,People in role,People
at level needed,People who can teach it,Evidence,Expires (People at
level needed leaves out anyone known to be leaving before the horizon
end; People who can teach it counts people in the team at the top
level of the scale); numbered notes; and settings (approver, horizon
end, who arranges courses, who arranges in-house teaching and
practice, renewal lead time, level scale, who may read it). If no
roles are named or the scope is "everyone", if today's date is
missing, or if either list is missing, stop and ask. If a header is missing or renamed, stop and ask which
column is which; never guess. If one role and ability appear twice in
a list, stop and ask. Never supply a standard list of abilities. If
the notes are not numbered, number the paragraphs in order and say so
on the From line; if there are none, write "none supplied". If the
inputs contain a password, a login code or any other sign-in detail,
do not repeat it and tell the manager to remove it from the source.
Missing settings take these defaults, named on the From line: approver
and course arranger the HR lead; in-house arranger the team manager;
horizon six months from today; renewal lead time 30 days; levels
1 Knows what it is, 2 Does it with help, 3 Does it alone, 4 Can teach
it; read by the approver and the team manager.

1. Do not repeat names, appraisal or performance scores, health, pay,
   disciplinary matters, start or leaving dates or other personal
   circumstances, including an absence. Use the rest of the note by
   role. Name each kind left out, with its note or row, on the Left
   out line. A note that holds
   nothing else goes on the Left out line only.
2. Match requirement and coverage rows on role and ability as written.
   A requirement with no coverage row has an unknown count. A coverage
   row with no requirement goes under Also noted.
3. For each row: Needed is People who need it, or People in role for
   "All". Expiring is the number of Expires dates on or before the
   horizon end, or "none" if blank. Short is Needed minus (At level now
   minus Expiring), never below zero; At level now minus Expiring is
   never below zero either, so Short never exceeds Needed; "unknown" if
   the count is blank.
   Evidence blank or "None" is "not evidenced"; a reason given for the
   count, such as "System not live yet", is printed as given.
4. Flag on the row: single holder (Essential, exactly one at level,
   short or not; a short single holder counts in both header totals);
   check first (a note gives a cause training will not fix, such as an
   out-of-date procedure, a missing tool, a system fault or too little
   time); not evidenced; unknown count; needs more than the role holds;
   count larger than the role (treat Short as unknown); dates do not
   match the count (use the dates given); importance not stated (treat
   as Important); level not stated.
5. Order shortfalls in bands: required by a rule; Essential; then any
   Essential single holder not short; Important; Useful. Within a band:
   larger shortfall, then earlier done-by date (a row with no training
   item counts as done by the horizon end), then list order.
6. Closed by, first that applies: Check first (no training item);
   Course that meets the rule (name any course in the notes); Course
   (the notes name one); Supervised practice (the notes say people
   were shown it but have not done it alone); Taught in-house (someone
   can teach it); otherwise Not found in the inputs (no item, raise a
   question). Name the source of each.
7. Training items T1, T2 in priority order: ability, how many people
   in the role (the shortfall, or one for a single holder not short)
   to what level, how, who arranges it, done by, cost. A course run by
   anyone outside the team, a vendor included, is arranged by the
   course arranger; teaching and practice by the in-house arranger.
   Done by: each certificate's expiry less the lead time; else a date
   in the scope brief or the notes when the ability is first needed;
   else the horizon end; "already past" if before today. Cost only
   from a price in the notes: per person, the price times the people;
   per session, the price times the sessions needed at the session
   size the notes give; else "not supplied". Never estimate a price.
   Total the costs and compare with any budget; count the items
   without a cost. Mark an item "subject to question [n]" when a
   question concerns it.
8. List single holders, certificates running out and rows to check
   first, each with its priority number.
9. Questions for the approver, in priority order of their rows, then
   any for the whole analysis: one for each course that must meet a
   rule; each item closed by Course (not one that must meet a rule)
   whose notes do not say it brings people to the level needed (ask
   whether it does, and what follows if not); each item taught in-house
   when exactly one person can teach it (ask whether that person has
   the time to teach it by the done-by date); check first; not
   evidenced; unknown count; no way found; needs more than the role
   holds; count larger than the role; dates that do not
   match; importance or level not stated; and costs over budget. Give
   the facts and their source. Recommend nothing unless asked.
10. Also noted: coverage rows with no requirement, and every note not
    used elsewhere, with its number, except a note left out entirely
    under step 1.
11. Use the output format exactly; print "None." or "Nothing." for an
    empty section. Make the header counts agree with the body. End
    with the draft line.

If asked to rate, rank or compare people, say who is weakest or choose
who attends, decline: the analysis describes roles. If asked to use it
for a pay, promotion, discipline, dismissal or hiring decision,
decline. If asked what a law requires or whether a course satisfies a
rule, decline and write it as a question for the HR lead. If asked to
enrol, book, buy, send or update a record, decline and name the role
that does it. If a role has one person, mark it "one person". If a
role has one or two people, keep Read by to the approver and the team
manager, and give a single-holder line in that role no note. Check
every figure before you return the draft.
```

## What to customize

- The level scale. By default: 1 Knows what it is, 2 Does it with help, 3 Does it alone, 4 Can teach it. Use your own framework's levels if you have one, and say which number counts as "can teach it".
- The renewal lead time: how many days before a certificate expires the renewal must be done. 30 by default; set it in the settings, or change the default in the instruction block.
- The horizon: the date the analysis looks ahead to, usually the end of the training budget year.
- Who approves, who arranges outside courses and who arranges teaching inside the team.
- The bands. As written, an ability required by a rule always comes first; some companies put a single holder of an Essential ability ahead of everything else.
- What counts as evidence in your company, and whether a manager's observation is enough for an Essential ability.
- Who may read the analysis, and where the approved version is kept.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 9 November 2026. Written by Fully Powered AI. Editorially reviewed. Tried on its invented example in Claude on 9 and 10 November 2026 in three runs: the template was revised after the first, and again after an independent review of the second, and the third is the run recorded. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
