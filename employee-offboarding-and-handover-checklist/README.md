# Employee offboarding and handover checklist

When someone leaves, your HR lead and their manager share one checklist: every piece of their work handed to a named colleague before the last day, every system on your access register removed by its owner at a set time, and every item of equipment back. Nothing is removed or sent without a person.

*Capability template · People and HR · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/employee-offboarding-and-handover-checklist/)*

## The outcome

The day a departure is confirmed, the HR lead and the manager hold the whole leaving on one page. Each piece of the person's work has a receiver and a date before the last day. Each system they can reach has an owner who removes it, a time, and a step to move any company data first. Each laptop, phone and pass has a way back.

The usual surprises arrive as questions in the first week instead of after the farewell: a monthly report nobody has picked up, a shared login nobody owns, a portal that never made it onto the register, recordings with nowhere to go. Each comes with the facts and the role who settles it.

Every departure gets the care your most careful manager gives one. The manager decides who takes over each piece of work. The IT lead and each system's owner remove access. The assistant removes nothing, moves nothing and sends nothing.

## Who starts the work, and when

The HR lead starts it the day the departure and the last working day are confirmed, so the handover begins while the person still has most of their time. The manager supplies the handover list and names every receiver. The HR lead approves the checklist before it is shared with the manager, the IT lead and the departing colleague, and runs it again when the last day moves or a receiver is named.

## What they supply

- **The departure record.** The role, the manager, the last working day and any days the person will not be working before then. The reason for leaving is not needed.
- **The access register,** exported for the departing person: each system, account, access level, admin owner, whether the account is shared and what company data it holds.
- **The equipment list,** exported the same way: asset tag, item, date issued and where it is kept.
- **The manager's handover list.** Each piece of recurring and open work, where it is kept, who relies on it and who takes it over, plus who receives the mailbox and files.
- **The company's offboarding standard.** When the handover is due, when access comes off, how long mail is forwarded and who receives returned equipment.
- **Any notes.** A system or item the lists leave out, or how the team will be told.

## What comes out

One dated checklist in six parts: the handover, with what the departing colleague's handover document must cover; access, one line per system; equipment, one line per item; the people to tell who takes over; the last day in order; and the decisions to settle before the checklist is shared, each addressed to the manager, the IT lead or the HR lead.

The reason for leaving and every sign-in detail stay out of it. Pay, benefits, leaving paperwork, references and any agreement stay with the HR lead's own process; the capability declines a termination letter, a severance offer or separation terms.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [People and HR](https://fullypowered.ai/functions/people-and-hr/), which owns the departure and approves the checklist.
- [IT and systems](https://fullypowered.ai/functions/it-and-systems/), which removes access, sets mail forwarding and wipes returned devices on the agreed day.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where client relationships and recurring reports sit with one person and must pass to another before they go.
- [Software and technology](https://fullypowered.ai/industries/software-technology/), where one person can reach dozens of systems, some with admin rights.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where passes, keys and site equipment come back as well as laptops.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where long-serving people hold work and access that nobody has written down.

## What has to change for your company

Start from your own access register and equipment list; the capability adds no systems of its own, and every system missing from the register comes back as a question for the IT lead. Set your standard once: how many working days before the last day the handover is due, when access comes off, who receives mail and returned equipment. Decide who answers which kind of question. What the departing colleague knows that no document holds is worth capturing properly; [SOP exception capture](https://fullypowered.ai/capabilities/sop-exception-capture/) records how they handle the awkward cases. It is the companion to the [employee onboarding plan](https://fullypowered.ai/capabilities/employee-onboarding-plan/), and runs in ChatGPT, Claude, Copilot or Gemini from files and notes you supply, with no connection to your systems.

## What has been checked

Fully Powered AI wrote this capability template. It was editorially reviewed on 9 November 2026. It was tried on its invented example in Claude on 9 November 2026; the record of that run is published with it, and lists the small edits made afterward that have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past departures your HR lead remembers well, plus hard cases written in advance, each with its expected behavior: a register with a renamed column, a shared login with no owner, a laptop kept at home, a hand-over date after the last day. The HR lead and the IT lead check every line against the register before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 9 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 9 November 2026. The record is in [TRIAL.md](TRIAL.md).
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
- [SOP exception capture](https://fullypowered.ai/capabilities/sop-exception-capture/)
- [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
