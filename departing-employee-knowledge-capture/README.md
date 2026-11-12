# Departing-employee knowledge capture

When someone is leaving or changing role, their manager gets an interview guide aimed at what only that person knows, then a handover document the successor can work from, every point traced to the conversations and marked with how sure it is. Nothing is shared until the manager approves.

*Workflow template · People and HR · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/departing-employee-knowledge-capture/)*

## The outcome

Years of know-how stay with the company when the person who built them moves on. Before the conversations, the manager holds a guide: the areas of know-how in priority order, starting with what nobody else holds, the sessions to book, who sits in, and the questions that draw out what is written nowhere. After them, the successor gets one document: what to know in each area, when it matters, the exceptions, the early warning signs, what the person settled alone and what they passed up, who else can help and where it is written down.

Every point names the conversation it came from and says how sure it is: confirmed, the person's own account with someone to check it with, unsure, or disputed by a colleague. Promises still open come with their dates. Ideas the company has tried and dropped are recorded, so nobody spends a year relearning them.

The manager runs the conversations and decides. The departing colleague checks the draft before anyone else reads it. The assistant books nothing, records nobody, shares nothing and never chooses who takes over a piece of work.

## Who starts the work, and when

The manager starts it the day a departure or a move to another role is confirmed, while the person still has most of their time. They list the areas the person looks after; the departing colleague can add their own. The manager approves the guide, books the sessions, and runs the second stage after each round of conversations. The successor sits in where one is named.

## What they supply

- **A short role brief.** The role, the last day in it, any days off before then, and the successor if one is named. The reason for leaving is not needed.
- **The knowledge area list.** Each area the person looks after, who depends on it, who else knows it and where it is written down, as a simple table with stated column headers.
- **The departing colleague's own list,** if they have one.
- **A few settings.** Session length, areas per session, and how many working days before the last day the conversations finish and the draft is checked.
- **The session notes,** numbered, for the second stage. Recording happens only if the person agrees.

## What comes out

First, the interview guide: the dates, the areas in priority order with the reason for each, questions for every area plus ones aimed at its documents and outside parties, a session plan with who to invite, the closing questions, and the decisions the manager makes before booking.

Second, the knowledge handover document: each area with its fields filled from the notes, the open commitments and coming dates, the ideas tried before and dropped, the people to know, and the questions to settle before the departing colleague checks it. Personal matters stay out; the document records the work, never the person.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [People and HR](https://fullypowered.ai/functions/people-and-hr/), which sees every departure and wants the know-how to stay.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), where unwritten practice is what keeps the work running.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where client relationships and judgment sit with one senior person.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where long-serving people know the machines, the suppliers and the workarounds.
- [Logistics and trade](https://fullypowered.ai/industries/logistics-and-trade/), where cut-offs, carriers and supplier habits live in one buyer's head.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/), where a project lead's knowledge of clients and past jobs has to pass on mid-project.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where people with long service hold what nobody has written down.

## What has to change for your company

Set your session length, how many areas a conversation covers, and when the conversations and the check must finish. Add the questions your best managers already ask, and keep the one on ideas tried and dropped. Decide whether conversations may be recorded, where notes and the approved document are kept, and who may read them. Access, equipment and the hand-over of each piece of work run on the [employee offboarding and handover checklist](https://fullypowered.ai/workflows/employee-offboarding-and-handover-checklist/). When one procedure turns out to be mostly exceptions, [SOP exception capture](https://fullypowered.ai/workflows/sop-exception-capture/) writes them down properly, and when a whole team's know-how needs capturing, that is the work of [Fully Powered Studio](https://fullypowered.ai/fully-powered-studio/). It runs in ChatGPT, Claude, Copilot or Gemini from the lists and notes you supply, with no connection to your systems.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 9 November 2026. It was tried on its invented example in Claude on 9 November 2026; the record of that run is published with it, and lists the small edits made afterward that have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past departure your manager remembers well, plus hard cases written in advance, each with its expected behavior: a blank where "others who know it" should be, a list with a renamed column, steps kept only in someone's own mailbox, a colleague who does the work differently. The manager checks every point against the notes before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 9 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 9 November 2026. The record is in [TRIAL.md](TRIAL.md).
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
- [SOP exception capture](https://fullypowered.ai/workflows/sop-exception-capture/)
- [Write an SOP from how the work is done](https://fullypowered.ai/workflows/sop-from-how-the-work-is-done/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
