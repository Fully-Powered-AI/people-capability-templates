# Culture health check

Workflow template, version 0.1.0.

## Purpose

Prepare one culture health check for a founder or people lead: the company's stated values written as behaviours someone could watch for, each behaviour read against the evidence the company supplies (survey results, exit notes, how recent decisions were made, what gets recognised), and a reading of where practice matches the values and where it drifts. The check also names the anti-patterns the evidence shows, proposes two or three rituals to try, and lists the questions leadership has to decide. Results are reported for the whole company, by team and by theme, never about a named person. The assistant prepares; it never shares anything with staff, never sends a survey and never decides what changes.

## When to use it and when not to

Use it after a staff survey closes, before an annual values review, when the company has grown or merged and leadership wants to know whether its values still describe how people work, or when exit conversations keep raising the same themes. Run it again after the next survey to see what moved.

Do not use it:

- to judge, rank or compare named people, to say whether one person fits the culture, or to work out who gave a survey answer. Results are by team and theme only;
- for hiring choices, performance ratings, discipline or any decision about one person's employment. The manager and HR own those;
- to look into a complaint, a grievance or the conduct of a named person. HR handles those through its own process, with the advice it needs;
- to announce a change once leadership has decided it. The internal change announcement workflow template prepares that;
- to prepare one manager's feedback conversation with one person. The manager feedback preparation workflow template does that;
- to write the company's values, mission or culture document from scratch. This workflow template reads the values the company already states.

## Roles

- **Runs it:** the founder, the people lead or the head of operations.
- **Leadership:** the founders or leadership team named in the settings. Confirms or rewords the behaviours, chooses which rituals to try, decides what changes and what is shared with staff.
- **Supplier of the evidence:** the person who ran the survey and kept the exit notes, usually the people lead. Removes names from notes before they are supplied where possible.

## Inputs

1. **The stated values,** typed or pasted: each value's name and the description the company uses. Behaviours already written for a value may be added; they are used as supplied.
2. **At least one source of evidence** from the list below. If none is supplied, stop and ask.
   - **The survey export,** one row per team and question, with these default column headers: `period`, `team`, `question`, `respondents`, `agree`, `neutral`, `disagree`. `agree`, `neutral` and `disagree` are counts of people. A team of `All teams` means the row is already a company total. If the headers do not match these, stop and ask which column holds which before reading any row. If a row's three counts do not add up to `respondents`, set that row aside, list it under LEFT OUT and do not use it.
   - **The survey questions:** each question code with its wording. Needed with the export; if it is missing, stop and ask.
   - **The last survey's export,** with the same headers, for the comparison. Optional.
   - **Survey comments,** each with its team and question code. Optional. Used as themes only.
   - **Exit notes:** one note per leaver in the period, with the leaver's team, the month they left and what they said about working here. Optional. Names should be removed before they are supplied; any that remain are removed by the assistant.
   - **Decision notes:** three to ten decisions from the period that changed how people work, each with what was decided, when, who proposed it, who was asked, who decided (as a role), how it was told and to whom. Optional.
   - **Recognition notes:** what people were thanked or recognised for in the period, as counts by theme, without names. Optional.
3. **The settings:** company name; headcount and number of teams; today's date; the period the evidence covers; who leadership is; the rituals already in place; whether the last survey's results were shared with staff; [your smallest group] (default 5); [your match threshold] (default 70 per cent agree); [your drift threshold] (default 50 per cent agree); [your team gap] (default 10 points); [your notable change] (default 10 points). If some or all are missing, use the defaults and say in the header which were defaulted. Without a headcount, the ritual menu is used without its size bands, and the header says so.

The assistant works only from what is supplied. It needs no connection to a survey tool, an HR system or a chat channel and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Confirm the values and at least one source of evidence. Check the survey export's headers against the defaults. Check every row's counts. If the survey's total respondents across all teams are fewer than [your smallest group], stop: the results cannot be reported without pointing to people.
2. **Remove names.** Delete every person's name from what you will use: exit notes, comments, decision notes and recognition notes. Keep the theme without the name and record under LEFT OUT that a name was removed and from which kind of input, never the name itself. Describe decisions by the role that made them. If a note is about one person's health, a complaint, discipline or a dispute, leave the note out entirely and say under LEFT OUT that one note was left out for that reason.
3. **Set the groups.** A team with at least [your smallest group] respondents is reported on its own. Combine every team below that size into one group; if the combined group is still below it, add the next smallest team. A combined group is named by its teams, for example "Client Services and Operations (combined)". If only company totals are supplied, there is no view by team.
4. **Number the evidence.** Every piece is cited by its number throughout.
   - **S[n]** for each survey question: company agree count over company respondents, the share to a whole per cent (halves round up), and the last survey's share if supplied. Work every share from counts, never by averaging teams' percentages.
   - **X[n]** for each exit theme: group the notes into themes; count how many leavers raised each, out of all leavers in the period. A theme raised by two or more leavers counts; one raised by a single leaver is noted only. Mark each theme as a concern or as something valued. Exit themes are reported for the whole company only, never by team or by note, and never quoted.
   - **C[n]** for each comment theme, counted the same way: two or more comments count, one is noted only. Never quote a comment.
   - **D[n]** for each decision note, in plain words, with the role that decided.
   - **R[n]** for each recognition theme, with its count out of all recognitions.
   A theme or survey question that bears on none of the values goes under OTHER SURVEY RESULTS or is marked "outside the stated values".
5. **Write the values as behaviours.** For each value, two or three behaviours someone new could watch for in an ordinary week, each describing something a person does and when they do it, and one line saying what the value does not look like. Use the company's own behaviours where supplied and mark them "supplied". Otherwise draft them from the value's description, the decision notes and the recognition notes, and mark them "draft for leadership to confirm". Number the behaviours B1, B2 and on. Never write a behaviour about a named person.
6. **Read each behaviour against the evidence.** List the evidence that bears on it and say in a few words how. Sort each item:
   - **For:** a survey question at or above [your match threshold]; an exit or comment theme valued by two or more people; a decision note that shows the behaviour; a recognition theme with two or more recognitions that describe the behaviour.
   - **Against:** a survey question below [your drift threshold]; a concern raised by two or more leavers or comments; a decision note that shows what the value does not look like.
   - **Noted, not counted:** a survey question between the two thresholds, a theme from one person, a recognition theme with fewer than two recognitions or that does not describe the behaviour.
   A survey question is sorted by its company share; a group's share shows only on the team gap line. A decision note that shows the behaviour for one team and what the value does not look like for another is listed under both For and Against, each saying which team it concerns.
   Then give the reading:
   - **Drifts:** at least one item against and none for, or two or more against and more against than for.
   - **Matches:** at least one item for and none against.
   - **Mixed:** items both for and against that do not meet the drift rule, or only survey questions between the thresholds.
   - **Not enough evidence:** nothing for or against and no survey question between the thresholds.
   Under each behaviour, add a team gap line for every reported group whose share on a question the behaviour cites is at least [your team gap] points below the company share. A team gap is reported, not counted in the reading. A team result describes how that group experiences its work; it is never a verdict on its manager or any person.
7. **Show the view by team.** For each survey question, the company share and each reported group's share, and any gap of [your team gap] points or more.
8. **Compare with the last survey.** For each question in both surveys, the change in whole percentage points between the rounded shares. List first every fall of [your notable change] points or more, largest first, then the rest in question order. Keep a large fall visible on its own line rather than inside an overall figure.
9. **Look for anti-patterns.** Check each one on this list. Name one as spotted only when at least two different numbered items show it; with one item, list it as "one sign only"; otherwise list it as not seen.
   - **Values in name only:** more than half of recognitions are for something no stated value names, or decision notes show choices the values argue against with no reason given. Either clause can supply an item: the first, when met, is one item however many recognition themes it draws on, and each decision note that meets the second is one item. A decision note meets the second clause only when the company's own description of a value argues against the choice; a behaviour the assistant drafted is not enough.
   - **Bad news unwelcome:** a survey question about raising problems is below [your match threshold] in any reported group, or two or more leavers or comments say raising a problem was held against them. When a group's share and an exit or comment theme are both cited, here or in a ritual, give the theme as company-wide and never put it in the same sentence or line as the named group.
   - **Decisions out of sight:** decisions that change people's work made without asking anyone affected, or told without reasons, or reaching a team late or second-hand.
   - **Culture left to spread by itself:** the company has more than 15 people and the settings name no onboarding practice and no regular meeting where the values come up.
   - **Habits from a smaller company:** a way of working that suited far fewer people now causes friction the evidence shows, such as every team-level choice waiting for a founder.
   - **Results never shared back:** the settings say the last survey's results were not shared with staff, or a theme says nothing changed after a survey.
   - **Uneven standards:** two or more items say the same rule applies differently by team or seniority. Report the team or level, never a person.
10. **Choose two or three rituals.** From the menu below, choose rituals that answer the behaviours that drift or are mixed and the anti-patterns spotted, that suit the headcount band, and that are not already in place. Never more than three. For each, say what it answers, how often, which role runs it, roughly how long it takes (the menu's typical time, a planning guide rather than a fact about the company), and what to watch at the next survey or in the next exit notes. Name no target figure. If the cap of three leaves a behaviour that drifts or is mixed, or a spotted anti-pattern, unanswered, raise it as a question for leadership.
    - **End-of-week round** (under 15 people): a short Friday circle where everyone says what they would do differently next week, alongside anything that went right. Typical time: about 15 minutes a week. Answers: raising problems; bad news unwelcome.
    - **Problem first** (any size): each weekly team meeting opens with one problem someone has noticed; the lead thanks whoever raised it and agrees who looks into it. Typical time: about five minutes of each weekly meeting. Answers: raising problems; bad news unwelcome.
    - **Values in recognition** (any size): each thank-you names the value it shows, and once a month the lead reads back which values were recognised and which were not. Typical time: a line on each thank-you and about 15 minutes a month for the read-back. Answers: values in name only.
    - **Survey read-back** (any size): soon after a survey closes, leadership tells staff what the company-wide results said and what it has chosen to act on, then says at the following all-hands what has happened since. Typical time: about half an hour at each of the two all-hands. Answers: results never shared back.
    - **Decision notes in the open** (15 people or more): before a decision that changes a team's work takes effect, leadership posts what was decided, why, who was asked and when it starts. Typical time: about ten minutes a decision. Answers: reasons for decisions; decisions out of sight.
    - **Hand-off owners** (15 people or more): in each weekly meeting the team lists work it has passed to or received from another team and names who owns each item until it closes. Typical time: about five minutes of each weekly meeting. Answers: ownership across teams.
    - **Founders' open hour** (15 to 200 people): a standing hour each fortnight when anyone can bring a founder a question or a concern. Typical time: one hour a fortnight. Answers: decisions out of sight; bad news unwelcome.
    - **Month-in conversation** (15 people or more): around four weeks in, a new starter compares what they were told before joining with what they have found, in a conversation with someone senior outside their own reporting line. Typical time: about half an hour for each new starter. Answers: culture left to spread by itself; habits from a smaller company.
    - **Cross-team culture group** (50 people or more): a small group drawn from several teams, with members replaced on a set rotation, reads each culture health check and takes its own proposals to leadership. Typical time: about an hour a month for each member. Answers: uneven standards; culture left to spread by itself.
11. **List the questions for leadership.** Always: confirm, reword or replace any drafted behaviours; which rituals, if any, to try and who owns each; what to share with staff and when. Add: any decision the evidence shows is still open with no owner; any behaviour with not enough evidence, and whether to add a survey question for it next time; any behaviour that drifts or is mixed, or spotted anti-pattern, that no chosen ritual answers.
12. **Run the final checks.** No person's name anywhere in the check; no group smaller than [your smallest group] shown; no exit theme tied to a team or a note, or put in the same sentence or line as a named group; every reading cites its numbered items; every figure recomputed from the counts. Return the check to the person who ran it. Leadership decides what changes.

## Exceptions and stop conditions

- **No values, or no evidence at all:** stop and ask.
- **Survey export headers do not match the defaults:** stop and ask which column holds which.
- **Survey export without the question wording:** stop and ask.
- **Fewer respondents in total than [your smallest group]:** stop; the results cannot be reported without pointing to people.
- **A row's counts do not add up:** set the row aside, list it under LEFT OUT, and continue without it.
- **Asked to say who gave an answer, to show a group smaller than [your smallest group], or to break exit themes down by team:** decline.
- **Asked to judge, rank or compare named people, to say whether a person fits the culture, or to help with a hiring choice, a rating or discipline:** decline; those belong to the manager and HR.
- **A note describes a complaint, a grievance, discipline, a dispute or one person's health:** leave it out without repeating it and tell the person who ran it to take it to HR.
- **Asked to decide what changes, to promise staff an outcome, or to write a message to staff:** decline; leadership decides, and any message is drafted separately and sent by a person.
- **Asked to send a survey, post results or share the check:** decline; a person shares it once leadership has approved.
- **The inputs contain a password, a login code or bank details:** do not repeat them, and tell the person to remove them from the source.

## Output format

```
CULTURE HEALTH CHECK: [company], [period]

For: [role who ran it]. Leadership decides: [who]. Prepared [weekday date].
Read from: [n] values; [survey export ([n] rows, [n] respondents, [n] teams) / no survey]; [last survey ([n] rows, [n] respondents) / no earlier survey]; [exit notes ([n] leavers) / no exit notes]; [decision notes ([n]) / no decision notes]; [recognition notes ([n] recognitions) / no recognition notes]; [survey comments ([n]) / no survey comments]. Settings: [as supplied / defaults used for [what was not supplied]].
Behaviours: [n]. Matches: [n]. Mixed: [n]. Drifts: [n]. Not enough evidence: [n]. Anti-patterns spotted: [n]. Rituals to try: [n]. Questions for leadership: [n].

THE EVIDENCE
S[n]. [Code] "[wording]". Company: [agree] of [respondents] agree ([share]%). Last survey: [share]% / not supplied.
X[n]. Exit theme: [theme]. Raised by [n] of [n] leavers. [Counts / Noted only]. [Concern / Valued][; outside the stated values].
C[n]. Comment theme: [theme]. [n] comments. [Counts / Noted only]. [Concern / Valued].
D[n]. [Month]: [what was decided]. Proposed by: [role]. Asked: [who / no one outside the deciders]. Decided by: [role / no one: still open]. Told: [how and to whom / not applicable].
R[n]. Recognition: [n] of [n] were for [theme].
[Write "none supplied" under any kind of evidence that was not supplied.]

VALUES AS BEHAVIOURS
[Value]: "[the company's description]"
B[n]. Looks like: [behaviour]. ([supplied / draft for leadership to confirm])
Does not look like: [one line].

WHERE PRACTICE MATCHES AND WHERE IT DRIFTS
B[n]. [Behaviour, short]. Reading: [Matches / Mixed / Drifts / Not enough evidence].
For: [item: how it bears / none].
Against: [item: how it bears / none].
Noted, not counted: [item: why / none].
Team gap: [group, share% against company share%, on S[n] / none].

BY TEAM
Groups reported: [group ([n] respondents), ...]. [Combined: [teams], because [team] had [n] respondents, below [smallest group]. / No team combined. / Company totals only: no view by team.]
S[n]: company [share]%; [group] [share]%; [...]. [Gap: [group], [n] points below. / No gap.]

CHANGE SINCE THE LAST SURVEY
[Notable falls, largest first, then the rest in question order:]
S[n]: [last]% to [now]% ([+/-n] points)[. Notable fall.]
[or: No earlier survey supplied.]

OTHER SURVEY RESULTS
S[n]: [share]%[, [+/-n] points since the last survey]. Bears on none of the stated values.
[or: none]

ANTI-PATTERNS
Spotted:
[n]. [Name]. Evidence: [item numbers]. Here: [one line drawn from those items].
[or: none]
One sign only: [name]: [item]: [one line]. / none
Not seen: [names, each with the reason where the inputs give one].

RITUALS TO TRY
[n]. [Ritual]. Answers: [B numbers; anti-pattern]. How often: [...]. Run by: [role]. Takes: [the menu's typical time]. Watch: [survey question or evidence to look at next time].
[or: none: no behaviour drifts or is mixed and no anti-pattern was spotted.]

QUESTIONS FOR LEADERSHIP
[n]. [Question], with the items it rests on.

LEFT OUT
[Names removed (from which kind of input), notes left out and why, teams combined, rows set aside, themes outside the stated values, requests declined.]
[or: none]

Prepared for [role who ran it]. [Leadership] decides what changes and what staff are told. Nothing has been shared with staff, sent or posted, and no record has been changed.
```

## Reviewer checklist

1. No person is named anywhere in the check, and no exit theme or comment is tied to a team, a note or a quotation. (Person who ran it)
2. No group smaller than the smallest group is shown, and a single small team is never shown in a way that lets it be worked out from the others. (Person who ran it)
3. Every share is recomputed from the counts, the company figures come from counts rather than averaged percentages, and every change matches the rounded shares. (Person who ran it)
4. Every reading cites numbered items, each item is sorted for, against or noted by the stated thresholds, and the reading follows the rules. (Person who ran it)
5. Every behaviour is something a newcomer could actually see in an ordinary week, and drafted ones are marked for leadership to confirm. (Leadership)
6. Every anti-pattern named as spotted rests on at least two different items. (Person who ran it)
7. The rituals answer what drifts or is mixed, suit the company's size, are not already in place, and promise no result. (Leadership)
8. Nothing in the check decides a change, judges a person or reads as a message to staff. (Leadership)

## Acceptance tests

Proposed tests. None has been run.

1. **Ordinary run.** Three values, a survey export for four teams, the last survey's totals, six exit notes and four decision notes. Expected: evidence numbered, six to nine behaviours drafted and marked for confirmation, every reading cited, a view by team, the comparison with the largest fall first, two or three rituals, questions for leadership.
2. **Wrong headers.** The export has `Dept, Item, N, Positive, Neutral, Negative`. Expected: stops and asks which column holds which; reads no row.
3. **Small team.** One team has three respondents. Expected: combined with the next smallest team; never shown alone; noted under LEFT OUT.
4. **Two small teams.** Two teams have two respondents each. Expected: combined into one group of four, still below five, so the next smallest team is added.
5. **Counts that do not add up.** A row has 10 respondents and 6, 2 and 1 in the counts. Expected: row set aside and listed; shares worked without it.
6. **A name in the exit notes.** A note names the leaver's manager. Expected: name removed; theme kept; LEFT OUT says a name was removed from the exit notes, without the name.
7. **One leaver's theme.** A concern raised by one leaver. Expected: noted only; never counted against a behaviour.
8. **Asked who answered.** "Which of the Operations team disagreed?" Expected: declines.
9. **Asked about a person.** "Is our sales lead a culture fit?" Expected: declines; names the manager and HR.
10. **A complaint in the notes.** An exit note describes a complaint about a named colleague. Expected: note left out without repeating it; the person is told to take it to HR.
11. **Anti-pattern on one sign.** Recognitions are mostly for deadlines and nothing else points to values in name only. Expected: listed as one sign only, not as spotted.
12. **No evidence for a behaviour.** Expected: reading "Not enough evidence" and a question for leadership about adding a survey question.
13. **Asked to send results to staff.** Expected: declines; a person shares them once leadership approves.
14. **No survey at all.** Exit notes and decision notes only. Expected: runs; survey sections say no survey; readings rest on the other evidence.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above and the ritual menu from step 10 of the procedure.

```
You prepare one culture health check for a founder or people lead: the
company's stated values written as behaviours, each read against the
evidence supplied, with anti-patterns, two or three rituals to try and
questions for leadership. You prepare; leadership decides. You never
share anything with staff, never send a survey or post results, never
change a record and never decide what changes. You never judge, rank or
name a person, never say who gave an answer, and never help with hiring,
ratings or discipline. You never ask for a password or a login code and
need no access to any system.

The user will supply: the stated values (name and description, with any
behaviours already written); at least one source of evidence (a survey
export with headers period, team, question, respondents, agree, neutral,
disagree, as counts, plus the question wording; the last survey's export;
survey comments; exit notes, one per leaver; decision notes; recognition
counts by theme); and the settings (company, headcount, teams, today's
date, period, who leadership is, rituals in place, whether the last
results were shared, smallest group (default 5), match threshold
(default 70% agree), drift threshold (default 50%), team gap (default 10
points), notable change (default 10 points)). If the values or all
evidence are missing, stop and ask. If the export's headers differ, stop
and ask which column holds which. If the export comes without question
wording, stop and ask. If total respondents are below the smallest
group, stop. If a row's counts do not add up to respondents, set it
aside and list it. A team of "All teams" is a company total. Say in the
header which settings were defaulted.

1. Remove every person's name from everything you use; keep the theme.
   Describe decisions by role. Leave out entirely any note about a
   complaint, a grievance, discipline, a dispute or one person's health,
   and tell the person to take it to HR. Record removals under LEFT OUT
   without the name.
2. Groups: a team at or above the smallest group is shown alone.
   Combine all smaller teams into one group; if still too small, add the
   next smallest team. Never show a group below the smallest group.
3. Number the evidence. S: each question, company agree over company
   respondents from counts, whole per cent, halves up, with the last
   survey's share. X: exit themes, counted as leavers raising each out of
   all leavers; two or more counts, one is noted only; company-wide
   only, never by team or note, never quoted; mark concern or valued.
   C: comment themes, counted the same way, never quoted. D: decisions,
   with the deciding role. R: recognition themes with counts. Mark
   anything that bears on no value.
4. Behaviours: two or three per value that a newcomer could see in an
   ordinary week, each saying what a person does and when, plus
   one "does not look like" line. Use supplied behaviours as given;
   otherwise draft and mark "draft for leadership to confirm". Number
   them B1, B2 and on.
5. Readings. For each behaviour, list the items that bear on it and how.
   For: a question at or above the match threshold; a valued theme from
   two or more; a decision showing the behaviour; a recognition theme of
   two or more that describes it. Against: a question below the drift
   threshold; a concern from two or more; a decision showing what the
   value does not look like. Noted: a question between thresholds; a
   one-person theme; a recognition theme under two or not describing it.
   Sort a question by its company share; group shares show only on team
   gap lines. A decision showing the behaviour for one team and its
   opposite for another goes under both For and Against, each saying
   which team it concerns.
   Drifts: against and no for, or two or more against and more against
   than for. Matches: for and no against. Mixed: both, not meeting
   drifts, or only between-threshold questions. Not enough evidence:
   nothing else. Add a team gap line for any group at least the team gap
   below the company share on a cited question; it is not counted, and
   it is never a verdict on a manager or anyone else.
6. By team: each question's company share and each group's share, with
   gaps. Change: each question's change between rounded shares; falls of
   the notable change or more first, largest first, then question order.
   Keep a large fall on its own line, never inside an overall figure.
7. Anti-patterns. Check each of these seven:
   Values in name only: more than half of recognitions are for
   something no value names (one item), or a decision note makes a
   choice a value's own description argues against, with no reason
   given (one item each); never rest it on a behaviour you drafted.
   Bad news unwelcome: a question on raising problems is below the
   match threshold in any group, or two or more leavers or comments say
   raising a problem was held against them.
   Decisions out of sight: decisions that change people's work made
   without asking anyone affected, told without reasons, or reaching a
   team late or second-hand.
   Culture left to spread by itself: more than 15 people and the
   settings name neither an onboarding practice nor a regular meeting
   where the values come up.
   Habits from a smaller company: a way of working that suited far
   fewer people now causes friction the evidence shows, such as every
   team-level choice waiting for a founder.
   Results never shared back: the last results were not shared with
   staff, or a theme says nothing changed after a survey.
   Uneven standards: two or more items say a rule applies differently
   by team or seniority; name the team or level, never a person.
   Spotted needs two different items; one item is "one sign only";
   otherwise not seen, with the reason where the inputs give one.
   Cite an exit or comment theme company-wide and never in the same
   sentence or line as a named group, here or in a ritual.
8. Rituals: two or three from the ritual menu pasted below that answer what
   drifts or is mixed and the anti-patterns spotted, fit the headcount
   band and are not already in place. For each: what it answers, how
   often, the role that runs it, the menu's typical time, what to watch
   next time. No target figures, no promised results. If the cap of
   three leaves a drift, a mixed behaviour or a spotted anti-pattern
   unanswered, raise it as a question for leadership.
9. Questions for leadership: confirm or reword drafted behaviours; which
   rituals and who owns them; what staff are told and when; any open
   decision with no owner; any behaviour short of evidence and whether
   to add a survey question; anything no chosen ritual answers.
10. Check: no names, no small group shown, no exit theme tied to a team
   or set beside a named group, every reading cited, every figure
   recomputed from counts.

Use the output format exactly; where a section has nothing, write its
empty wording. End with the line saying leadership decides and nothing
has been shared with staff, sent or posted. If asked to show who
answered, judge a person, decide a change, promise staff an outcome or
send anything, decline and say who decides.
```

## What to customize

- [your smallest group]: five is a careful floor; raise it if your teams are small or close-knit.
- [your match threshold], [your drift threshold], [your team gap] and [your notable change], so the readings match how your company reads its own survey.
- Your survey's column headers, if your survey tool exports different ones, and your question wording mapped to your values once, so every run reads the same questions the same way.
- Your values and, once leadership has confirmed them, your behaviours, supplied as written so the drafts are no longer needed.
- The ritual menu: remove anything that would not suit your company and add rituals you already trust.
- Who leadership is, who sees the check, and who decides what is shared with staff.
- Which exports the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI. Not yet tested in a client environment.
