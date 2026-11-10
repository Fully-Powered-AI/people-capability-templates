# Culture health check: trying the template on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

This trial used only the invented example's inputs: the company, the people, the survey and every figure are made up, and no client data was used. The run was a single pass. The model that ran it did not write the template. It read the whole of `member/template.md`, including the procedure's anti-pattern list, and followed the instruction block and the output format on the eight inputs in `public/example.md` (settings, stated values, survey questions, the October survey export, the April survey export, exit notes, decision notes and recognition notes). It did not read the example's output until it had finished its own.

**Edited after this run, 10 November 2026.** Following the independent review, the template and the published example were edited after the run recorded here, and the run was not repeated. The output and the observations below are left as recorded, so where they describe the template or the example they describe them as they were at the time of the run. What changed:

- The instructions for the AI assistant now carry a one-line test for each of the seven anti-patterns, which before were listed there by name only.
- "Values in name only" now says that each of its two conditions can supply one of the two items, and that a decision note counts only when the company's own description of a value argues against the choice, not a behaviour the assistant drafted. This settles point 5 below. This run's second item, D1, rested on its own drafted behaviour B2, so under the rule as now written the run would have listed "Values in name only" as one sign only, with two anti-patterns spotted.
- An exit or comment theme is now cited company-wide and never in the same sentence or line as a named group, in the anti-patterns or a ritual. This settles point 6 below; this run already wrote it that way. The example's "Bad news unwelcome" line and its "Problem first" ritual were rewritten to match, and that ritual now runs in every team's weekly meeting, as in this run.
- The readings now say that a survey question is sorted by its company share, which is what this run did (point 2), and that a decision note showing a behaviour for one team and its opposite for another is listed under both For and Against (point 3). Under that rule this run's B2 would list D3 on both sides and still read Drifts. The example's B2 now lists D3 on both sides; before, it listed D3 as against only.
- Each ritual on the menu now gives a typical time, and the output's "Takes" is that typical time, a planning guide rather than a fact about the company. This run's figures (about ten minutes a decision, about five minutes of a weekly meeting) match the menu's. This settles the first half of point 10.
- When the cap of three rituals leaves a drift, a mixed behaviour or a spotted anti-pattern unanswered, it is now raised as a question for leadership, which is what this run did. This settles the second half of point 10.
- In the example, D3 no longer counts for B1, since the problem was raised the week after the second dispute rather than the week it was spotted; B1 still reads Mixed. The example's D4 line now uses the format's wording, "no one: still open".
- The opening paragraph's description of what the run read was corrected: the run read the whole template, as observations 5 and 7 show.

## What came out

This is the check as produced, before it was compared with the published example.

```
CULTURE HEALTH CHECK: Harrowfinch Studio, October 2026 survey

For: People lead. Leadership decides: the two founders. Prepared Tuesday 10 November 2026.
Read from: 3 values; survey export (24 rows, 52 respondents, 4 teams); last survey (6 rows, 48 respondents); exit notes (6 leavers); decision notes (4); recognition notes (9 recognitions); no survey comments. Settings: defaults used for the smallest group (5), the match threshold (70%), the drift threshold (50%), the team gap (10 points) and the notable change (10 points).
Behaviours: 6. Matches: 1. Mixed: 2. Drifts: 2. Not enough evidence: 1. Anti-patterns spotted: 3. Rituals to try: 3. Questions for leadership: 6.

THE EVIDENCE
S1. Q1 "I can tell my manager about a problem without worrying how it will land." Company: 37 of 52 agree (71%). Last survey: 75%.
S2. Q2 "I know what the studio is aiming for this quarter and how my work fits in." Company: 33 of 52 agree (63%). Last survey: 60%.
S3. Q3 "When a decision affects my work, I hear why it was made." Company: 23 of 52 agree (44%). Last survey: 65%.
S4. Q4 "When work crosses into another team, someone still sees it through to the end." Company: 30 of 52 agree (58%). Last survey: 58%.
S5. Q5 "Work is checked properly before a client sees it." Company: 42 of 52 agree (81%). Last survey: 81%.
S6. Q6 "I would tell a friend this is a good place to work." Company: 34 of 52 agree (65%). Last survey: 69%.
X1. Exit theme: raising a problem was held against the person who raised it. Raised by 2 of 6 leavers. Counts. Concern.
X2. Exit theme: changes made without reasons, or heard of late. Raised by 3 of 6 leavers. Counts. Concern.
X3. Exit theme: work passed between teams with no owner. Raised by 1 of 6 leavers. Noted only. Concern.
X4. Exit theme: work reviewed before clients see it, and the quality bar. Raised by 2 of 6 leavers. Counts. Valued.
X5. Exit theme: pay below other agencies. Raised by 1 of 6 leavers. Noted only. Concern; outside the stated values.
X6. Exit theme: no clear path to promotion. Raised by 1 of 6 leavers. Noted only. Concern; outside the stated values.
C. Comment themes: none supplied.
D1. June 2026: Engineering reorganised into two groups by product line. Proposed by: the founders. Asked: no one outside the deciders. Decided by: the two founders, in one leadership meeting. Told: all staff, by message on the day it took effect, with no reasons given.
D2. August 2026: a peer review step added before any client delivery. Proposed by: the design leads. Asked: Design and Engineering, in a joint team meeting. Decided by: the head of design, two weeks later. Told: Design and Engineering, in their team meeting before the step began, with reasons written up.
D3. September 2026: the studio stopped work for one client after repeated scope disputes. Proposed by: a Client Services account lead, at the weekly meeting the week after the second dispute. Asked: Client Services, for the history. Decided by: the two founders, within a week. Told: Client Services, in its team meeting, with reasons; Engineering was not told and found out when the client's tickets stopped.
D4. October 2026: who picks up out-of-hours support requests between Client Services and Engineering. Proposed by: both team leads. Asked: both teams, in two meetings. Decided by: no one: still open. Told: not applicable.
R1. Recognition: 6 of 9 were for working late or over a weekend.
R2. Recognition: 2 of 9 were for passing on praise from a client.
R3. Recognition: 1 of 9 was for helping another team with a problem.

VALUES AS BEHAVIOURS
Candour: "We say what we see, early."
B1. Looks like: when someone notices a problem in client work or a plan, they raise it with the person who can act on it in the same week, and it is heard without being held against them. (draft for leadership to confirm)
B2. Looks like: when a decision changes a team's work, the team is told the reason at the same time as the decision. (draft for leadership to confirm)
Does not look like: a problem kept quiet until a client forces it out, or a change announced on the day it starts with no reasons.
Ownership: "We see things through."
B3. Looks like: when work passes from one team to another, each item has a named owner until it closes. (draft for leadership to confirm)
B4. Looks like: when a problem is raised in a team meeting, someone is named to look into it and the team hears back. (draft for leadership to confirm)
Does not look like: a question discussed in two meetings with no one named to own it.
Craft: "We make work we are proud of."
B5. Looks like: before work goes to a client, a colleague who did not make it checks it. (draft for leadership to confirm)
B6. Looks like: when a piece of work is good, someone says so to the people who made it and says what was good about it. (draft for leadership to confirm)
Does not look like: work sent to a client unchecked because of a deadline, or thanks that are only ever for hours.

WHERE PRACTICE MATCHES AND WHERE IT DRIFTS
B1. Problems raised in the week and heard. Reading: Mixed.
For: S1: 71% agree, at or above 70%. D3: the scope disputes were raised at the weekly meeting and acted on within a week.
Against: X1: 2 of 6 leavers said raising a problem was held against them.
Noted, not counted: none.
Team gap: Client Services and Operations (combined), 56% against company 71%, on S1.

B2. Teams hear the reason when a decision changes their work. Reading: Drifts.
For: D2: reasons for the review step were written up and given to both teams before it began.
Against: S3: 44% agree, below 50%. X2: 3 of 6 leavers raised changes made without reasons or heard of late. D1: the June reorganisation was announced on the day it took effect with no reasons.
Noted, not counted: D3: Client Services was told with reasons, but Engineering was not told; the item shows the behaviour and its opposite, so it is not counted either way.
Team gap: none.

B3. Work passed between teams keeps a named owner. Reading: Drifts.
For: none.
Against: D4: out-of-hours support between Client Services and Engineering was discussed in two meetings and has no owner.
Noted, not counted: S4: 58% agree, between the thresholds. X3: one leaver raised work moving between teams with no owner.
Team gap: Engineering, 44% against company 58%, on S4.

B4. Problems raised in a meeting get a named owner and a report back. Reading: Mixed.
For: D3: raised at the weekly meeting, the founders asked for the history, decided within a week and told the team that raised it.
Against: D4: two meetings, no owner named.
Noted, not counted: none.
Team gap: none.

B5. Client work is checked by a colleague first. Reading: Matches.
For: S5: 81% agree, at or above 70%. X4: 2 of 6 leavers valued the review and the quality bar. D2: a peer review step before client delivery was added.
Against: none.
Noted, not counted: none.
Team gap: none.

B6. Good work is noticed and the reason said. Reading: Not enough evidence.
For: none.
Against: none.
Noted, not counted: R1: 6 of 9 recognitions were for working late or over a weekend, which does not describe this behaviour. R2: 2 of 9 passed on client praise, but the note does not say what the praise was for. R3: one recognition, fewer than two.
Team gap: none.

BY TEAM
Groups reported: Design (20 respondents), Engineering (16), Client Services and Operations (combined, 16). Combined: Client Services and Operations, because Operations had 4 respondents, below 5, and was still below 5 alone, so the next smallest team, Client Services, was added.
S1: company 71%; Design 75%; Engineering 81%; Client Services and Operations 56%. Gap: Client Services and Operations, 15 points below.
S2: company 63%; Design 60%; Engineering 56%; Client Services and Operations 75%. No gap.
S3: company 44%; Design 45%; Engineering 44%; Client Services and Operations 44%. No gap.
S4: company 58%; Design 70%; Engineering 44%; Client Services and Operations 56%. Gap: Engineering, 14 points below.
S5: company 81%; Design 85%; Engineering 81%; Client Services and Operations 75%. No gap.
S6: company 65%; Design 70%; Engineering 69%; Client Services and Operations 56%. No gap (9 points below).

CHANGE SINCE THE LAST SURVEY
S3: 65% to 44% (-21 points). Notable fall.
S1: 75% to 71% (-4 points)
S2: 60% to 63% (+3 points)
S4: 58% to 58% (0 points)
S5: 81% to 81% (0 points)
S6: 69% to 65% (-4 points)

OTHER SURVEY RESULTS
S2: 63%, +3 points since the last survey. Bears on none of the stated values.
S6: 65%, -4 points since the last survey. Bears on none of the stated values.

ANTI-PATTERNS
Spotted:
1. Decisions out of sight. Evidence: D1, D3, X2, S3. Here: the June reorganisation was decided with no one outside the founders asked and announced without reasons; Engineering found out second-hand that a client's work had stopped; 3 of 6 leavers raised it; S3 is 44%, down 21 points.
2. Bad news unwelcome. Evidence: S1, X1. Here: one reported group is at 56% on S1, below 70%; 2 of 6 leavers said raising a problem was held against them.
3. Values in name only. Evidence: R1, D1. Here: 6 of 9 recognitions were for working late or over a weekend, which no stated value names; the June reorganisation was decided without reasons.
One sign only: Habits from a smaller company: D1: the founders alone decided a team's structure; D2 shows a team lead deciding a team-level change, and nothing shows team choices waiting for a founder.
Not seen: Culture left to spread by itself (an onboarding buddy, a weekly team meeting and a monthly all-hands are in place); Results never shared back (the April results went to all staff in May); Uneven standards (no item says a rule applies differently by team or level).

RITUALS TO TRY
1. Decision notes in the open. Answers: B2; decisions out of sight. How often: for every decision that changes a team's work, posted before it takes effect. Run by: the founders. Takes: about ten minutes a decision. Watch: S3 at the next survey, and whether X2 comes up again in exit notes.
2. Hand-off owners. Answers: B3, B4. How often: weekly, inside each team's existing meeting. Run by: each team's lead. Takes: about five minutes. Watch: S4 at the next survey, and whether open items like D4 gain an owner.
3. Problem first. Answers: B1; bad news unwelcome. How often: weekly, opening each team meeting. Run by: each team's lead. Takes: about five minutes. Watch: S1 for each reported group at the next survey, and whether X1 comes up again.

QUESTIONS FOR LEADERSHIP
1. Confirm, reword or replace the six drafted behaviours, B1 to B6; none was supplied.
2. Which of the three rituals, if any, to try, and who owns each (B1 to B4; decisions out of sight; bad news unwelcome).
3. What staff are told from this check, and when (S1 to S6; the April results were shared in May).
4. Who owns out-of-hours support requests between Client Services and Engineering (D4), still open after two meetings.
5. Whether to add a survey question on good work being noticed, since nothing supplied bears on B6 (R1, R2, R3).
6. Values in name only is spotted (R1, D1) and no chosen ritual answers it; whether to try Values in recognition in place of one of the three.

LEFT OUT
Exit notes: one person's name removed; the theme is kept without it.
Exit notes: one leaver left to move city; that reason is not a culture theme.
Survey: Operations (4 respondents) combined with Client Services, the next smallest team.
Survey rows set aside: none; every row's counts add up to its respondents.
Themes outside the stated values: X5 (pay) and X6 (promotion path), each from one leaver.
Survey comments: none supplied.

Prepared for the people lead. The two founders decide what changes and what staff are told. Nothing has been shared with staff, sent or posted, and no record has been changed.
```

## What was observed

**Every required part was produced.** All sections of the output format are present. All 30 export rows added up to their respondent counts, and no stop condition was triggered. Every share was recomputed from counts, and the company figures were worked from summed counts, not averaged team percentages.

**Where the instructions left a choice or needed a guess.**

1. *Mapping questions to values.* The template does not say how a survey question is matched to a value or behaviour. It lists this only as something to set once under "What to customize". The run matched Q1 to raising problems, Q3 to reasons for decisions, Q4 to hand-offs and Q5 to checking work, and put Q2 and Q6 under OTHER SURVEY RESULTS. A different reader could map them differently.
2. *Which share sorts a question.* A question is "at or above the match threshold" or "below the drift threshold", but the template does not say whether the company share or a group's share decides. The run used the company share and treated group shares only through the team gap line.
3. *A decision that shows both a behaviour and its opposite.* D3 told one team with reasons and left another team unaware. The template has no rule for an item that points both ways. The run counted D3 for B1 and B4 and set it aside as "noted, not counted" for B2.
4. *Recognition cannot count against.* The "Against" rules list surveys, concerns and decisions, not recognition. So R1 (6 of 9 recognitions for working late) could not count against any behaviour. B6 came out "Not enough evidence" even though the recognition pattern is plainly relevant. The pattern only surfaced through the anti-pattern list. Whether R2 (client praise, with no detail on what was praised) describes a behaviour about good work is also a guess.
5. *Two-clause anti-pattern.* "Values in name only" has two conditions joined by "or". The run treated R1 (first condition) and D1 (second condition) as two different items and named it as spotted. That reading of "at least two different items" is a judgement, and the published example read it more strictly. The second condition also leans on behaviours the assistant drafted itself, which is circular.
6. *Bad news unwelcome beside an exit theme.* The rule pairs a survey group below the threshold with an exit theme. Written side by side, that can let a reader guess which team the exit theme came from, even though exit themes must never be tied to a team. The run avoided naming the group on that line, but the rule itself invites the juxtaposition.
7. *Habits from a smaller company.* "Friction the evidence shows, such as every team-level choice waiting for a founder" is loose. The run called it one sign only. A reasonable reader could call it spotted or not seen.
8. *Exit-note grouping.* Themes are the assistant's own grouping. One note holds two themes (cross-team ownership, and hearing of a change from a client). The run used it for both. How far to merge "no reasons" with "heard late" into one theme is a choice. The run merged them into X2.
9. *A named manager in an exit note.* One note quotes a team lead telling a leaver to keep things positive. The template says to remove names and keep the theme, and to leave out notes about a complaint or grievance. The run treated it as a working-environment theme, removed the name and kept it. It is not obvious whether it should count as a complaint about a named person and go to HR.
10. *Ritual durations and the cap.* The format asks for "roughly how long" each ritual takes, and the template gives no source for it. The run's figures (about ten minutes a decision, about five minutes weekly) are estimates, not drawn from the inputs. With three anti-patterns spotted and two drifting behaviours, three rituals could not answer everything. The run covered the two drifts and two of the three anti-patterns, and raised the third as a question for leadership. The template does not say what to do when the cap leaves something unanswered.
11. *Typo-level slips avoided but possible.* Pairing the behaviours and readings by number depends on the assistant keeping B-numbers consistent across three sections. Nothing in the template checks this.

**Stops.** Nothing in the inputs triggered a stop. Headers matched, question wording was supplied, total respondents (52) were above the smallest group, and no row failed its count check. The single name in the exit notes was removed under the "remove names" step, with no stop. None of the stop conditions about requests (identify who answered, rank a person, send results) arose, because the inputs asked for none.

**Facts in the output not in the inputs.** The ritual durations above. The six behaviours, which are drafted by design and marked for leadership to confirm. The groupings of exit notes into themes. Nothing else was added; every figure, date and role comes from the inputs.

**Differences from the published example.**

- Survey evidence S1 to S6, the group shares, the team gaps, the combined group and the change since the last survey are identical to the published example.
- Exit themes cover the same six, numbered in a different order (the example puts "reasons for decisions" first; this run put "raising a problem" first). The counts match.
- The behaviours differ in wording. B1, B3 and B5 are close. B2, B4 and B6 differ: the example's B4 is following up problems outside a team's area, and its B6 is raising quality risks before a deadline. This run's B4 is a named owner and a report back, and its B6 is good work being noticed.
- Readings agree for B1 (Mixed), B2 (Drifts), B3 (Drifts), B5 (Matches) and B6 (Not enough evidence). B4 differs: Mixed here, counting D3 for and D4 against, and Mixed in the example with nothing for or against and only a between-thresholds survey question. The totals (1 match, 2 mixed, 2 drifts, 1 short) are the same.
- B2: the example counted D3 as against; this run set it aside.
- Anti-patterns: this run spotted three (the example spotted two). It named "Values in name only" as spotted where the example listed one sign only. It listed "Habits from a smaller company" as one sign only where the example listed it as not seen.
- Rituals: the same three, in a different order, and this run's "Problem first" is not limited to one group.
- Questions for leadership: six here, five in the example, because this run asked about the recognition ritual left unchosen.
- LEFT OUT: this run adds the line saying no survey rows were set aside; the example omits it.

**Against the reviewer checklist.** The run found no person named, no group under five shown, no exit theme tied to a team, note or quotation, every share recomputed from counts and every reading citing numbered items sorted by the stated thresholds. It also found every spotted anti-pattern resting on at least two items, rituals that fit the size and are not already in place, and no decision or message to staff. Item 5 (behaviours a newcomer could see) and item 7 (rituals that promise no result) are judgements for leadership. The run met item 6 only on the reading described in point 5 above.
