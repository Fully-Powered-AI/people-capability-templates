# Departing-employee knowledge capture: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-09

The inputs are the invented example in `public/example.md` (a made-up specialty food distributor, an invented purchasing lead and invented notes). No client data was used. The run was one attempt, by an assistant that did not write the template, following the instruction block in `member/template.md` and the output format as written.

## Inputs used

- Stage one: the role brief, the knowledge area list, the purchasing lead's own list and the settings, as given in "Stage one: the inputs" in `public/example.md`.
- Stage two: the guide this run produced in stage one (not the example's guide), the two sets of session notes, and today's date, Wednesday 25 November 2026, as given in "Stage two: the inputs".

Two things weakened the test, and they are stated here so the result is not read as cleaner than it was. First, the run read the stage two notes before writing the stage one guide, because they sit in the same file as the stage one inputs. One stage one question ("What do you do when supply is short?") picked up a detail that only the notes contain. Second, the first thirteen lines of the example's stage one output (the header with its counts) were seen by accident before the run's own output was written. The dates, the priority bands and the counts were then worked out again by hand and agreed. A cleaner trial would give the assistant the stage one inputs alone.

## What came out

The full output of both stages follows, as produced (role titles are written in lower case inside sentences).

~~~~
STAGE ONE

KNOWLEDGE CAPTURE INTERVIEW GUIDE: Purchasing lead, Buying team

For: Operations director. Status: draft for the Operations director's approval.
Change: leaving the company. Last day in the role: Friday 4 December 2026. Prepared: Monday 9 November 2026.
Successor: Buyer.
Working days left: 19, from Monday 9 November to Friday 4 December. Not working: Thursday 26 November (office closed).
Sessions: 2 of 60 minutes, held by Friday 27 November (5 working days before the last day). Draft handover document checked by the departing purchasing lead by Wednesday 2 December.
From: knowledge area list (3 areas); the departing purchasing lead's own list (1 area); settings (all supplied, no defaults used).
Areas: 4 (3 first, 1 second, 0 third priority). Decisions: 2.
Left out: nothing.

Before each session
Record only with the departing purchasing lead's agreement; otherwise type numbered notes.
For each point, ask who else knows it and where it is written down.
Write down their own words wherever they say how something must be done.
Leave out why they are leaving, their health, pay and performance.

Opening, to read at the start of each session
"This conversation is about keeping what you have learned as Purchasing lead working after you hand it on. It is not a review of your work. I will note what you say, and you will check the draft before anyone else reads it. I will only record if you agree."

Questions for every area
1. Take me through the last time this came up, from start to finish.
2. How can you tell, before anyone complains, that this is going wrong?
3. What do you settle yourself here, what do you pass up, and to whom?
4. What is promised or under way right now, to whom, and by when?
5. Who else could answer these questions, even in part?

Areas, in priority order
A1 Holiday peak ordering · Session 1 · Priority: first (nobody else stated as knowing it; customers depend on it)
Covers: Ordering for the November-December peak: quantities and timing for the top 40 lines. Depends on it: Sales team; customers. Others who know it: not stated. Written down in: Partly: last year's peak spreadsheet.
How: conversation; go through last year's peak spreadsheet together.
Also ask: "Going through last year's peak spreadsheet, which parts do you skip, change or add to?" "Besides your usual contacts, whose word settles things at customers?" "Tell me about a time things went badly with customers. What put it right?" "How do you settle the quantities and the timing for the top 40 lines?" "What makes you change an order once it is placed?"
FLAG, others not stated: the list leaves "Others who know it" blank; not treated as someone else knowing it. See decision 1.

A2 Two main cheese importers · Session 1 · Priority: first (nobody else knows it; suppliers depend on it)
Covers: The relationship with the two importers that supply most of the cheese range. Depends on it: Suppliers; Finance manager. Others who know it: None. Written down in: None.
How: conversation.
Also ask: "Besides your usual contacts, whose word settles things at the importers?" "Tell me about a time things went badly with the importers. What put it right?" "How does each importer like to be dealt with?" "What do you do when supply is short?"

A3 Italian container freight (added by the departing purchasing lead) · Session 2 · Priority: first (nobody else has dealt with the forwarder, in her words)
Covers: booking the Italian containers with the freight forwarder (from her email). Depends on it: not stated. Others who know it: None (from her email: "nobody else has dealt with them"). Written down in: not stated.
How: conversation.
Also ask: "What do you check with the forwarder when you book?"
FLAG, depends on it not stated, written down in not stated: her email gives neither. See decision 2.

A4 Short-dated stock · Session 2 · Priority: second (partly known by the Warehouse lead; written down in GI-04)
Covers: What happens to stock that arrives with less shelf life than agreed. Depends on it: Warehouse lead; customers. Others who know it: Partly: Warehouse lead. Written down in: Goods-in procedure GI-04.
How: conversation; go through Goods-in procedure GI-04 together.
Also ask: "Going through Goods-in procedure GI-04, which parts do you skip, change or add to?" "Besides your usual contacts, whose word settles things at customers?" "Tell me about a time things went badly with customers. What put it right?" "What do you do when stock arrives short-dated?"

Session plan
Session 1 (60 minutes, by Friday 27 November): A1, A2. Invite: Buyer.
Session 2 (60 minutes, by Friday 27 November): A3, A4; closing questions. Invite: Buyer; Warehouse lead for A4.

Closing questions, in the last session
1. Which ideas have been tried here and dropped? What would you say if one came up again?
2. What do people come to you for that is not in your role description?
3. Which question do you get asked most, and what is the answer?
4. What have I not asked that will catch your successor out in the first month?

Decisions before the sessions: 2
1. A1, others not stated. For: Operations director. The list leaves "Others who know it" blank for Holiday peak ordering. Who else, if anyone, knows this area?
2. A3, depends on it not stated, written down in not stated. For: Operations director. The purchasing lead's own list names the area and says nobody else has dealt with the forwarder, but does not say who depends on it or where it is written down. Who depends on it, and is anything written down?

Draft for the Operations director's approval. No session has been booked and nothing has been sent.

STAGE TWO

KNOWLEDGE HANDOVER DOCUMENT: Purchasing lead, Buying team

For: Buyer, from the departing purchasing lead. Owner: Operations director.
Status: Draft. The departing purchasing lead checks it by Wednesday 2 December; the Operations director approves it before it is shared.
Last day in the role: Friday 4 December 2026. Prepared: Wednesday 25 November 2026.
From: interview guide of Monday 9 November 2026; Session 1 (Monday 16 November: Purchasing lead, Operations director, Buyer); Session 2 (Tuesday 24 November: Purchasing lead, Operations director, Buyer, Warehouse lead); documents named: last year's peak spreadsheet, Goods-in procedure GI-04.
Areas: 5 (4 from the guide, 1 raised in the sessions). Commitments: 4. Questions to settle: 5.
Held by nobody else: A2, A3, A5.
Left out: the reason for leaving (Session 2, note 14).

Areas
A1 Holiday peak ordering · Priority: first · Covered in Session 1
What to know: Peak orders for the top 40 lines go in by the second week of October. Top-ups go in by 20 November at the latest, because the importers stop taking December changes after that. The Buyer has placed peak orders with her for two years and knows the quantities, but has never done the top-ups alone.
When it matters: Peak orders, second week of October. Top-ups, by 20 November.
Exceptions: Last year's spreadsheet is right on quantities but wrong on the panettone line. It shows one delivery. She splits it into two, late October and mid-November, because the warehouse ran out of space in 2025. The spreadsheet was never updated.
Warning signs: When the two largest restaurant-group customers stop sending their weekly forecasts in early November, they are usually moving some volume to a cash-and-carry. She cuts the top-up by about a fifth.
Decides alone / passes up: She places top-ups within the agreed peak budget herself. Anything above the peak budget goes to the Operations director.
Who else can help: Buyer: knows the quantities from placing peak orders with her for two years; has not done top-ups alone.
Written down in: last year's peak spreadsheet; differs from what was said: see question 1.
How sure: Their account; check with the Buyer on the quantities.
Source: Session 1, notes 1-6.

A2 Two main cheese importers · Priority: first · Covered in Sessions 1 and 2
What to know: Importer one: the account manager is the day-to-day contact, but the owner signs off any price or allocation change. She calls the owner directly once a year, in January, before the price round. Importer two prefers email to calls. Orders by Tuesday noon for Friday delivery; anything later slips a week. Both importers close from 23 December to 4 January. The question she is asked most is "Can we get X for a customer by Friday?"; the answer turns on importer two's Tuesday noon cut-off.
When it matters: January, before the price round. Tuesday noon each week. Last orders for early January go in by Tuesday 15 December. In short years, when the importers ration popular cheeses.
Exceptions: In 2024 a pallet from importer two arrived warm. It was settled by a credit note because she sent the temperature logger readings within 24 hours. Without the logger readings they refuse claims.
Warning signs: none raised.
Decides alone / passes up: In short years she agrees the allocation herself. Price changes above 5% go to the Finance manager.
Who else can help: nobody else named. The Finance manager sees the invoices only; nobody else has spoken to importer one's owner.
Written down in: nowhere.
How sure: Their account; nobody else named.
Source: Session 1, notes 7-12; Session 2, notes 11, 12.

A3 Italian container freight (added by the departing purchasing lead) · Priority: first · Covered in Session 2
What to know: Two containers a year from Italy, booked with the freight forwarder about eight weeks before the shipping date. The forwarder's quotes leave out port storage. She always gets the free storage days in writing, because the port charges by the day after that.
When it matters: The next booking, for the March container, is due in the first week of January.
Exceptions: none raised.
Warning signs: If the forwarder has not confirmed a vessel two weeks before the shipping date, call. A booking has been bumped before.
Decides alone / passes up: She books within the freight budget herself. Anything over goes to the Operations director.
Who else can help: nobody else named.
Written down in: her own email folder "Italy freight", not shared; personal place only: see question 2.
How sure: Their account; nobody else named.
Source: Session 2, notes 1-5.

A4 Short-dated stock · Priority: second · Covered in Session 2
What to know: GI-04 says reject anything under 60% of its shelf life. Customers are never sent stock under 50%. The sales team is told, so they can tell the customer about the shorter date.
When it matters: When stock arrives with less shelf life than agreed.
Exceptions: In practice she accepts cheese from the two importers down to 50% if a customer's standing order will use it within the week, and notes it on the delivery note.
Warning signs: Two short-dated deliveries in a month from one supplier usually means they are clearing old stock before a price change.
Decides alone / passes up: She accepts importer cheese down to 50% herself under the exception above. What she passes up: not covered.
Who else can help: Warehouse lead: applies GI-04 as written and did not know about the 50% exception.
Written down in: Goods-in procedure GI-04; differs from what was said: see question 3.
How sure: Disputed: the Warehouse lead said he applies GI-04 as written, rejects, and she then overrides by phone; see question 3.
Source: Session 2, notes 6-9.

A5 Substitutions on customer orders · Priority: not set · Raised in Session 2
What to know: The warehouse asks her to approve any substitution on customer orders. The rest: not covered.
When it matters: not covered.
Exceptions: none raised.
Warning signs: none raised.
Decides alone / passes up: not covered.
Who else can help: nobody else named.
Written down in: not stated.
How sure: Their account; nobody else named.
Source: Session 2, note 13.

Commitments and coming dates
C1 Top-up order for the chocolate gift lines, drafted but not placed · For: the supplier · Due: Friday 20 November 2026 · Area: A1 · Takes over: to decide: see question 5 · Date passed. Source: Session 1, note 5.
C2 A January meeting with importer one's owner, promised · For: not said · Due: January, date not set · Area: A2 · Takes over: to decide: see question 5. Source: Session 1, note 11.
C3 Booking for the March container with the freight forwarder · For: not said · Due: first week of January, as the notes give it · Area: A3 · Takes over: to decide: see question 5. Source: Session 2, note 1.
C4 Last orders to the importers for early January · For: both importers · Due: Tuesday 15 December 2026 · Area: A2 · Takes over: to decide: see question 5. Source: Session 2, note 12.

Not to try again
N1 A group buying arrangement with two other distributors for better cheese prices, 2022 · Why it failed: it fell apart over who paid for storage and left a stock dispute that took months · If it comes up again: agree storage costs in writing first. Source: Session 2, note 10.

People to know
Importer one's account manager · day-to-day contact · not said. Source: Session 1, note 7.
Importer one's owner · signs off any price or allocation change · she calls directly, once a year in January. Source: Session 1, note 7.
Importer two · orders by Tuesday noon for Friday delivery · prefers email to calls. Source: Session 1, note 8.
Finance manager · price changes above 5% · not said. Source: Session 1, note 10.
Operations director · anything above the peak budget or the freight budget · not said. Source: Session 1, note 4; Session 2, note 4.
Freight forwarder · the Italian containers · not said. Source: Session 2, notes 1-3.
Warehouse lead · applies GI-04; asks her to approve substitutions on customer orders · not said. Source: Session 2, notes 7, 13.
The two largest restaurant-group customers · weekly forecasts in early November · not said. Source: Session 1, note 3.

Questions to settle before Wednesday 2 December
1. A1, differs from what was said. For: Operations director. Last year's spreadsheet shows one panettone delivery; she splits it into two, late October and mid-November (Session 1, note 2). Should the spreadsheet be corrected, and by whom?
2. A3, personal place only. For: Operations director. The booking steps are in her own email folder "Italy freight", not shared (Session 2, note 5). Where should the steps be kept for the successor?
3. A4, differs from what was said, disputed. For: Operations director. GI-04 says reject under 60%. She accepts importer cheese down to 50% when a standing order will use it within the week; the Warehouse lead applies GI-04 as written, did not know of the exception, rejects, and she overrides by phone (Session 2, notes 6, 7). Which is the rule?
4. A5, raised in the sessions. For: Operations director. The warehouse asks her to approve any substitution on customer orders (Session 2, note 13); nothing more was said. Should the area be covered with the purchasing lead before her last day?
5. Commitments, no one named. For: Operations director. C1 to C4 have no one named to take them over. C1's date, Friday 20 November, has passed; the notes of 16 November say the order was drafted and not placed, and do not say whether it has been placed since (Session 1, note 5). Who takes over each?

Draft. Not yet checked by the departing purchasing lead or approved by the Operations director. Nothing has been shared or sent.
~~~~

## What was observed

**Every required part was produced.** Stage one: the header with counts, the before-each-session list, the opening, the five questions for every area, four areas in priority order with flags, the session plan, the four closing questions, two decisions, the closing line. Stage two: the header, five areas (four from the guide, one raised in the sessions), four commitments, one not-to-try-again entry, the people to know, five questions and the closing line. Nothing in the instructions told the assistant to stop: the last day, the list, the headers, the guide and the notes were all present, nobody was recorded without agreement, and no sign-in detail appeared. The reason for leaving (Session 2, note 14) was left out and named by kind only.

**The rules gave clear answers on the hard parts.** The working-day count (19, with the office closure on Thursday 26 November), the finish date (Friday 27 November) and the check date (Wednesday 2 December) came straight from the rules. The blank "Others who know it" cell was treated as not stated, ranked first and flagged. The purchasing lead's own area was numbered after the manager's within its band. The warm-pallet, 60% and 50% account was shown as differing and disputed, with a question and neither version chosen. The chocolate top-up was listed as a commitment with "Date passed". Nobody was chosen to take over any commitment.

**Where the instructions were ambiguous and a guess was needed:**

1. *Is the successor "someone else who knows it"?* In area A1 the Buyer knows the quantities from two years of peak orders. The run listed the Buyer under "Who else can help" and so did not put A1 on the "Held by nobody else" line. The template does not say whether the successor counts.
2. *Does a colleague who only sees part of the picture count as someone else?* In A2 the Finance manager sees the invoices only. The run wrote "nobody else named" and put A2 on the "Held by nobody else" line. The example treats the Finance manager as a person to check with. The rule for "how sure" and for that header line does not settle it.
3. *The "Document" question kind.* The output format lists "Document" as a kind of question, but no step says when one is raised. None was raised here.
4. *"Documents named".* Whether a folder in someone's own mailbox, or a delivery note, counts as a document for the From line is not said. The run listed only the peak spreadsheet and GI-04; the example also lists the email folder.
5. *Questions about an outside party named only as a class.* The instruction is to name the party, but A1 and A4 depend on "customers". The result ("whose word settles things at customers?") reads awkwardly. Also, the freight forwarder is plainly an outside party, but because "Depends on it" was not stated for that area, the two outside-party questions were not asked for it.
6. *Where a fact goes inside an area.* The panettone split could sit under "What to know" or under "Exceptions". The run put it under "Exceptions"; the example puts it under "What to know".
7. *"For whom" on a commitment.* The notes do not say whom the January meeting or the March booking are for. The run wrote "not said"; the example filled in the owner and the forwarder. The template says to give only what the notes give, so the run's reading seems the stricter one, but the template does not say what to write when a party can be inferred.
8. *A date without a year or a day.* "First week of January" and "January" were copied as the notes give them. The template does not say whether to add the year.
9. *Closure periods.* "Both importers close from 23 December to 4 January" is a coming date but not a deadline. The run put it in the area's text and made only the 15 December order date a commitment. The template says "dated deadline" and does not cover closures.
10. *Capitalisation of roles.* The format uses "[role]" in the opening and headers. The run capitalised it in the headings and the guide's own title line and used lower case in sentences; the example does the same in places but not consistently.
11. *Reading "nobody else has dealt with them".* The purchasing lead wrote this about the forwarder. The run used it to fill "Others who know it: None" for the whole area, as the template's rule about filling fields from the person's words allows, and said so in the field. The example does the same.
12. *The 20 November top-up cut-off.* It is a stated deadline that has already passed by the stage two date. The template lists only promises under way and dated deadlines after today, so it is not a commitment, and the run left it in "What to know". A reader might expect it to be flagged.

**Differences from the published example as it stood at the time of the run** (beyond wording, which differs throughout; the example has changed since, as "Changes made after this run" below explains, so some of these no longer hold):

- "Held by nobody else": the run named A2, A3 and A5; the example names A3 and A5 (see ambiguity 2).
- A2 "How sure": the run gave "nobody else named"; the example gave "check with the Finance manager".
- A1: panettone under "Exceptions" in the run, under "What to know" in the example, which says "Exceptions: none raised". The run's source line covers notes 1 to 6; the example's leaves out note 5.
- Commitments C2 and C3: the "For" field differs (ambiguity 7).
- The From line of stage two: the run lists two documents; the example lists three (ambiguity 4).
- The "Also ask" questions are different questions drawn from "what the area covers"; the template allows this.
- The run's decisions and questions are worded differently but cover the same areas and raise the same issues. Both outputs have 4 areas, 2 decisions, 5 areas in the handover document, 4 commitments and 5 questions.
- Area A5's name: "Substitutions on customer orders" in the run, "Substitution approvals" in the example.

**Facts in either output that are not in the inputs:**

- In the run: the stage one question "What do you do when supply is short?" for A2 (the idea comes from stage two note 10, which the run had already read). The run found no other fact in its own output that the inputs do not support.
- In the example: "Finance manager ... decides price changes above 5%" (the notes say such changes "go to" the Finance manager); C3 "For: the freight forwarder" and C2 "For: importer one's owner" (the notes do not say); "the importers stop taking December changes" is attributed in A1 to the importers as the notes say, but the notes do not say which importers. These are small, and none changes the meaning.

**Shortcomings of the template found in this trial:**

- It is long. The instruction block is shorter than the procedure above it, but a person pasting only the block would lose the exact wording of some rules (for example how "Others who know it" is read when a person's own words answer the field), so the two have to be kept in step.
- The "how sure" and "held by nobody else" rules depend on a judgement (ambiguities 1 and 2) that two careful readers resolved differently.
- The acceptance tests in the template have not been run by this trial. This trial covered one complete path through both stages and so exercised tests 3, 4, 6, 7, 8 and 9 in practice (all behaved as the test expects); it did not exercise tests 1, 2, 5, 10 or 11.
- The version notes in `member/template.md` still say the template has not been tried on its invented example in a named AI product. That line was left alone, as the task allowed changes only to the trial record and the evidence field.

## Changes made after this run

The template, the published example and the public profile were revised on 9 November 2026, after this run and after an independent review, to settle what the run found. These edits have not been run again. The output and the observations above are as recorded; where they compare this run with the published example, they describe the example as it stood at the time of the run. None of the edits changes an area, a priority band, a date, a flag, a decision, a commitment, the left-out line or the number of questions to settle on the example. Each edit is listed with whether the output recorded above fits it.

- **Evidence lines.** The public profile and the template's version notes now say the template was tried on its invented example in Claude on 9 November 2026, which settles the last shortcoming above.
- **Who counts as someone else (ambiguities 1 and 2).** Procedure step 12 and pasted step 9 now say the successor counts for whatever the notes say they know, and a colleague the notes say sees only a result of the work, such as the invoices, does not: the field reads "nobody else named", then that colleague with the limit, and the area goes on the "Held by nobody else" line. This settles both as this run chose, so the run's A1, A2 and header line fit. The example now matches: its header line names A2, A3 and A5, its A2 "How sure" reads "Their account; nobody else named", and the Finance manager follows "nobody else named" with the limit.
- **The "Document" question kind (ambiguity 3).** The pasted instructions now name the two document-wide kinds, check date to set and successor not named, as procedure step 15 already did. The run raised none, which fits.
- **Documents named (ambiguity 4).** The From line's documents named are now every document, file, folder or register the guide or the notes name as holding part of the work, a personal place included, and not a form the work is only noted on, such as a delivery note. The run does not fit: under the revised rule its From line would also list the email folder "Italy freight", as the example does.
- **Outside parties (ambiguity 5).** A party listed only as a class is named in the singular ("each customer", "a customer"), and an outside party named in what the area covers, or in the departing person's words for it, gets the two outside-party questions even when "Depends on it" does not name it. The run does not fit: its "at customers" would read "at each customer", and its A3 would carry the two freight forwarder questions. The example's A3 now carries them.
- **Where a fact goes inside an area (ambiguity 6).** What to know is how the work runs now, including a standing practice that differs from a document; Exceptions are the cases, with their conditions, where that usual way does not hold. This settles it as the example had it; the run's panettone split under "Exceptions" does not fit.
- **"For whom" on a commitment (ambiguity 7).** It is the party the notes name, or the party the commitment itself names (a meeting with an owner, an order to a supplier, a booking with a forwarder); otherwise "not said". This settles it as the example had it; under it the run's "not said" for C2 and C3 would read importer one's owner and the freight forwarder.
- **Dates (ambiguity 8).** Dates are given as the notes give them, with a year added only where the notes or the role brief make it certain. The run fits; the year it added to C1 and C4 is certain from the brief.
- **Closures (ambiguity 9).** A closure or other period that is not a deadline goes under "When it matters", as the example had it. The run put the importers' closure under "What to know", which does not fit.
- **A passed cut-off (ambiguity 12).** A recurring cut-off whose date has passed and that is not under way is not a commitment and stays in its area's text. This settles it as the run chose, so the run fits.
- **Commitment notes in an area's source.** The procedure already said a commitment's note goes to its area's source as well; pasted step 7 now says so too. The example's A1 and A2 source lines now include notes 5 and 11, as the run's already did.
- **Stops in the pasted instructions.** The stop for inputs covering more than one departing person, already in the procedure, is now in the pasted instructions, and stage two's "If either is missing" now names the guide or the notes. This run exercised neither.
- **Wording.** The example's A2 now says price changes above 5% "go to" the Finance manager, as the notes do. In the output format, the What to know hint now reads "the point itself", and the section and question label "Not to try again" is now "Tried before and dropped", with entries T1, T2 and so on in place of N1, to keep clear of a phrase in the source method. The run's output uses the earlier labels.
- **After a second independent review.** Pasted step 2 now says a field the departing person's words answer is filled from them and says so, and pasted step 5 now gives the "How:" line rule; both were already in the procedure and the output format, and the run did both. In the example, A4's "What to know" now says that the purchasing lead accepts some importer cheese below GI-04's 60%, pointing to the conditions under "Exceptions"; A4's "Decides alone / passes up" now ends "what she passes up: not covered", the output format's own phrase, as the run's did; and the Warehouse lead's line under "People to know" now cites note 7 only, since note 13 says "the warehouse", not the Warehouse lead. The run's own People to know line cites note 13 for the Warehouse lead in the same way.
- **Not changed.** Ambiguities 10 (capitalisation of roles) and 11 (filling a field from the person's own words) needed no change.

One deviation in the run was not listed above: in its commitments it printed "Takes over:" where the output format says "Takes it over:". The output is left as the run produced it.
