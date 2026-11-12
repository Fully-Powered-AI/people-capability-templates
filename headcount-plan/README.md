# Headcount plan

For a founder, people lead or finance lead preparing next year: every role and its cost by team, the new roles and backfills with their months, the fully loaded cost month by month against the budget, and what changes if revenue lands lower or higher. It plans roles and money, never decisions about named people.

*Workflow template · People and HR · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/headcount-plan/)*

## The outcome

Next year's people cost goes onto a few pages the board can read. The approver sees every role the company has today and what each team costs, then every change planned for the year: each new role, each backfill and each departure already confirmed, with the month it lands and what it adds or saves.

Month by month, the plan shows how many people the company will have and what they cost once employer taxes, benefits, bonus targets, equipment and joining costs are counted, beside the budget for that month. The months that go over stand out before anyone has signed off a single role.

Then the same plan two more ways: if revenue lands lower, with the changes your team leads have marked as able to wait, and if it lands higher, with the roles you would add. Each case shows the cost for the year, people cost as a share of revenue, and the cost rate the company carries into the following year. Every gap arrives as a question for the approver, with the facts beside it. The plan works by role from your own figures. It names no one, proposes no cuts among the people you already have, opens no role and changes no budget.

## Who starts the work, and when

The finance lead or people lead starts it when next year's budget is being set; in a smaller company, the founder does. It is worth running again when revenue moves far from plan, before a funding round or a board meeting that asks for the people plan, and whenever a change is added, approved or dropped. The chief executive, or whoever holds the budget, approves the plan before any role is opened.

## What they supply

- **A short scope brief.** The company, the first month of the plan year, the currency, today's date and why now.
- **The current roles.** Each team and role, how many people hold it, whether they are employees or contractors, the total annual pay for the row and any bonus or commission target, as a simple table with stated column headers. Counts and totals only, no names.
- **The changes.** Each new role, backfill and confirmed departure, with its month, its pay, whether it is approved or proposed, and which revenue cases it belongs to.
- **The settings.** The rate your finance lead uses for employer taxes, benefits and pension, any monthly cost per person and joining cost, the pay review, the people-cost budget and the revenue for each case.
- **Notes.** What has been agreed, any limits the board has set, and anything else the approver should weigh.

## What comes out

One plan, in a fixed order. A short summary of all three cases. The current roles by team, with what each costs a month. Every change on one line, with its month, its cost in the year and anything that needs a second look, such as a backfill that starts before the person it replaces has left, or pay well away from what the role pays today.

Then the base case month by month against the budget, the three cases side by side, the assumptions behind every figure with a check against last month's actual people cost in your accounts, and the questions the approver settles. Names and personal details in the notes are left out, and the plan says what kind was removed.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [People and HR](https://fullypowered.ai/functions/people-and-hr/), which owns the roles, the pay review and the plan for who the company needs next.
- [Finance and accounting](https://fullypowered.ai/functions/finance-and-accounting/), which owns the budget and the cost rates the plan is built on.
- [Leadership](https://fullypowered.ai/functions/leadership/), where the chief executive decides which roles the company can afford, and when.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where people are most of the cost and every hire is a bet on revenue.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where the team is what clients pay for and hiring ahead of work costs real money.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where agencies staff up for accounts that can grow or go.
- [Startups & new ventures](https://fullypowered.ai/situations/startups-and-new-ventures/), when the next round depends on a hiring plan the numbers support.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when the company adds roles faster than anyone can keep the total in their head.
- [Private equity & portfolios](https://fullypowered.ai/situations/private-equity-and-portfolios/), where owners want the people plan tied to the budget and to revenue.

## What has to change for your company

Settle the cost rates with your finance lead: the rate for employer taxes, benefits and pension, whether it applies to bonuses, what the per-person monthly cost covers and whether contractors carry it. Decide what "lower" and "higher" revenue mean for you and which changes each team lead may mark as able to wait. Set how far a new role's pay may sit from the role's current average before the plan asks about it, and how close the plan must come to last month's accounts. Choose who approves and who may read the plan, since a role held by one person shows that person's pay. Once a role is approved, the [job description](https://fullypowered.ai/workflows/job-description/) workflow template takes it forward; the [budget-versus-actual variance commentary](https://fullypowered.ai/workflows/budget-versus-actual-variance-commentary/) follows the plan through the year. It runs in ChatGPT, Claude, Copilot or Gemini from the lists and notes you supply, with no connection to payroll or your accounts.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 10 November 2026. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on last year's plan, which your finance lead already knows, plus hard cases written in advance, each with its expected behavior: a backfill that overlaps the departure, a missing cost rate, a renamed column, a lower case that is still over budget, a request to say who should leave. The finance lead checks every figure against payroll and the accounts before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
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

- [Budget-versus-actual variance commentary](https://fullypowered.ai/workflows/budget-versus-actual-variance-commentary/)
- [Thirteen-week cash flow forecast](https://fullypowered.ai/workflows/thirteen-week-cash-flow-forecast/)
- [Job description](https://fullypowered.ai/workflows/job-description/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
