# Exit interview themes summary

Each quarter or half-year, your HR lead sees what leavers said on the way out: themes with counts, unattributed quotes with identifying detail removed, set beside the reasons recorded at the time, and questions for leadership. Small groups are combined or withheld by a stated rule. It decides nothing about any person.

*Workflow template · People and HR · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/exit-interview-themes-summary/)*

## The outcome

Leadership hears what leavers actually said, in one place, without anyone being exposed. Every exit interview note and leaver form from the period is read and grouped into themes from a fixed list, such as workload and hours, career growth or pay. Each theme is counted by leaver, so someone who makes the same point three times still counts once, and each shows how many leavers raised it, for how many it was the main reason, and how many had it recorded as their reason when they resigned.

The comparison is the point. If "career move" was recorded for several leavers and some of them told the exit interviewer the hours were the real reason, the summary says so plainly, and asks who records the reason and when.

Anonymity is a rule, not a judgement call. No group smaller than the number you set, five by default, is shown. Small teams are combined, and the team view is withheld when combining leaves only one group. A theme raised by a single leaver is not named in the shared summary. Quotes carry no name, team, role or detail that points to a person or a small group, and a quote that cannot be made anonymous is withheld and counted. Health and family detail is counted, never described.

The summary ends with questions for leadership, each built on the counts. It recommends nothing about any person, names no one and sends nothing. The HR lead approves it before anyone else reads it.

## Who starts the work, and when

The HR lead or people lead runs it once a quarter, or once every half-year where too few people leave in a quarter to stay anonymous. It is also worth running before leadership looks at pay, rotas, progression or a reorganisation. The HR lead reads the draft, removes the note marked for HR only, and decides what goes to the leadership team.

## What they supply

- **The leaver list,** exported from the HR system or a spreadsheet: one row per leaver in the period, with a reference instead of a name, the team, the leaving date, how they left and the reason recorded at the time. Default column headers are given; if one does not match, it stops and asks.
- **Exit interview notes,** one per leaver, headed with the same reference, with the leaver's own words in quotation marks.
- **Leaver forms,** the exit survey export: the main reason, whether they would recommend working here, and their comments.
- **A few settings:** the period, which kinds of leaving to include, the smallest group to show, and your own theme list if you have one. A starter list is included.
- **Last period's summary,** if there is one, marked to show which questions leadership has answered.

## What comes out

One summary in a fixed order: coverage, showing who left, who had an exit conversation or form and who is out of scope; the themes, with counts and up to two quotes each; what leavers said beside what was recorded; a view by team, with small teams combined; whether leavers would recommend working here and what they spoke well of; the change since last period; and the questions for leadership, with any still open from last time.

A short note for the HR lead only comes last, to remove before sharing. It lists any matter raised in a note that belongs to HR's own process, such as a report of abuse or a complaint about conduct, by leaver reference and kind; the topics raised by a single leaver; and every quote withheld or changed, with the reason.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [People and HR](https://fullypowered.ai/functions/people-and-hr/), which holds the exit notes and owes leavers their anonymity.
- [Leadership](https://fullypowered.ai/functions/leadership/), which reads the themes and decides what the company looks at next.
- [Hospitality](https://fullypowered.ai/industries/hospitality/), where rotas and short-notice shift changes often sit behind a recorded "personal reasons".
- [Professional services](https://fullypowered.ai/industries/professional-services/), where people leave for progression and the firm wants to know whether it could have offered it.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where reorganisations and on-call rotas show up in exit conversations before they show up anywhere else.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where the leavers from one shift or line can be few enough that combining groups matters.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when leaving rises with headcount and leadership needs the reasons, not just the number.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where years of recorded leaving reasons have never been set beside what leavers said.

## What has to change for your company

Set the smallest group you will show; five is a careful floor, and a company where everyone knows who left a team of six may want more. Supply your own theme list and map your recorded reasons to it once, so every period reads the same way. Decide which kinds of leaving the summary covers; it covers resignations by default. Ask whoever holds exit conversations to put the leaver's own words in quotation marks, because only those are ever quoted. Agree who sees the HR-only note, how a matter raised in it is followed up under your own procedure, and who in leadership receives the approved summary. The handover, access and equipment for each leaver run on the [employee offboarding and handover checklist](https://fullypowered.ai/workflows/employee-offboarding-and-handover-checklist/), and what a leaver knows is captured with [departing-employee knowledge capture](https://fullypowered.ai/workflows/departing-employee-knowledge-capture/). It runs in ChatGPT, Claude, Copilot or Gemini from the files you supply, with no connection to your HR system, and never asks for a password or a login code.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 12 November 2026. It was tried on its invented example in Claude on 12 November 2026 in two runs; the record of the second, made on the instructions as revised after the first and repeated once more after a review, is published with it. The second run was not independent of the first: the same session made the edits and ran it. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past period your HR lead already knows, with hard cases written in advance: a team with two leavers, a quote that names a manager, a note that reports a complaint about conduct, a request to say who said something. The HR lead checks every count against the notes and every quote against its source before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) sets those cases up, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 12 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 12 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete workflow template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the workflow template drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related workflow templates

- [Employee offboarding and handover checklist](../employee-offboarding-and-handover-checklist/)
- [Departing-employee knowledge capture](../departing-employee-knowledge-capture/)
- [Culture health check](../culture-health-check/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
