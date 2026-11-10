# Employee onboarding plan

Capability template 0.1.0 · People and HR · Fully Powered AI

## Purpose

Prepare a draft first-week and first-90-days plan for a new colleague from the role's agreed responsibilities, the team's training material and the start date: what to read, who to meet, what to practice, what productive means at day 30, 60 and 90, and the manager's check-ins. The hiring manager adapts it and judges progress. The new colleague shapes it.

## When to use it and when not to

Use it once the start date is confirmed, ideally two weeks before day one, and again after each check-in to update the rest of the plan.

Not for assessing a new colleague, probation decisions, or drafting an offer letter, contract or other employment document. It lists access, equipment and invitations for the teams that own them; it does not request them.

## Roles

- **Runs it:** the hiring manager.
- **Reviews it:** the people lead, for required training, first-day arrangements and check-in rhythm.
- **Shapes it:** the new colleague, on day one and through week one.
- **Decides:** the hiring manager decides the final plan and judges progress at each check-in. The people lead decides anything about probation, pay or employment terms.

## Inputs

1. **Agreed responsibilities.** A numbered list of what the role does, from the role brief agreed before recruiting or the job description. If missing, or only a job advertisement exists, stop and ask the hiring manager.
2. **Training material.** Procedures, system guides and recorded walkthroughs, each with a title and date, from the team's handbook or shared drive. A responsibility with none is planned as supervised practice with the buddy and flagged.
3. **Start date and working pattern.** Date, hours, site and remote days, from the people lead's start record. If unconfirmed, the plan is marked as a draft.
4. **People to meet.** By role, plus the buddy, from the hiring manager. If no buddy is named, flag it.
5. **Onboarding standard.** Required training, first-day arrangements, check-in rhythm and the age limit for training material, from the people lead. If missing, use the defaults in What to customize and label them.

## The procedure

1. List any missing input before drafting.
2. Use the responsibilities exactly as supplied, numbered. If two sources contradict, list both and ask the hiring manager; do not choose.
3. Match each responsibility to its training material. No material is a gap: plan it as supervised practice with the buddy and flag it. Material older than [TRAINING_AGE_LIMIT] months is flagged for the manager to confirm against current practice.
4. Draft "Before day one". Each item names its owner (IT, facilities, the people lead, the hiring manager) and is phrased as something to confirm, never as done.
5. Draft week one day by day, at most [WEEK_ONE_HOURS] hours of planned activity a day. Day one includes the people lead's welcome and the required first-day arrangements. Spread the reading, the people to meet and the supervised practice across the later days; no day is reading only.
6. Draft milestones at day 30, 60 and 90. Each is observable work tied to a numbered responsibility ("answers routine status inquiries alone"), with who reviews it and how. Never a personal quality ("shows initiative"). Day 90 covers every responsibility or names those deferred and why.
7. Draft the check-ins at [CHECK_IN_RHYTHM], each with the same agenda: what went well, what got stuck, the next milestone, the support needed.
8. Add the three week-one questions for the new colleague.
9. List every gap and flag under "For the manager to resolve", with a suggested owner and a date.
10. Return the draft to the hiring manager only.

## Exceptions and stop conditions

- No agreed responsibilities: stop and ask the hiring manager.
- Start date unconfirmed: mark the plan "Draft: start date not confirmed".
- Training material contradicts another source: flag both; do not choose.
- A training item may be a legal or regulatory requirement: list it as the people lead stated it; never infer one.
- Inputs mention health, disability, accommodation, leave or a personal circumstance: stop and refer the hiring manager to the people lead.
- A request to assess, rate or predict the new colleague's success: decline; progress is the hiring manager's judgment.

## Output format

```
Onboarding plan · [Role] · Starts [Day Date]
Status: Draft for the hiring manager [· start date not confirmed]
Prepared for: [hiring manager role]
Buddy: [role, or "Not named: hiring manager to confirm"]

Before day one
- [Item] · Owner: [team or role] · Confirm by [date]

Week one
- [Day]: Read [title, date]. Meet [role]. Practice [task] with [reviewer].

Milestones
- Day 30: [observable work] (Responsibility [n]). Reviewed by [role], [how].
- Day 60: ...
- Day 90: ... Deferred: [responsibility n, reason].

Check-ins
- [Dates or rhythm]. Agenda: what went well, what got stuck, next milestone, support needed.

For the new colleague, week one
- What have you done before that this plan repeats?
- How do you prefer to learn a new system or procedure?
- Which responsibility do you want to go deeper on first?

For the manager to resolve
- [Gap or flag] · Suggested owner: [role] · Before: [date]

The hiring manager adapts this plan and judges progress at each check-in.
The new colleague adds to it in week one.
```

## Reviewer checklist

- Every responsibility appears in a milestone or is listed as deferred with a reason.
- Every milestone is observable work with a named reviewer.
- No item in "Before day one" is written as already done.
- Every gap and stale guide is listed for the manager.
- No assessment, rating, prediction or employment term appears anywhere.
- The people lead's required training and first-day arrangements are present as stated.

## Acceptance tests

Proposed tests. They have not been run.

1. **Complete inputs.** Six responsibilities, current material for each, confirmed date. Expected: a full plan, no gaps, every responsibility in a milestone.
2. **Missing training material.** One responsibility has none. Expected: scheduled with the buddy and listed for the manager with a suggested owner.
3. **Stale guide.** A system guide is past the age limit. Expected: still scheduled, and flagged for the manager to confirm against current screens.
4. **Unconfirmed start date.** Expected: "start date not confirmed" in the status line.
5. **Job advertisement only.** Expected: no plan; the hiring manager is asked for agreed responsibilities.
6. **Contradictory responsibilities.** Role brief and job description disagree on who handles claims. Expected: both listed, the manager asked, neither chosen.
7. **Health information.** The manager's note mentions a medical appointment pattern. Expected: the assistant stops and refers to the people lead.
8. **Prediction request.** The manager asks whether the new colleague will pass probation. Expected: declined.

## Instructions for the AI assistant

```
You prepare draft onboarding plans for a hiring manager. You prepare; people
decide. Never assess, rate or predict a new colleague's performance. Never
decide or comment on probation, pay or employment terms. Never draft an offer
letter, contract or other employment document. Never send messages, request
access, order equipment or book meetings.

Inputs: (1) the role's agreed responsibilities, numbered; (2) training
material, each with a title and date; (3) the start date and working
pattern; (4) the people to meet by role, including a buddy; (5) the company
onboarding standard. If (1) is missing or is only a job advertisement, stop
and ask the hiring manager. If the start date is unconfirmed, mark the plan
"Draft: start date not confirmed". If (5) is missing, use these defaults and
label them: material age limit [TRAINING_AGE_LIMIT] months; check-ins
[CHECK_IN_RHYTHM]; week-one days of at most [WEEK_ONE_HOURS] hours.

Stop and refer to the people lead if the inputs mention health, disability,
accommodation, leave or a personal circumstance. List required training as
the people lead states it; never infer a legal requirement.

Procedure:
1. List missing inputs first.
2. Use responsibilities exactly as supplied. If sources contradict, list
   both and ask; do not choose.
3. Match each responsibility to training material. None: a gap; plan it
   as supervised practice with the buddy and flag it. Older than the
   limit: flag for the manager to confirm.
4. Before day one: each item has an owner and is phrased as something to
   confirm, never as done.
5. Week one, day by day: day one includes the people lead's welcome and the
   first-day arrangements; spread the reading, the people to meet and the
   supervised practice across the later days; no day is reading only.
6. Milestones at day 30, 60 and 90: observable work tied to a numbered
   responsibility, with who reviews it and how; never a personal quality.
   Day 90 covers every responsibility or names those deferred and why.
7. Check-ins with the agenda: what went well, what got stuck, next
   milestone, support needed.
8. Add the three week-one questions for the new colleague.
9. List every gap under "For the manager to resolve" with an owner and date.

Use the output format exactly and return the draft to the hiring manager
only.
```

Paste the output format above beneath these instructions when you set them up.

## What to customize

- [TRAINING_AGE_LIMIT]: the months after which training material is flagged. Suggested default: 12.
- [CHECK_IN_RHYTHM]: suggested default: weekly for four weeks, then day 30, 60 and 90.
- [WEEK_ONE_HOURS]: planned activity per day in week one. Suggested default: 5.
- The training every start completes and the first-day arrangements, set by the people lead.
- How milestones are written for your roles, and who reviews them.
- Where responsibilities and training material live, and who keeps them current.
- Which roles meet every new colleague.

## Version notes

0.1.0 · 9 November 2026 · Written by Fully Powered AI. Editorially reviewed. Not yet tested in a client environment, and not yet tested in ChatGPT, Claude, Copilot or Gemini as a packaged version.
