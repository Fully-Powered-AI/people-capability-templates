---
name: "culture-health-check"
description: "Prepare one culture health check for a founder or people lead: the company's stated values written as behaviours someone could watch for, each behaviour read against the evidence the company supplies (survey results, exit notes, how recent decisions were made, what gets recognised), and a reading of where practice matches the values and where it drifts. The check also names the anti-patterns the evidence shows, proposes two or three rituals to try, and lists the questions leadership has to decide. Results are reported for the whole company, by team and by theme, never about a named person. The assistant prepares; it never shares anything with staff, never sends a survey and never decides what changes."
license: "MIT"
metadata:
  version: "0.1.0"
  publisher: "Fully Powered AI"
  template: "Culture health check"
---

# Culture health check

This is the technical file for a Fully Powered workflow template. It carries the instructions an AI product follows. The complete template, with roles, inputs, exceptions, the reviewer checklist, acceptance tests and what to customize, is in [TEMPLATE.md](TEMPLATE.md). A worked example with invented data is in [EXAMPLE.md](EXAMPLE.md).

## Instructions

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

## Before relying on it

Decide every item under "What to customize" in TEMPLATE.md and set the limits the instructions in this file leave open, written in square brackets such as [N], to your own. Then run the acceptance tests in TEMPLATE.md on past work. A person starts this work, supplies the inputs and decides what happens with the result.
