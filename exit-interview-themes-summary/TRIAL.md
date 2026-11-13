# Exit interview themes summary: a trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (claude-sonnet-5-5)
- **Date:** 2026-11-12

The inputs were the invented example's own: the settings, leaver list, exit notes, leaver forms and last period's extract in [example.md](example.md), sections 1 to 5. No client data was used. This is the second run, repeated once after an independent review. The first run found eight ambiguities; after the template was edited to settle them, the same session ran it again. A reviewer then found that the instruction block did not hold the starter theme list, and one sentence in the example's inputs ("Told my manager twice.", on L-05's form) did not trace under the example's own coding. The block was edited (the starter theme list and its order now sit inside it, and a step to list each leaver's recorded and main-reason themes before counting was added), the sentence was dropped from the inputs, and the template was run again. The record below is of that latest run. It is not independent of the earlier runs: the same session made the edits, had seen the earlier outputs and the published example, and ran the template again. I followed the edited instruction block and the output format, with the settings and inputs as given and nothing else, wrote the summary, and only then compared it with the published example and the reviewer checklist.

## What came out

```
EXIT INTERVIEW THEMES SUMMARY: 1 July to 30 September 2026

For: HR lead. Status: draft for the HR lead's approval before anyone else reads it.
Prepared: 5 October 2026, from the leaver list (13 rows), 8 exit notes, 8 leaver forms, last period's summary (extract).
Settings: smallest group 5, smallest count 2, quotes per theme 2, question threshold 3, leaving types Resigned. Defaults used for: the starter theme list, and a proposed reason mapping.
Anonymity: no group under 5 leavers with an exit record is shown, small teams are combined or the team view withheld, no theme raised by fewer than 2 leavers is named, and no quote carries a name, team, role or personal detail.

1. Coverage
Leavers in the period: 13. In scope (Resigned): 11. Out of scope: 2 (Fixed term ended 1, Company decision 1).
With an exit record: 10 of 11 (6 note and form, 2 note only, 2 form only). No exit record: 1.
All records matched.

2. Themes (raised by, of 10 leavers with an exit record)
Workload and hours: raised by 6; main reason for 4; recorded as the reason for 1.
  "The weekend rota made it hard to plan anything."
  "Covering two queues for most of the year after [a colleague] left."
Career growth: raised by 3; main reason for 3; recorded as the reason for 5.
  "I'd have stayed for a path to senior."
  "After the reorganisation in May nobody could tell me what the senior track looks like now."
Company direction and change: raised by 3; main reason for 0; recorded as the reason for 0.
  "Decisions about [our plans] changed every quarter after the reorganisation."
Personal circumstances: raised by 2; main reason for 2; recorded as the reason for 2.
  Not quoted: personal circumstances are counted, never quoted.
Pay and benefits: raised by 2; main reason for 1; recorded as the reason for 2.
  "The pay rise elsewhere was nice but I'd have stayed for normal hours."
  Withheld: 2 comments that could not be made anonymous.
Other: 2 topics raised by one leaver each, named in the HR note only.
Main reason not stated: 0.

3. What leavers said beside what was recorded
Recorded at the time: Workload and hours 1, Career growth 5, Personal circumstances 2, Pay and benefits 2, not stated 0.
Leavers' own main reasons: Workload and hours 4, Career growth 3, Personal circumstances 2, Pay and benefits 1, not stated 0.
Compared: 10. Same theme: 7. Different: 3.
Recorded as Career growth, main reason Workload and hours: 2. Other differences: 1.
Reason mapping proposed, for the HR lead to confirm: Career move -> Career growth; Better pay elsewhere -> Pay and benefits; Personal reasons -> Personal circumstances; Relocation -> Personal circumstances; Work-life balance -> Workload and hours.

4. By team (leavers with an exit record)
Customer Support: 6 in scope, 5 with an exit record. Raised by 2 or more: Workload and hours 5.
Engineering, Product, Sales (combined): 5 in scope, 5 with an exit record. Raised by 2 or more: Career growth 2; Company direction and change 3.
Teams combined because each had fewer than 5: Engineering, Product, Sales.

5. Recommend and spoken well of
Would recommend working here: Yes 3, Unsure 3, No 2, of 8 forms.
Spoken well of: Team and colleagues 2.

6. Since last period
Workload and hours: 2 of 7 then, 6 of 10 now.
Career growth: 3 of 7 then, 3 of 10 now.
Company direction and change: not shown last period, 3 of 10 now.
Personal circumstances: 2 of 7 then, 2 of 10 now.
Pay and benefits: 3 of 7 then, 2 of 10 now.

7. Questions for leadership
1. Workload and hours. Raised by 6 of 10 leavers and the main reason for 4; recorded as the reason for 1; all 5 leavers with an exit record in Customer Support raised it. What do you want to understand about how cover and rotas are set?
2. Career growth. Raised by 3 of 10 and the main reason for 3; recorded as the reason for 5. How does someone here find out what the next step is?
3. Company direction and change. Raised by 3 of 10, none of them in Customer Support, and the main reason for none. How are changes explained to the people they affect?
4. Recorded reasons. For 3 of 10, the reason recorded at the time is in a different theme from the leaver's own main reason; for 2 recorded as Career growth, the leaver gave Workload and hours. What is the recorded reason meant to capture?
Carried from last period: Career growth. What path is there from support to senior support, and is it written down? (open). Answered, not carried: 1.

Left out: names of people and companies; where leavers are going and what they were offered; health and family detail. Matters passed to the HR lead outside this summary: 1.
This summary decides nothing about any person and names no one.

NOTE FOR THE HR LEAD ONLY: remove before sharing
Matters for your own process: L-08: a report of abuse by a customer.
Topics raised by one leaver: Manager (L-06). Flexibility and place of work (L-07).
Quotes withheld: L-05, Pay and benefits: 2, each with more than one identifying detail (words pointing to a group smaller than 5, with the leaver's own pay or a kind of work; the form sentence and the quotation on the note's main reason line).
Words replaced in quotes: L-02: a person's name replaced with [a colleague]. L-10: a word pointing to a group smaller than 5 replaced with [our plans].
Main reasons that differ between form and note: None.
Records not used: None.
No exit record: L-09.
To confirm: the proposed reason mapping; the default theme list.
```

## What was observed

The run produced every required part: all seven sections, the Left out line, the closing line and the HR note. Nothing in the instructions told me to stop. The group was big enough (10 leavers with an exit record against a smallest group of 5), every header matched, and the one report of abuse was set aside as step 5 says.

**The starter list now comes with the block.** Theme names, the short definitions that decide where a remark goes (for example that rotas and on-call are Workload and hours, and that one-to-ones are Manager) and the list order used for ties and for the quote tie rule were all in the block, so no outside list was needed. The block and the output format were the only instructions used.

**The per-leaver list worked.** Before counting same and different I wrote down each of the ten leavers with both a recorded and a main reason, side by side, and counted from that list: same 7 (L-01, L-03, L-04, L-05, L-07, L-10, L-11), different 3 (L-02, L-06, L-08). Both counts were right the first time. In both earlier runs they were first miscounted, so the step does what it was added for; one run does not prove it.

**Differences from the published example.** The two outputs agree on every count, every theme, every quote, the team grouping, the since-last-period lines, the carried question and the HR note's contents. They differ in these places only:

- **Questions.** The wording of the open questions differs from the example's. I kept the wording from the earlier record rather than rewording it. All four state counts first and ask one open question. In question 3 I said "none of them in Customer Support" rather than naming the combined group.
- **HR note wording.** The reason given for the withheld Pay quotes is worded in my own words.
- **Small things.** I dropped the "Not stated -> not stated" mapping item (nothing in scope mapped to it) and wrote "last period's summary (extract)".

**Dropping the L-05 sentence.** With "Told my manager twice." gone, Manager is raised by L-06 alone (no one-to-one since March), so it stays under Other, as before. No count, quote or line of the output changed.

**Facts not in the inputs.** I found none. Everything shown (counts, teams, quotes, dates, refs) traces to the inputs.

**Where the instructions were still open.** Subtraction: the company-wide count for Workload and hours is 6 and the Customer Support line says 5, so a reader can work out that 1 leaver in the combined group raised it, below the smallest count. The template now says so as a known limit and leaves the choice of what to share to the HR lead; this run did not hide anything because of it. What counts as a word that points to a group smaller than the smallest group is still a judgement, now steadied by examples in the template; I kept "weekend rota" and "queues" and replaced "roadmap". Mapping "Career move" to Career growth stays a guess for the HR lead to confirm. Two quotes from L-01 and from L-02 appear under different themes, as the template allows (at most one quote per leaver under a theme, so the same leaver can be quoted under two themes).

**Reviewer checklist.** Items 1 to 8 can be checked by hand against this output and its inputs. Item 2 (recounting two themes) and item 6 (every quote verbatim, with replacements listed) hold. Item 9 is a step for the HR lead, not the assistant.
