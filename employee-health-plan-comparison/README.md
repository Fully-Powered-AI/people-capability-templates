# Employee health plan comparison

For an owner or people lead at renewal: the broker's health plan options next to each other, with premiums split between company and employee, deductibles, out-of-pocket limits, network notes, the cost to the company and to a typical employee at low, middle and high use, and questions for the broker.

*Capability template · People and HR · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/employee-health-plan-comparison/)*

## The outcome

The renewal decision goes onto a few pages the owner can read in one sitting. Every plan the broker put forward sits next to the others: who insures it, what kind of plan it is, the network, the deductibles, the out-of-pocket limits, the visit and drug charges, and what happens outside the network.

Then the money, worked from your own enrollment. For each coverage tier, what the plan costs a month, what the company pays and what the employee pays. For each plan, what the company would spend in the year if everyone enrolled today took it, beside this year's cost and your budget. And for a typical employee on single cover, what the year costs at low, middle and high use, once premiums, the deductible, coinsurance and any company account money are counted.

If the current plan is renewing, every change in its terms is marked, item by item, with the rise in premiums. Every blank in the broker's documents and every condition in the covering email becomes a question for the broker, with the fact behind it. The choices that belong to the owner arrive as points with their figures. The comparison names no employee, uses no one's health information, tells no employee which plan to pick and recommends no plan. The broker advises; the company decides.

## Who starts the work, and when

The people lead, office manager or finance lead starts it as soon as the broker sends the renewal terms and the alternative quotes, early enough to get answers back before the decision date. In a small company, the owner does it. It is worth running again when the broker revises a quote, when the company changes what it pays, or when enrollment moves. The owner, or whoever holds the benefits budget, decides with the broker's advice.

## What they supply

- **A short scope brief.** The company, the first day of the plan year, the date the decision is due, the currency and today's date.
- **The plan list.** One row for each plan and status, typed from the broker's plan summaries, with stated column headers: deductibles, coinsurance, out-of-pocket limits, visit and drug charges and out-of-network cover.
- **The premium list.** The monthly premium for each plan and coverage tier.
- **What the company pays.** A percentage or a monthly amount for each tier.
- **Enrollment by tier.** How many employees are on each tier today. Counts only, never names.
- **Notes.** What the broker's covering email says, and what matters to the company, such as where staff live.
- **The settings.** Three spending levels for a year of low, middle and high use (the broker can suggest them), any company account contribution, the benefits budget and who decides.

## What comes out

One comparison, in a fixed order. A summary of what each option costs the company and the lowest-cost option at each use level, stated as facts. The plans' designs next to each other. Premiums and shares by tier. The company's cost for the year against this year and the budget. The typical employee's cost at each use level. What the renewal changes. Then the questions for the broker, the points for the owner, the assumptions behind every figure, and anything else in the notes. Names and health details in the notes are left out, and the comparison says what kind was removed.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [People and HR](https://fullypowered.ai/functions/people-and-hr/), which runs the renewal, enrollment and what employees are told about their benefits.
- [Finance and accounting](https://fullypowered.ai/functions/finance-and-accounting/), which owns the benefits budget and checks what each option costs the company.
- [Leadership](https://fullypowered.ai/functions/leadership/), where the owner decides which plans to offer and how much of the premium the company pays.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where benefits help keep the people clients pay for.
- [Construction](https://fullypowered.ai/industries/construction/), where a growing contractor offers office staff and crews one set of plans.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where benefits are a large share of the cost of every role on the floor.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where the plan has renewed for years and nobody has priced the alternatives against it.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when headcount grows and benefits become one of the biggest lines in the budget.
- [Startups & new ventures](https://fullypowered.ai/situations/startups-and-new-ventures/), when a young company chooses its first plans and its share of the premium.

## What has to change for your company

Agree the three spending levels with your broker and keep them the same each year, so one year's comparison lines up with the next. Decide whether a second typical employee on family cover should be worked, whether copays should count in the totals, and how a company contribution to an employee account is treated. Set the renewal rise that should prompt a question and the budget each option is held against. Choose who decides and who may read the comparison, since a small tier can point to the people on it. Once the plans are chosen, the [headcount plan](https://fullypowered.ai/capabilities/headcount-plan/) carries the benefits cost into next year's people budget. It runs in ChatGPT, Claude, Copilot or Gemini from the lists and notes you supply, with no connection to the broker's portal, the insurer or payroll.

## What has been checked

Fully Powered AI wrote this capability template. It was editorially reviewed on 10 November 2026. It was tried on its invented example in Claude on 10 November 2026, in two runs, not as a blind test; the record of the second, made by the session that revised it, is published with it, and lists the small edits made afterward that have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on last year's renewal, which your people lead and broker already know, plus hard cases written in advance, each with its expected behavior: a blank out-of-pocket limit, a renamed column, a renewal above your threshold, a note that names an employee's treatment, a request to say which plan an employee should choose. Your people lead checks every figure against the broker's documents before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
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

- [Headcount plan](../headcount-plan/)
- [Business insurance renewal review](https://fullypowered.ai/capabilities/business-insurance-renewal-review/)
- [Vendor quote comparison](https://fullypowered.ai/capabilities/vendor-quote-comparison/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
