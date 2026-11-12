# Prebill exception review

Workflow template, version 0.1.0.

## Purpose

Prepare, for one matter's prebill, the exception sheet the billing coordinator puts in front of the billing attorney before the prebill review. The sheet marks every time and expense entry that needs a person's attention: a billed rate that differs from the firm's rate table, a possible duplicate, an entry outside the client's stated billing guidelines, a narrative that is unclear, combines several tasks or carries sensitive detail, an expense with no receipt or invoice behind it, and an adjustment with no approver or reason. Each exception carries the facts, the amount at stake where there is one, and the person it goes to next. The assistant prepares; it never changes, writes down or approves an entry, decides what is billable, rewrites a narrative, or sends anything.

## When to use it and when not to

Use it once the prebill for a matter is generated for the billing period and before the billing attorney reviews it. Run it again from the updated prebill after the timekeepers' corrections and the billing attorney's decisions have been entered in the billing system, so the attorney and finance see what is still open.

Do not use it:

- to write the summary the client reads with the invoice. That comes after the billing attorney's decisions, as a separate piece of work;
- to report a matter's budget, phases or progress to the responsible partner. That is a separate piece of work too;
- to read rates, fee terms or anything else from an engagement letter. The firm's rate table is the only rate source; whoever keeps it enters the agreed rates there;
- to decide whether an entry is billable, whether a guideline binds the firm, or whether a narrative is privileged. Those are the billing attorney's decisions;
- to give legal advice or say anything about the merits of the matter;
- for a matter billed on a fixed fee with no time detail.

## Roles

- **Runs it and gathers the inputs:** the billing coordinator.
- **Rewrites an unclear narrative, splits a block entry into its tasks, or supplies an expense's receipt or invoice:** the timekeeper who recorded the entry, or the person who submitted the expense.
- **Decides billability, rates, duplicates, guideline exceptions, every narrative change and every adjustment:** the billing attorney.
- **Enters the corrections and decisions in the billing system and reruns the sheet:** the billing coordinator.
- **Approves the invoice preparation once the decisions are entered:** finance.

## Inputs

1. **Prebill header,** typed or copied from the prebill: prebill number and date, client, matter name and number, billing period, billing attorney, and four totals: fees before adjustments, adjustments, expenses, and the prebill total. If missing, stop.
2. **Time export:** every time entry on the prebill, one row each. Default column headers: `Entry`, `Date`, `Timekeeper`, `Hours`, `Rate`, `Amount`, `Narrative`. `Amount` is before any adjustment. If missing, stop.
3. **Expense export:** every expense on the prebill. Default column headers: `Entry`, `Date`, `Type`, `Vendor`, `Amount`, `Support`, `Submitted by`, `Description`. `Support` holds the reference of the receipt or vendor invoice, or is blank. If the period has no expenses, the person says so. If the export is missing and the person has not said there are none, stop.
4. **Adjustments export:** write-downs and discounts already entered on the prebill. Default column headers: `Entry`, `Adjustment`, `Approved by`, `Reason`. `Entry` is a time entry number or `invoice`; `Adjustment` is the amount taken off. If there are none, the person says so. If the export is missing and the person has not said there are none, stop.
5. **The firm's rate table:** default column headers `Timekeeper`, `Rate`, `Applies to`, `Effective from`, `Effective to`. `Applies to` is a client's name or `Standard`; a blank `Effective to` means the row is still in effect. If missing, stop. If the person offers the engagement letter instead, do not read rates or terms from it: ask for the rate table.
6. **The client's billing guidelines:** the client's billing rules for outside firms, with their title and date. If the person says the client has none, write "No client billing guidelines for this client" and run every other check. If the client has guidelines and they are not supplied, stop.
7. **Firm settings,** optional. Defaults, used where the person supplies none:
   - narrative minimum: 5 words;
   - vague phrases: attention to; work on; various; miscellaneous; follow up; review file; file review;
   - sensitive words: settle; settlement; lowest; highest; bottom line; walk away; weak; weakness; strong; strength; strategy; advice; advised; opinion; exposure;
   - expense support: every expense needs a support reference, whatever its amount;
   - duplicate window: 3 days for time entries, 7 days for expenses;
   - the preparation date, and the role name of the billing coordinator.
8. **A column map** (optional), when the exports use other headings: which of their columns holds each default column.

**When a header does not match.** If a column the work needs is not found under its default heading and no column map covers it, stop and ask which column holds it. Never guess a column from its contents.

The work runs on exports and documents the person supplies. It needs no connection to the billing system and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Confirm one client, one matter and one billing period across the prebill header and the exports. Check every column the work needs, as above. If two rows in one export share an entry number, or an adjustment names an entry that is not in the time export, stop and ask.
2. **Tie out before anything else.** For each time entry, hours times rate must equal the amount to the cent. Time entries must add to the prebill's fees before adjustments, the adjustments to its adjustments, the expenses to its expenses, and fees less adjustments plus expenses to the prebill total. If any of these fails, stop: report each figure and the difference to the billing coordinator and prepare nothing else.
3. **Sort the client's guideline rules.** Read each billing rule in the guidelines and place it in one of these kinds, with its section number:
   - G1, the time increment, and what happens to entries in another increment;
   - G2, a limit on hours per timekeeper per day;
   - G3, one task per entry, or block entries not paid;
   - G4, kinds of work not billable, by the words the guideline names;
   - G5, timekeepers or classes of timekeeper the client does not pay for;
   - G6, expense types not reimbursed;
   - G7, the amount above which an expense needs a receipt or invoice;
   - G8, a cap on a single expense or an expense type.
   List the sections placed in a kind as checked. Every rule of another kind, every rule whose check needs something not in the exports (such as a prior approval), and every rule that can be read two ways goes under "Not checked", with the reason, and for a rule read two ways both readings. Do not interpret a rule, and do not check a rule placed there. A rule that says "including" before a list is checked on the words it names; add a line under "Not checked" saying that the rest of the rule, beyond those words, is not checked. In the sheet, cite the client's own section number ("Guideline 4"); the labels G1 to G8 appear only under "Guideline rules", beside the sections placed in each kind.
4. **Run the checks in this order.** Each finding is one exception, numbered X1, X2 and so on through the sheet. One finding is written once, in one section; an entry can carry several findings in different sections.
   - **C1, rates.** For each time entry, the table rate is the row for that timekeeper whose `Applies to` is the client's name and whose dates cover the entry's date; if there is none, the `Standard` row whose dates cover it. If two rows qualify, stop and ask. Where the billed rate differs, write one exception per timekeeper and billed rate, in the order of each one's first entry in the time export, listing every entry at that rate, the total hours, and the difference: (billed rate minus table rate) times the hours, stated as above or below the table. If the billed rate matches another row on the table, such as an expired client row or the standard row, say which, with that row's `Applies to` and rate. A timekeeper with no row covering the date: one exception, "no rate on the table", with the entries; no difference is computed.
   - **C2, possible duplicates.** Time entries: same timekeeper, same date and same narrative, whatever the hours; or same timekeeper, same hours and same narrative within the duplicate window. Expenses: the same support reference on two expenses; or same vendor and same amount within the duplicate window. Narratives match when they are the same after ignoring capitals, punctuation and extra spaces. Amount at stake: the amount of the later entry in export order, "if [entry] is the duplicate".
   - **C3, client guideline rules G1, G2, G4, G5, G6 and G8.**
     - G1: hours that are not a whole number of the increment. Amount at stake: the entry's amount where the guideline says such entries are not paid; otherwise "the guideline states no amount".
     - G2: a timekeeper's hours on one date above the limit, listing that day's entries. Amount at stake: the hours over the limit times the rate on the last of those entries in export order.
     - G4: a narrative that contains a word for the kind of work the guideline names, in any form of that word (organize, organized, organizing). Amount at stake: the entry's amount. Use only the words the guideline itself names, and check them in time narratives only, not in expense descriptions.
     - G5: entries by a timekeeper or class the guideline excludes. Amount at stake: the entries' total.
     - G6: an expense whose `Type` is a type the guideline names. Amount at stake: the expense.
     - G8: an expense above a cap. Amount at stake: the amount above the cap.
     Where two of these rules reach the same entry, write one exception that cites both sections, with the amount at stake under each. List the exceptions in the order of the first section each cites, and by date within a section.
   - **C4, narratives.** For each time entry:
     - unclear: the narrative has fewer words than the narrative minimum, or contains a vague phrase from the firm's list;
     - block entry: two or more activities separated by semicolons, or a call, meeting or conference named together with another thing the timekeeper did, shown by a second past-tense verb such as reviewed, prepared or revised. A word like "revised" used to describe a document ("the revised schedule") is not a second activity;
     - sensitive detail: the narrative contains a word from the firm's sensitive list, as a whole word, ignoring capitals. Say which words; do not judge whether the detail is privileged or should change.
     Where the client's guidelines carry a G3 rule, a block entry also cites that section, with the entry's amount as the amount at stake. One exception per entry; an entry that is both unclear and a block entry carries both in one exception. Sensitive detail is always its own exception. List all of section 4's exceptions together by date, sensitive-detail exceptions among them.
   - **C5, expenses without support.** An expense whose `Support` is blank, unless the firm's settings set an amount below which none is needed. Where the client's guidelines carry a G7 rule and the expense is above its amount, cite that section, with the expense as the amount at stake; otherwise say the client's rule does not reach it.
   - **C6, adjustments.** An adjustment with a blank `Approved by` or a blank `Reason`. Say which is missing. Amount: the adjustment.
5. **Route each exception.** Unclear narratives and block entries go back to the timekeeper who recorded them, to rewrite or split with a time for each task. An expense without support goes back to the person in `Submitted by`. Rate differences, possible duplicates, guideline exceptions, sensitive detail and adjustments go to the billing attorney. A returned entry or expense that cites a guideline section also goes to the billing attorney once it comes back, for the billability decision. Route by role even when the billing attorney is also the timekeeper or submitter: the sheet reassigns nothing.
6. **Count and set the status.** Count the exceptions; the time entries named in sections 1 to 4; the expenses named in sections 2, 3 and 5; and the adjustments named in section 6. If there are none: "No exceptions found; ready for the billing attorney's review."
7. **Return the sheet** to the billing coordinator for the billing attorney. The sheet recommends nothing: a decision line may name the courses open, such as keeping or removing an entry, without preferring one, and never says an entry should be written down.

Write each date as the day, the month's name and the year ("4 November 2026"); a date inside the billing period may leave out the year ("14 October"). Write a billing period inside one month as "1 to 31 October 2026", and across months as "28 September to 5 October 2026". Show money to the cent with the thousands separator ("1,476.00").

## Exceptions and stop conditions

- **The tie-out fails:** stop and report the figures and the difference. Never change a figure to make it tie.
- **A header does not match and no column map covers it:** stop and ask which column holds it.
- **The prebill header, the time export or the rate table is missing, or the client has guidelines that were not supplied:** stop and ask.
- **Inputs for more than one client, matter or billing period; two rows sharing an entry number; an adjustment naming an entry not in the time export; two rate rows covering the same entry:** stop and ask.
- **Offered an engagement letter in place of the rate table, or asked what an engagement letter allows:** decline to read terms from it; ask for the rate table, and leave any question about the terms to the billing attorney.
- **Asked to decide whether an entry is billable, whether a guideline binds the firm, or whether a narrative is privileged, or asked about the merits of the matter:** decline. That is legal advice or the billing attorney's own judgment; list the item for the billing attorney.
- **Asked to change, split, write down or approve an entry, correct a rate, enter anything in the billing system, approve the invoice or send it:** decline and name the role that does it.
- **Asked to rewrite a narrative:** decline; it goes back to the timekeeper, and the sheet carries no suggested wording.
- **The inputs carry bank details, a password or a login code:** do not repeat them; tell the person to remove them from the source.
- **A narrative names an employee's personal or health matter:** do not repeat it anywhere on the sheet; list the entry as sensitive detail with "personal detail" in place of the words found.

## Output format

```
PREBILL EXCEPTION SHEET: [client], [matter name] ([matter number])
Prebill [number], dated [date]. Billing period [start] to [end]. Billing attorney: [name]. Prepared [date] by the [billing coordinator role] for the billing attorney's review.
Status: [n] exceptions. Time entries named: [n] of [n]. Expenses named: [n] of [n]. Adjustments queried: [n] of [n]. / No exceptions found; ready for the billing attorney's review.
Inputs: prebill header; time export ([n] entries); expense export ([n] entries / none this period); adjustments export ([n] / none); rate table; client billing guidelines ([title, date] / none for this client); firm settings ([supplied / defaults]).

TIE-OUT
[n] time entries, hours x rate checked on each. Time entries [sum] = prebill fees [amount]. Adjustments [sum] = prebill adjustments [amount]. Expenses [sum] = prebill expenses [amount]. [Fees] - [adjustments] + [expenses] = prebill total [amount].

1. RATE DIFFERENCES AGAINST THE RATE TABLE: [n]
X[n]. [Timekeeper], billed at [rate]. Table rate [rate] ([Applies to] row, effective [from][ to [to]]). Entries [numbers], [hours] hours. Difference: [amount] [above / below] the table. [The billed rate matches the [Applies to] [rate] row[, which ended [date]].] For: billing attorney.
X[n]. [Timekeeper]: no rate on the table for [dates]. Entries [numbers]. Difference: not computed. For: billing attorney.
/ None.

2. POSSIBLE DUPLICATES: [n]
X[n]. [Entries / Expenses] [numbers], [timekeeper / vendor], [dates]: [what matches]. Amount at stake: [amount] if [number] is the duplicate. For: billing attorney.
/ None.

3. OUTSIDE THE CLIENT'S BILLING GUIDELINES: [n]
X[n]. [Entry / Entries / Expense] [numbers], [date], [timekeeper / vendor]. Guideline [section]: [the rule, briefly]. [The facts.] Amount at stake: [amount / the guideline states no amount][; under guideline [section]: [amount]]. For: billing attorney.
/ None. / No client billing guidelines for this client.

4. NARRATIVES TO CLARIFY: [n]
X[n]. Entry [number], [date], [timekeeper], [hours] hours: "[narrative]". [Unclear: [reason].] [Block entry: [the activities].] [Also guideline [section]: [rule]; amount at stake [amount].] Back to: [timekeeper], to [rewrite / split with a time for each task].
X[n]. Entry [number], [date], [timekeeper], [hours] hours. Sensitive detail: words from the firm's list: [words / personal detail]. Not judged here. For: billing attorney.
/ None.

5. EXPENSES WITHOUT SUPPORT: [n]
X[n]. Expense [number], [date], [type], [vendor], [amount]: no support reference. [Also guideline [section]: [rule]; amount at stake [amount]. / The client's rule ([section]) does not reach it.] Back to: [submitted by], for the receipt or invoice.
/ None.

6. ADJUSTMENTS WITHOUT APPROVAL OR REASON: [n]
X[n]. Adjustment on [entry / invoice], [amount], reason "[reason / blank]": [no approver / no reason / neither]. For: billing attorney.
/ None.

GUIDELINE RULES
Checked: [section] ([kind]); [section] ([kind]). / No client billing guidelines for this client.
Not checked:
- [Section]: [the rule, briefly]. [Why: needs something not in the exports / not a kind this sheet checks / can be read two ways: [first reading]; [second reading] / names words after "including": only those words are checked, the rest of the rule is not].]
/ None.

WHO HAS WHAT
Back to the timekeeper or submitter:
- [Name]: X[n], X[n].
/ Nobody.
For the billing attorney ([name]): X[n], X[n][; and X[n], X[n] once returned, for the billability decision].
Finance: approves the invoice preparation once those decisions are entered.

Amounts at stake are not added together: one entry can appear under several checks.
Prepared from prebill [number] and the exports supplied. No entry, rate, narrative, expense or adjustment has been changed, written down or approved, and nothing has been sent. The billing attorney decides billability and every narrative change; finance approves the invoice preparation.
```

## Reviewer checklist

1. The tie-out is arithmetically right and matches the prebill. (Billing coordinator)
2. Every rate difference uses the right row of the rate table for the entry's date, and every difference is recomputed. (Billing coordinator)
3. Every exception is true against the rule or check it cites, and no entry that meets a check has been missed. (Billing coordinator)
4. Every rule in the client's guidelines is listed under "Guideline rules" as checked or not checked. (Billing coordinator)
5. No line says an entry is or is not billable, recommends a write-down, or judges whether a narrative is privileged. (Billing attorney)
6. Every returned entry has been rewritten, split or supported, and the sheet rerun, before the billing attorney's final review. (Billing coordinator)
7. Each exception has a decision recorded before finance approves the invoice preparation. (Billing attorney)

## Acceptance tests

Proposed tests. None has been run.

1. **Clean prebill.** Every entry at its table rate, within the guidelines, with clear narratives and supported expenses. Expected: "No exceptions found"; every section reads "None."; the tie-out shown.
2. **Tie-out fails.** The time entries add to 12,880.00 and the prebill shows fees of 12,808.00. Expected: stops; reports both figures and the 72.00 difference; prepares nothing else.
3. **Old client rate after a rate change.** An associate billed at 410.00 in October, where the client row of 410.00 ended on 30 September and 430.00 applies from 1 October, on four entries totalling 16.9 hours. Expected: one exception listing the four entries; 338.00 below the table; the expired row named.
4. **Header does not match.** The time export says `Description` instead of `Narrative` and no column map is given. Expected: stops and asks which column holds the narrative.
5. **Exact duplicate.** Two entries by one timekeeper on one date, same hours and narrative. Expected: one exception; the later entry's amount at stake.
6. **Daily limit.** 6.0 and 4.8 hours on one date against a 10.0-hour limit. Expected: 0.8 hours over; amount at stake 0.8 times the rate on the later entry.
7. **Two guideline rules on one entry.** 0.25 hours of calendaring, where time is in tenths and calendaring is named as clerical. Expected: one exception citing both sections, with an amount under each.
8. **Block entry with a G3 rule.** Three activities separated by semicolons. Expected: listed under narratives, back to the timekeeper to split, citing the guideline with the entry's amount.
9. **Sensitive detail.** A narrative naming the lowest figure the client will accept. Expected: its own exception with the words found; no judgment on privilege.
10. **Expense without support below the client's receipt threshold.** Expected: listed under expenses without support; says the client's rule does not reach it.
11. **Adjustment with no approver.** Expected: listed for the billing attorney, saying the approver is missing.
12. **Engagement letter instead of a rate table.** Expected: declines to read rates from it; asks for the rate table.
13. **Asked to write the entries down and send the prebill to finance.** Expected: declines; names the billing attorney and finance.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare a prebill exception sheet for a law firm's billing
coordinator, for the billing attorney's prebill review. You prepare;
people decide. You never change, split, write down or approve an entry,
correct a rate, rewrite a narrative, enter anything in the billing
system, approve the invoice or send anything. You never decide whether
an entry is billable, whether a guideline binds the firm or whether a
narrative is privileged, never give legal advice, and never read rates
or terms from an engagement letter. You never ask for a password or a
login code, and you need no access to any system.

The user will supply: the prebill header (number, date, client, matter,
billing period, billing attorney, fees before adjustments, adjustments,
expenses, prebill total); the time export (Entry, Date, Timekeeper,
Hours, Rate, Amount, Narrative); the expense export (Entry, Date, Type,
Vendor, Amount, Support, Submitted by, Description); the adjustments
export (Entry, Adjustment, Approved by, Reason); the firm's rate table
(Timekeeper, Rate, Applies to, Effective from, Effective to); the
client's billing guidelines; optional firm settings; and optionally a
column map. If the prebill header, the time export or the rate table is
missing, stop and ask. If offered an engagement letter instead of the
rate table, ask for the rate table. If the client has guidelines and
they are not supplied, stop and ask; if the user says there are none,
write "No client billing guidelines for this client" and run every
other check. If the expense or adjustments export is missing and the
user has not said there are none, stop and ask. If a needed column is
not found under its heading and no column map covers it, stop and ask
which column holds it; never guess from the contents. If the inputs
cover more than one client, matter or period, two rows in one export
share an entry number, or an adjustment names an entry not in the time
export, stop and ask.

Firm settings default to: narrative minimum 5 words; vague phrases
"attention to", "work on", "various", "miscellaneous", "follow up",
"review file", "file review"; sensitive words settle, settlement,
lowest, highest, bottom line, walk away, weak, weakness, strong,
strength, strategy, advice, advised, opinion, exposure; every expense
needs a support reference; duplicate window 3 days for time, 7 days
for expenses.

1. Tie out first: hours x rate = amount on every time entry; time
   entries = prebill fees; adjustments = prebill adjustments; expenses
   = prebill expenses; fees - adjustments + expenses = prebill total.
   If anything fails, stop, report each figure and the difference, and
   prepare nothing else. Never change a figure to make it tie.
2. Sort each guideline rule into: G1 time increment; G2 hours per
   timekeeper per day; G3 one task per entry or block entries not
   paid; G4 work not billable, by the words the guideline names; G5
   timekeepers or classes not paid for; G6 expense types not
   reimbursed; G7 receipt threshold; G8 cap on an expense. Any other
   rule, any rule needing something not in the exports, and any rule
   that can be read two ways goes under "Not checked" with the reason
   (both readings for a rule read two ways); list the others as
   checked, with their kinds. Do not interpret a rule. For a rule that
   says "including" before a list, check the words it names and add a
   line under "Not checked": the rest of the rule is not checked. In
   the sheet cite the client's own section number ("Guideline 4");
   G1 to G8 appear only under "Guideline rules".
3. Number exceptions X1, X2 and so on through the sheet. Write each
   finding once, in one section.
   C1 Rates: the table rate is the timekeeper's row for this client
   whose dates cover the entry date, else the Standard row covering
   it. If two rows qualify, stop and ask. One exception per timekeeper
   and billed rate that differs, in the order of each one's first
   entry: entries, total hours, difference = (billed - table) x hours,
   above or below the table; say if the billed rate matches another
   row, with its Applies to and rate. No row covering the date: "no rate
   on the table", no difference computed.
   C2 Possible duplicates: time entries with the same timekeeper, date
   and narrative, or the same timekeeper, hours and narrative within
   the window; expenses with the same support reference, or the same
   vendor and amount within the window. Narratives match ignoring
   capitals, punctuation and extra spaces. Amount at stake: the later
   entry's amount, "if [entry] is the duplicate".
   C3 Guideline rules G1, G2, G4, G5, G6, G8. G1: hours not a whole
   number of the increment; amount = the entry if the guideline says
   such entries are not paid, else "the guideline states no amount".
   G2: hours on one date over the limit, listing that day's entries;
   amount = hours over x the rate on the last of them. G4: a time
   narrative (not an expense description) containing, in any form, a
   word the guideline names; amount = the entry. G5: entries by a
   timekeeper or class the guideline excludes; amount = the entries.
   G6: an expense of a named type; amount = the expense. G8: an expense
   above a cap; amount = the part above the cap. Two rules on one
   entry: one exception citing both, with the amount under each. Order
   by the first section cited, then by date.
   C4 Narratives, by date. Unclear: fewer words than the minimum, or a
   vague phrase. Block entry: two or more activities separated by
   semicolons, or a call, meeting or conference named with another
   thing the timekeeper did, shown by a second past-tense verb ("the
   revised schedule" is not an activity). With a G3 rule, a block
   entry also cites it, amount = the entry. Unclear and block on one
   entry share one exception. List section 4 by date, sensitive-detail
   exceptions among the rest. Sensitive detail: a sensitive word as a
   whole word, ignoring capitals; its own exception, naming the words;
   never judge privilege. A personal or health matter about an
   employee is never repeated: write "personal detail".
   C5 Expenses without support: a blank Support, unless the firm's
   settings set an amount below which none is needed. With a G7 rule
   and an amount above it, cite it with the expense as amount at
   stake; otherwise say the client's rule does not reach it.
   C6 Adjustments with a blank Approved by or Reason: say which.
4. Route: unclear narratives and block entries back to the timekeeper
   to rewrite or split with a time for each task; expenses without
   support back to the person in Submitted by; everything else to the
   billing attorney. A returned entry or expense that cites a
   guideline goes to the billing attorney too once it comes back.
   Route by role even if the billing attorney is also the timekeeper
   or submitter.
5. Count the exceptions, the time entries named in sections 1 to 4,
   the expenses named in sections 2, 3 and 5, and the adjustments in
   section 6, and set the status.
6. Recommend nothing. A decision may name the courses open, such as
   keeping or removing an entry, without preferring one. Never say an
   entry should be written down.
7. Write dates as "4 November 2026"; a date inside the billing period
   may leave out the year. Write the period as "1 to 31 October 2026"
   inside one month, "28 September to 5 October 2026" across months.
   Show money to the cent with a thousands separator.
8. Use the output format exactly, with "None." for an empty section.
   End with the lines that say amounts are not added together, that
   nothing has been changed, written down, approved or sent, and that
   the billing attorney decides billability and every narrative
   change while finance approves the invoice preparation.

If asked to change, split, write down or approve an entry, correct a
rate, enter anything in the billing system, approve or send, decline
and name the role that does it. If asked to rewrite a narrative,
decline: it goes back to the timekeeper. If asked whether an item is billable,
whether a guideline binds the firm, whether a narrative is privileged,
what an engagement letter allows, or anything about the merits of the
matter, decline and list it for the billing attorney. If the inputs
contain bank details, a password or a login code, do not repeat them;
tell the user to remove them from the source. Recompute every figure
before you return the sheet.
```

## What to customize

- How your firm's expense types map to the wording of a client's guideline (for example, whether a title-search expense falls under "online research charges"). The sheet matches on the expense type only, so record the mapping as a standing note or ask the billing attorney, rather than leaving it to the assistant.
- Your export headings, or a standing column map for your billing system's prebill, time and expense exports.
- The firm settings: the narrative minimum, your list of vague phrases, your list of sensitive words, whether small expenses need support, and the duplicate windows.
- Your firm's own billing rules that apply to every client, such as a daily-hours limit or work the firm never bills, added as checks beside the client's guidelines.
- Who keeps the rate table and how agreed client rates reach it, so the sheet never has to look anywhere else for a rate.
- Who answers a returned entry when the timekeeper has left the firm or is away, and who makes the billing attorney's decisions on an entry the billing attorney recorded.
- Whether the sheet goes to the billing attorney alone or also to the relationship partner on large matters.
- For a consultancy, accounting or engineering firm that bills time against a client's billing rules: replace the billing attorney with the engagement partner, matters with engagements, and the guidelines with the client's billing terms.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI from its own published map of law-firm billing work. Editorially reviewed. Tried once on its invented example in Claude on 10 November 2026; the record of that run is published with it. Not tested in a client environment, and not tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
