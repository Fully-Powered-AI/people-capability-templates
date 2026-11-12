# Manager feedback preparation

Workflow template 0.1.0 · People and HR · Fully Powered AI

## Purpose

Prepare a structured feedback conversation for a team manager from the role's agreed responsibilities, specific dated observations and the previous conversation's commitments: observations kept apart from interpretations, the questions to ask, the ask and the support on offer. Any observation that is vague, second-hand or missing an example goes back to the manager. The conversation is the manager's to hold, and the development plan is agreed in it by manager and colleague.

## When to use it and when not to

Use it two or three days before a scheduled conversation: a regular one-to-one, an onboarding check-in at day 30, 60 or 90, or a conversation about one piece of work.

Not for a disciplinary meeting, a formal performance process, a complaint or investigation, or a conversation about health, leave, accommodation or a personal circumstance: those go to the people lead. Never for a rating, score, ranking or recommendation about pay, promotion or employment, and never for drafting a warning, an improvement plan or any other employment document.

## Roles

- **Runs it:** the team manager.
- **Reviews it:** the team manager, before the conversation. The people lead reviews the observation standard, not individual preparations.
- **Decides:** the manager decides what to raise and holds the conversation. The manager and the team member agree the development plan. The people lead owns pay, promotion, ratings and any formal process.

## Inputs

1. **Agreed responsibilities.** Numbered, from the role brief or job description. If missing, ask the manager which responsibility each observation relates to.
2. **Observations.** Each with a date, what the manager saw or checked in a record, the source and the effect, from the manager's notes and team records. One that fails the test in step 2 is sent back.
3. **Previous commitments.** What each person agreed last time, from the last preparation or the manager's notes. If none, write "No recorded commitments" and ask whether this is the first conversation.
4. **Manager's interpretations.** What the manager thinks lies behind an observation, marked as interpretation. Optional.
5. **Conversation details.** Date, length, type. If missing, ask.

## The procedure

1. List missing inputs. Check every note against the stop conditions; if one applies, stop the whole preparation.
2. Test each observation. It is usable when it has all four: a date within the last [LOOKBACK_DAYS] days; a first-hand source (the manager saw it, or checked it in a named record); a specific example of what happened; a link to a numbered responsibility.
3. Send back each observation that fails. Quote it as written and ask one specific question that would fix it:
   - Vague: "What happened, when, and with what effect?"
   - Second-hand: "Did you see this, or check it in a record? If not, ask [the person who saw it] to raise it directly, or leave it out."
   - No example: "Which occasion are you thinking of?"
   - Interpretation written as fact ("doesn't care about detail"): move it to interpretations and ask for the observation behind it.
4. Choose the responsibility in focus: the one the manager names, or the one with most usable observations; at most [MAX_FOCUS].
5. Put one usable observation of work that went well first, if one exists. Never invent one.
6. List the other usable observations with date, what happened, effect and source, in the manager's facts with no adjectives added.
7. List interpretations separately, each turned into a question.
8. Draft three to five open questions: at least one asks for the colleague's account before the manager's view, and one asks what would help.
9. Draft "The ask": one or two observable behaviors tied to the responsibility in focus. If the manager has not said what they want, write "Manager to state the ask".
10. List the support as the manager supplied it, or write "Manager to state the support".
11. Report each previous commitment as done (with date), open or unknown, the manager's own open commitments first, with a request to resolve or date each. If two sources disagree on a commitment's status, report it as unknown and cite both.
12. Return the preparation to the manager only.

## Exceptions and stop conditions

Stop the preparation and tell the manager to take the notes to the people lead when the inputs mention or suggest:

- possible misconduct, a complaint, harassment, discrimination or an investigation;
- health, disability, accommodation, pregnancy, leave or a personal circumstance;
- a formal performance process, probation decision, warning or termination;
- a protected characteristic.

If asked to rate, score, rank or compare colleagues, or to recommend pay, promotion or any employment action, decline that request, say it belongs to the people lead's process, and continue the preparation without it.

## Output format

```
Feedback preparation · [Role] · [Day Date]
Prepared for: [manager role]. Conversation: [type], [length].
Responsibility in focus: Responsibility [n]: [as written].

Start with
- [Date]: [what went well]. Source: [record].

Observations
- [Date]: [what happened]. Effect: [effect]. Source: [record].

Interpretations to test
- The manager's note: "[as written]". Ask: [question].

Questions
- [3 to 5 open questions]

The ask
- [specific behavior] / Manager to state the ask

Support on offer
- [as supplied] / Manager to state the support

Last time, [date]
- Manager: [commitment]: [done on date / open / unknown]
- [Team member role]: [commitment]: [done on date / open / unknown]

Sent back to the manager
- "[observation as written]": [reason]. [question]

Preparation for the manager. The manager holds the conversation; manager and
[team member role] agree the development plan together.
```

## Reviewer checklist

- Every observation in the preparation has a date, a first-hand source, an example and a responsibility.
- No interpretation appears as an observation.
- Every failed observation is quoted and sent back with a question.
- The manager's open commitments appear first under "Last time".
- No rating, score, label of the person or employment recommendation appears.
- "The ask" and "Support on offer" come from the manager or say they are missing.

## Acceptance tests

Proposed tests. They have not been run.

1. **Usable inputs.** Three dated first-hand observations, two commitments. Expected: a complete preparation; nothing sent back.
2. **Vague observation.** "Needs to be more proactive." Expected: quoted under "Sent back" with "What happened, when, and with what effect?"; not used.
3. **Second-hand report.** "The warehouse team said they were short with them." Expected: sent back with the second-hand question.
4. **Interpretation as fact.** "Doesn't care about detail." Expected: moved to interpretations; manager asked for the observation behind it.
5. **Manager's commitment, contradictory records.** The manager's notes say done; the last preparation shows it open. Expected: listed first under "Last time" as unknown, both sources cited, with a request to resolve or date it.
6. **No positive observation.** Expected: "Start with" omitted; nothing invented.
7. **Health mention.** A note links missed shifts to a medical issue. Expected: the preparation stops and the manager is referred to the people lead.
8. **Rating request.** The manager asks for a 1 to 5 score. Expected: declined; the preparation continues without one.

## Instructions for the AI assistant

```
You prepare feedback conversations for a team manager. You prepare; people
decide. You never rate, score, rank or compare colleagues, never recommend
pay, promotion or any employment action, never draft a warning, improvement
plan or other employment document, and never send anything to anyone.
The manager holds the conversation; manager and team member agree the
development plan.

Inputs: numbered responsibilities, observations, previous commitments,
optional interpretations, and the conversation's date, length and type.

First, stop the whole preparation and tell the manager to take the notes to
the people lead if anything mentions or suggests misconduct, a complaint,
harassment, discrimination, an investigation, health, disability,
accommodation, pregnancy, leave, a personal circumstance, a formal
performance process, probation, a warning, termination or a protected
characteristic. If asked for a rating, score, ranking or employment
recommendation, decline that part, say it belongs to the people lead's
process, and continue without it.

Test each observation. Usable means all four: dated within [LOOKBACK_DAYS]
days; first-hand (seen by the manager or checked in a named record); a
specific example; linked to a numbered responsibility. Send back each one
that fails, quoted as written, with one question:
- vague: "What happened, when, and with what effect?"
- second-hand: "Did you see this, or check it in a record? If not, ask the
  person who saw it to raise it directly, or leave it out."
- no example: "Which occasion are you thinking of?"
- interpretation as fact: move it to interpretations and ask for the
  observation behind it.

Then: pick the responsibility in focus (at most [MAX_FOCUS]). Put one usable
observation of work that went well first if one exists; never invent one.
List usable observations in the manager's facts with date, effect and
source, adding no adjectives. Turn each interpretation into a question.
Draft 3 to 5 open questions, including one asking for the team member's
account first and one asking what would help. Write the ask and support only
from what the manager supplied, otherwise "Manager to state the ask" or
"Manager to state the support". Report each previous commitment as done,
open or unknown, with the manager's own open commitments first. If two
sources disagree on a commitment's status, write unknown and cite both.

Use the output format exactly. End with: "Preparation for the manager. The
manager holds the conversation; manager and [team member role] agree the
development plan together." Return it to the manager only.
```

Paste the output format above beneath these instructions when you set them up.

## What to customize

- [LOOKBACK_DAYS]: how far back an observation may reach. Suggested default: 60.
- [MAX_FOCUS]: responsibilities in focus per conversation. Suggested default: 1, or 2 at a day-90 check-in.
- Your observation standard, written by the people lead, with one good and one returned example.
- The full list of topics that go to the people lead, matched to your policies.
- Where commitments are recorded so the next preparation can find them.
- Which conversations use it: one-to-ones, onboarding check-ins, project reviews.

## Version notes

0.1.0 · 9 November 2026 · Written by Fully Powered AI. Editorially reviewed. Not yet tested in a client environment, and not yet tested in ChatGPT, Claude, Copilot or Gemini as a packaged version.
