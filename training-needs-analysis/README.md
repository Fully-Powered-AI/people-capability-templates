# Training needs analysis

For one team, the HR lead or team manager gets what each role must be able to do, how many people can do it now, where the team falls short, and the training to arrange first, with who arranges it and by when. Counted by role, never a rating of a named person.

*Capability template · People and HR · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/training-needs-analysis/)*

## The outcome

Training money goes where the team actually needs it. For every role in the team, the HR lead sees each ability the work depends on, the level it takes, how many people are there today and how many are still needed. The shortfalls come in a clear order: anything a rule or a customer requires first, then what the team cannot work without, then the rest.

The quiet risks show up before they cost anything. An ability only one person holds. Certificates that run out before anyone has booked the renewal. A "training problem" that is really an out-of-date script or a missing tool, which goes back to be fixed instead of being trained around.

Each training item says how it is delivered, who arranges it, the date it must be done by and what it costs, where the price is known. Everything is counted by role. The team manager chooses who attends, the HR lead approves, and the AI assistant enrols nobody, books nothing and buys nothing.

## Who starts the work, and when

The team manager starts it, or the HR lead with them, when the work is about to change or has drifted: a new system going live, a role growing, a run of errors in one kind of work, certificates coming up for renewal. It is worth running again before each training budget is set. The HR lead approves the analysis before anyone is booked or told.

## What they supply

- **A short scope brief.** The team, the roles in it, why now, and today's date.
- **The requirements.** For each role, the abilities it needs, how much each matters, the level it takes, how many people need it, and any rule or customer term that requires it, as a simple table with stated column headers.
- **The coverage.** For each role and ability, how many people can do it now, how many could teach it, where that count comes from, and certificate end dates. Counts only, no names.
- **The manager's notes.** What goes wrong and why, changes coming, courses and prices known, and the budget.

## What comes out

One analysis, in a fixed order. A grid of every role against its abilities, with what is needed, what is held, what lapses before the horizon date and the shortfall. The shortfalls in priority order, each with what closes it: a course, teaching from someone in the team, supervised practice, or a check first because training is not the answer.

Then the single holders, the certificates running out with their renewal dates, the training items with arranger, date and cost, the total against the budget, and the questions the HR lead settles before anything is booked. Names, scores and personal details in the notes are left out, and the analysis says what kind was removed.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [People and HR](https://fullypowered.ai/functions/people-and-hr/), which holds the training budget and wants it spent where the gaps are.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), where a new system or process changes what every role has to do.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where the team's know-how is what clients pay for.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where certificates, machines and single experts decide whether a shift can run.
- [Logistics and trade](https://fullypowered.ai/industries/logistics-and-trade/), where new systems, equipment tickets and seasonal staff keep the abilities a team needs moving.
- [Hospitality](https://fullypowered.ai/industries/hospitality/), where turnover is high and the same abilities have to be rebuilt in every new team.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when roles fill faster than anyone can teach them.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where one long-serving person often holds what the rest of the team cannot do.

## What has to change for your company

Set your level scale, or use the four steps it comes with. Decide your horizon date, usually the end of the training budget year, and how many days before a certificate expires the renewal must be done. Name who approves, who arranges outside courses and who arranges teaching inside the team. Decide what counts as evidence for each count, and who may read the analysis. A new starter's first weeks run on the [employee onboarding plan](https://fullypowered.ai/capabilities/employee-onboarding-plan/); when one person holding an ability is leaving, [departing-employee knowledge capture](https://fullypowered.ai/capabilities/departing-employee-knowledge-capture/) keeps what they know. It runs in ChatGPT, Claude, Copilot or Gemini from the lists and notes you supply, with no connection to your HR system.

## What has been checked

Fully Powered AI wrote this capability template. It was editorially reviewed on 9 November 2026. It was tried on its invented example in Claude on 9 and 10 November 2026 in three runs: the template was revised after the first, and again after an independent review of the second, and the record of the third is published with it. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a team your HR lead knows well, plus hard cases written in advance, each with its expected behavior: a certificate that lapses before the horizon, an ability one person holds, a note that blames a broken checklist, a renamed column, a request to say who is weakest. The HR lead checks every count against the coverage list before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 9 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete capability template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the capability drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related capabilities

- [Employee onboarding plan](../employee-onboarding-plan/)
- [Departing-employee knowledge capture](../departing-employee-knowledge-capture/)
- [Manager feedback preparation](../manager-feedback-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
