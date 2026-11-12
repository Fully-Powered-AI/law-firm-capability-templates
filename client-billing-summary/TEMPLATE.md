# Client billing summary

Workflow template, version 0.1.0.

## Purpose

Prepare, from one matter's pre-bill, the summary that goes to the client with the invoice: fees by timekeeper, by task and by phase, the expenses, and the write-downs and discounts already decided, all tied to the pre-bill's totals. Alongside it, prepare a review for the responsible attorney alone: every entry that breaks the client's billing guidelines, with the guideline, the facts and the amount affected, and every time entry description that may say more than an invoice should. The assistant prepares; it never writes down an entry, changes the pre-bill or the billing system, decides what is privileged, approves the summary or sends it.

## When to use it and when not to

Use it once the pre-bill for a matter is generated for the billing period and before the responsible attorney's pre-bill review, so the attorney reviews the flags and the client summary together. Run it again after the attorney's decisions have been entered in the billing system, from the updated pre-bill.

Do not use it:

- to chase an invoice that is already overdue. That is a separate piece of work, done after the invoice is sent;
- to set up a matter's billing terms. Those are captured when the matter is opened;
- to decide whether an entry should be written off, whether a guideline binds the firm, or whether the firm may bill something under its engagement terms. Those are the responsible attorney's decisions;
- to give legal advice, assess the matter, or say what is or is not privileged;
- for a matter billed on a fixed fee with no time detail, where there is nothing to summarize by timekeeper or task.

## Roles

- **Runs it:** the billing coordinator.
- **Decides every flag, rewords or approves each flagged description, and approves the client summary:** the responsible attorney.
- **Enters the attorney's decisions in the billing system and reruns it:** the billing coordinator.
- **Changes a time entry's description:** the timekeeper who recorded it, or the billing coordinator at the attorney's direction.
- **Sends the invoice and the summary to the client, or uploads them to the client's billing portal:** [the role your firm names], after the attorney approves.

## Inputs

1. **The pre-bill:** the draft invoice from the billing system, with its number and date, the client, the matter, the billing period, and its four totals: fees, write-downs and discounts, expenses, and the invoice total. If missing, stop.
2. **Time export:** every time entry on the pre-bill, one row each. Default column headers: `Entry`, `Date`, `Timekeeper`, `Role`, `Task`, `Phase`, `Hours`, `Rate`, `Amount`, `Description`. `Amount` is the entry's value before any write-down. `Task` and `Phase` may be blank. If missing, stop.
3. **Expense export:** every expense on the pre-bill. Default column headers: `Entry`, `Date`, `Category`, `Vendor`, `Description`, `Amount`, `Receipt` (yes or no). If the period has no expenses, the person says so. If the export is missing and the person has not said there are none, stop.
4. **Adjustments export:** the write-downs and discounts already decided and entered on the pre-bill. Default column headers: `Entry` (a time entry number, or `invoice`), `Type` (write-down or discount), `Amount`, `Approved by`, `Note for client`. If there are none, the person says so. Adjustments reduce fees. If one names an expense entry, stop and ask how it is to be shown.
5. **The client's billing guidelines:** the client's billing rules for outside firms, or the billing terms of the engagement, with their title and date. If the person says the client has none, write "No client billing guidelines" and run only the firm's own checks in step 4. If the client has guidelines and they are not supplied, stop.
6. **Matter settings:** the client's name, the matter's name and number, the responsible attorney, the date the summary is prepared, and the fees billed on the matter before this invoice. The last is needed only for a budget check; if missing, write "billed to date not supplied" on the budget line.
7. **A column map** (optional), when the exports use other headings: which of their columns holds each default column.

**When a header does not match.** If a column the work needs is not found under its default heading and no column map covers it, stop and ask which column holds it. Never guess a column from its contents.

The work runs on exports and documents the person supplies. It needs no connection to the billing system or the client's portal and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Confirm one client, one matter and one billing period across the pre-bill and the exports. Check every column the work needs, as above. If two rows share an entry number, stop and ask.
2. **Tie out before anything else.** For each time entry, hours times rate must equal its amount to the cent. The time entries must add to the pre-bill's fees, the expenses to its expenses, and the adjustments to its write-downs and discounts. Fees less write-downs and discounts, plus expenses, must equal the pre-bill's invoice total. If any of these fails, stop: report each figure and the difference to the billing coordinator and draft nothing else.
3. **Read the guidelines.** List each rule that can be checked from the exports, with its section number. List every rule that cannot, such as notice of a rate change or an approval held somewhere else, under "Not checkable from the inputs". Do not interpret a rule. If one can be read two ways, put it under "Other questions" and do not check it.
4. **Run the checks.** Each finding is one flag, numbered in the order below.
   - **Rates and timekeepers:** each timekeeper's billed rate against the rate the guidelines approve for them or their role; any timekeeper the guidelines do not approve. One flag per timekeeper and rate, listing every entry at that rate. Amount affected: the difference in rate times the hours, or the entries' total for a timekeeper who is not approved.
   - **Codes:** where the guidelines require task or phase codes, any entry with a blank code or a code not on the client's list.
   - **Time recording:** entries not in the increment the guidelines set; any timekeeper whose hours on one day pass the daily limit the guidelines set. Amount affected: the hours over the limit times the rate.
   - **Several activities under one time,** where the guidelines bar it: a description that names two or more separate activities, each with its own verb, under a single time. Amount affected: the entry's amount.
   - **Internal conferences,** where the guidelines allow one attendee only: entries by two or more firm timekeepers on the same date for the same conference. List every attendee's entry and amount. Amount affected: for each entry that could stay, the total of the others, written as "[amount] if entry [number] stays" for each.
   - **Administrative work,** where the guidelines name work that is not billable: an entry whose description is that work. Amount affected: the entry's amount.
   - **Expenses:** an expense in a category the guidelines do not reimburse; an expense above the guidelines' receipt threshold with `Receipt` set to no; an expense above any cap. Amount affected: the expense, or the amount above the cap.
   - **Budget:** where the guidelines set one and the fees billed to date are supplied, billed to date plus this invoice's net fees against the budget. Always show the budget line; flag only if the total passes the budget. Where the budget covers only a stage or a period, such as fees through the end of document production, say so on the budget line, and compare only if the fees billed to date and this invoice's fees fall within that same stage or period; if they may not, do not compare, and put the budget under "Other questions".
   - **The firm's own checks,** whatever the guidelines say: two entries with the same timekeeper, date, hours and description; an adjustment with no approver; a blank task code where the guidelines do not require one. These go under "Other questions", not flags.
   Where two rules reach the same entry or expense, write one flag that cites both sections, with the amount affected under each, and count it once.
   Write each flag with the entry, date, timekeeper or vendor, the guideline section, the facts, the amount affected, and the question for the responsible attorney. The question may name the courses open to the attorney, such as keeping or taking off an entry, without preferring one. Recommend nothing and never say an entry should be written off.
5. **Find descriptions to reword.** A time entry's description may print on the invoice's itemized detail, and invoices travel beyond the client's lawyers, to accounts payable, auditors and insurers. List every description that names advice given or asked for, a view of the strengths or weaknesses of a position, the firm's plan for how the matter will be argued or resolved, a settlement position or figure, or someone's opinion of the case. Ordinary work plans, such as a document production plan or a filing schedule, are not listed. Say what kind of detail it carries; do not decide whether it is privileged. The responsible attorney decides.
6. **Build the client summary from the pre-bill as it stands,** before any decision on the flags.
   - **Overview:** two to four sentences on what the work covered in the period, phase by phase in date order, then the totals line.
   - **By timekeeper:** one line per timekeeper and rate, with hours, fees and a short note on the work, taken from their descriptions. A timekeeper billed at two rates gets two lines.
   - **By task:** one line per code in the `Task` column, named as in the guidelines' list of codes, or shown as the code alone if the guidelines give no name, with hours, fees and one or two sentences on what the work was and what it was for. Never sort entries into tasks yourself. Entries with a blank code go on a line marked "Not coded". If the whole column is blank, write "No task codes recorded in the time export."
   - **By phase:** one line per code in the `Phase` column, named the same way, with the dates of its first and last time entry, hours, fees and the main work. Same rule for blanks: "Not coded", or "No phases recorded in the time export."
   - **Expenses:** each expense, then a subtotal for each category and the total.
   - **Write-downs and discounts:** each adjustment with its amount and the `Note for client`. Where the note is blank, show the type and amount only; never copy an internal reason.
   The timekeeper, task and phase views show fees before write-downs; write-downs appear once, in their own section.
   Write each date as the day, the month's name and the year: "4 November 2026". In a range, do not repeat a month or year both ends share: "1 to 31 October 2026", "28 September to 3 October 2026". A date inside the billing period, in a phase, expense or flag line, may leave out the year: "1 to 7 October".
7. **Write every narrative from the time and expense entries only.** Name the records, documents and parties the work involved. Describe an entry listed in step 5 only by the kind of work and the party, "on the matter": for example, "a further call with the client on the matter". Add no fact that no entry states, and no view of the matter's merits or prospects.
8. **Set the status.** If any flag, description to reword or other question is open: "Not ready to send", with each count. Otherwise: "No flags open; ready for the responsible attorney's approval."
9. **Return the draft** to the billing coordinator for the responsible attorney. Nothing goes to the client until the attorney approves the client summary. After the attorney decides, the billing coordinator enters the decisions in the billing system and runs this again from the updated pre-bill.

## Exceptions and stop conditions

- **The tie-out fails:** stop and report the figures and the difference. Never adjust a figure to make it tie.
- **A header does not match and no column map covers it:** stop and ask.
- **The client has guidelines that were not supplied:** stop and ask for them.
- **Two rows share an entry number, or an adjustment names an expense:** stop and ask.
- **Asked to write down or change an entry, change the pre-bill or the billing system, approve the summary, send it or upload it to a client portal:** decline and name the role that does it.
- **Asked to say whether something is privileged, whether a guideline binds the firm, whether the firm may bill an item, or anything about the merits of the matter:** decline. That is legal advice or the attorney's own judgment; list the item for the responsible attorney.
- **Asked to reword a flagged description:** only if the responsible attorney asks, suggest neutral wording in the review. The timekeeper or the billing coordinator changes the entry.
- **A guideline can be read two ways:** do not check it; put it under "Other questions" with the section and the two readings.
- **The inputs carry bank details, a password or a login code:** do not repeat them; tell the person to remove them from the source.
- **A description names an employee's personal or health matter:** do not repeat it anywhere; list the entry under descriptions to reword as "personal detail".

## Output format

```
CLIENT BILLING SUMMARY: [client], [matter name] ([matter number])
Billing period [start] to [end]. Pre-bill [number], dated [date]. Prepared [date] for [responsible attorney].
Status: DRAFT. Not ready to send: [n] guideline flags, [n] descriptions to reword, [n] other questions open. / DRAFT. No flags open; ready for the responsible attorney's approval.
Inputs not supplied: [list / none].

PART A: FOR THE CLIENT, ONCE THE RESPONSIBLE ATTORNEY APPROVES

1. Matter
Client: [name]. Matter: [name and number]. Billing period: [start] to [end]. Responsible attorney: [name]. Billing guidelines: [title, date / No client billing guidelines].

2. Overview
[Two to four sentences: the work of the period, phase by phase in date order.]
Fees [amount]. Write-downs and discounts -[amount]. Net fees [amount]. Expenses [amount]. Total for this invoice [amount].

3. By timekeeper
- [Timekeeper], [role]: [hours] hours at [rate] = [fees]. [Short note on the work.]
Total: [hours] hours, [fees].

4. By task
- [Code and name]: [hours] hours, [fees]. [One or two sentences on what the work was and what it was for.]
- Not coded: [hours] hours, [fees]. [Note.]
/ No task codes recorded in the time export.

5. By phase
- [Code and name], [first date] to [last date]: [hours] hours, [fees]. [Main work.]
/ No phases recorded in the time export.

6. Expenses
- [Date], [category], [vendor]: [description], [amount].
Subtotals: [category] [amount]; [category] [amount]. Total expenses [amount].
/ No expenses this period.

7. Write-downs and discounts
- [Entry number / Invoice], [type]: -[amount]. [Note for client / nothing].
/ None.

Fees in sections 3 to 5 are shown before write-downs.

PART B: FOR THE RESPONSIBLE ATTORNEY ONLY. NEVER SENT TO THE CLIENT.

Tie-out: [n] time entries, hours times rate checked on each. Time entries [sum] = pre-bill fees [amount]. Adjustments [sum] = pre-bill write-downs and discounts [amount]. Expenses [sum] = pre-bill expenses [amount]. [Fees] - [adjustments] + [expenses] = pre-bill total [amount].

Checks run against [guidelines title and date]: [section, rule; section, rule]. The firm's own: arithmetic, duplicate entries, adjustments with an approver.
Not checkable from the inputs: [section, rule / none].
Budget: [billed to date] billed to date + [net fees] net fees this invoice = [total] of [budget] ([section][, which covers stage or period]); [amount] remains / over by [amount]. / No budget in the guidelines. / Billed to date not supplied. / [Budget] ([section]) covers [stage or period]; not compared, see Other questions.

Guideline flags: [n]
[n]. [Entry numbers / expense], [date], [timekeeper / vendor]. Guideline [section]: [the rule, briefly]. [The facts.] Amount affected: [amount]. Decision: [the question].
/ None.

Descriptions to reword before the itemized detail prints: [n]
- Entry [number], [date], [timekeeper]: [kind of detail]. Decision: reword, or approve as recorded.
/ None.

Other questions: [n]
- [Duplicate entry / adjustment with no approver / blank task code / guideline read two ways / budget scope]: [facts]. For: [role].
/ None.

Prepared from pre-bill [number] and the exports supplied. Nothing has been written down, changed, approved or sent. [Responsible attorney] decides every flag and approves Part A before anyone sends it.
```

## Reviewer checklist

1. The tie-out is arithmetically right and matches the pre-bill. (Billing coordinator)
2. Every figure in Part A traces to the exports, and sections 3, 4 and 5 each add to the fees. (Billing coordinator)
3. Every flag is true against the guideline section it cites, and none has been missed for a rule listed as checked. (Billing coordinator)
4. Every rule the guidelines contain is either listed as checked or as not checkable. (Billing coordinator)
5. No sentence in Part A states advice, a view of the matter, the firm's plan for arguing or resolving it, or a settlement position, and every description that does is listed for rewording. (Responsible attorney)
6. Part A says nothing that no entry states, and carries no internal reason for a write-down. (Responsible attorney)
7. Each flag has a decision recorded before the summary is sent. (Responsible attorney)
8. Part B is removed before anything goes to the client. (Billing coordinator)

## Acceptance tests

Proposed tests. None has been run.

1. **Clean pre-bill.** All entries within the guidelines. Expected: no flags; status "ready for the responsible attorney's approval"; every section filled.
2. **Tie-out fails.** The time entries add to $13,136.00 and the pre-bill shows fees of $13,316.00. Expected: stops; reports both figures and the $180.00 difference; drafts nothing else.
3. **Rate above the approved rate.** An associate approved at $380 billed at $400 on three entries totalling 11.5 hours. Expected: one flag listing the three entries; amount affected $230.00; no write-down suggested.
4. **Header does not match.** The time export says `Narrative` instead of `Description` and no column map is given. Expected: stops and asks which column holds the description.
5. **Several activities under one time.** "Reviewed first production set; call with client on custodians; revised chronology", 3.5 hours, where the guidelines bar it. Expected: flagged with the entry's amount.
6. **Both attendees bill an internal conference** where the guidelines allow one. Expected: one flag listing both entries and amounts; the amount affected given for each entry that could stay; the question asks which stays.
7. **Description carries a settlement position.** Expected: listed under descriptions to reword by kind of detail; Part A describes the entry only as a call with the client on the matter.
8. **Expense over the receipt threshold with no receipt.** Expected: flagged with the guideline section and the amount.
9. **No task codes at all.** Expected: "No task codes recorded in the time export."; no categories made up; an "Other questions" line if the guidelines do not require codes, a flag if they do.
10. **Client has no guidelines.** Expected: "No client billing guidelines" in the header; only the firm's own checks run; no guideline flags.
11. **Asked to write off the flagged entries and send the summary.** Expected: declines; names the responsible attorney for the decision and the role that sends.
12. **Asked whether an entry is privileged.** Expected: declines to decide; lists it for the responsible attorney.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare a client billing summary from one matter's pre-bill for a
law firm's billing coordinator, with a review for the responsible
attorney. You prepare; people decide. You never write down or change an
entry, change the pre-bill or the billing system, approve the summary,
send it or upload it anywhere. You never decide what is privileged, give
legal advice, or say anything about the merits of the matter.
You never ask for a password or a login code, and you need no access to
any system.

The user will supply: the pre-bill and its totals; the time export
(Entry, Date, Timekeeper, Role, Task, Phase, Hours, Rate, Amount,
Description); the expense export (Entry, Date, Category, Vendor,
Description, Amount, Receipt); the adjustments export (Entry, Type,
Amount, Approved by, Note for client); the client's billing guidelines;
the matter settings, including fees billed to date; and optionally a
column map. If the pre-bill or the time export is missing, stop and
ask. If the client has billing guidelines and they are not supplied,
stop and ask. If the user says the client has none, write "No client
billing guidelines", raise no guideline flags, and run only the firm's
own checks in step 4. If the expense or adjustments export is missing
and the user has not said there are none, stop and ask. Confirm that
the pre-bill and every export are for one client, one matter and one
billing period; if not, stop and ask. If a needed column is not found
under its heading and no column map covers it, stop and ask which
column holds it; never guess from the contents. If two rows share an
entry number, or an adjustment names an expense, stop and ask.

1. Tie out first: hours x rate = amount on every time entry; time
   entries = pre-bill fees; adjustments = pre-bill write-downs and
   discounts; expenses = pre-bill expenses; fees - adjustments +
   expenses = pre-bill total. If anything fails, stop, report each
   figure and the difference, and draft nothing else. Never adjust a
   figure to make it tie.
2. List each guideline rule you can check from the exports, with its
   section, and each rule you cannot under "Not checkable from the
   inputs". If a rule can be read two ways, do not check it; put it
   under "Other questions" with the section and the two readings.
3. Flag, in this order, with the amount affected for each:
   - billed rates above the approved rate, and timekeepers not
     approved: one flag per timekeeper and rate, listing every entry;
     amount = rate difference x hours, or the entries' total for a
     timekeeper not approved;
   - blank or unknown codes where codes are required;
   - time not in the set increment, and hours over the daily limit:
     amount = hours over the limit x rate;
   - one time for two or more separate activities, each with its own
     verb, where barred: amount = the entry's amount;
   - an internal conference billed by more than one attendee, where
     barred: list every attendee's entry and amount; amount = for each
     entry that could stay, the total of the others, written as
     "[amount] if entry [number] stays" for each;
   - work the guidelines call non-billable: amount = the entry's
     amount;
   - expenses not reimbursed, over the receipt threshold without a
     receipt, or over a cap: amount = the expense, or the amount above
     the cap;
   - billed to date plus net fees over the budget.
   Where the budget covers only a stage or a period, say so on the
   budget line, and compare only if the fees billed to date and this
   invoice's fees fall within that same stage or period; if they may
   not, do not compare, and put the budget under "Other questions".
   Where two rules reach the same entry or expense, write one flag
   citing both sections, with the amount affected under each, and
   count it once. Each flag gives the entries, date, timekeeper or
   vendor, section, facts, amount affected and a question for the
   responsible attorney. The question may name the courses open, such
   as keeping or taking off an entry, without preferring one.
   Recommend nothing.
4. Whatever the guidelines say, list under "Other questions": duplicate
   entries (same timekeeper, date, hours and description), adjustments
   with no approver, and blank task codes the guidelines do not require.
5. List under "Descriptions to reword" every description that names
   advice given or asked for, a view of the strengths or weaknesses of
   a position, the firm's plan for how the matter will be argued or
   resolved, a settlement position or figure, or someone's opinion of
   the case, saying only what kind of detail it carries. Ordinary work
   plans, such as a document production plan or a filing schedule, are
   not listed. A description naming an employee's personal or health
   matter is listed as "personal detail" and never repeated.
6. Build Part A from the pre-bill as it stands. The overview is two to
   four sentences on the work of the period, phase by phase in date
   order, then the totals line. Timekeeper, task and phase views show
   fees before write-downs; write-downs appear once.
   One line per timekeeper and rate. Task and phase lines come only
   from the Task and Phase columns; never sort entries yourself; blanks
   go on a "Not coded" line. Name each code as in the guidelines' list
   of codes; if the guidelines give no name, show the code alone. Show
   a write-down's "Note for client", or its type and amount only; never
   an internal reason.
7. Write every narrative from the time and expense entries only,
   naming the records, documents and parties involved. Describe an
   entry listed in step 5 only as the kind of work and the party "on
   the matter". Add no fact no entry states and no view of the matter.
8. Write each date as the day, the month's name and the year: "4
   November 2026". In a range, do not repeat a month or year both ends
   share: "1 to 31 October 2026", "28 September to 3 October 2026". A
   date inside the billing period, in a phase, expense or flag line,
   may leave out the year: "1 to 7 October".
9. Set the status: "Not ready to send" with each count if anything is
   open; otherwise "No flags open; ready for the responsible
   attorney's approval".
10. Use the output format exactly, with the empty-section wording it
    gives. End with the line that says nothing has been written down,
    changed, approved or sent, and that the responsible attorney
    decides every flag and approves Part A before anyone sends it.

If asked to write down or change an entry, approve, send or upload,
decline and name the role that does it. If asked whether something is
privileged, whether a guideline binds the firm, whether an item may be
billed, or anything about the merits of the matter, decline and list it
for the responsible attorney. Suggest neutral wording for a flagged
description only if the responsible attorney asks. If the inputs
contain bank details, a password or a login code, do not repeat them;
tell the user to remove them from the source. Recompute every total
before you return the draft.
```

## What to customize

- Your export headings, or a standing column map for your billing system's pre-bill and time exports.
- Who sends the invoice and the summary, and whether it goes by email or through the client's billing portal.
- Whether the client summary goes to every client or only to clients whose guidelines ask for one.
- The firm's own checks to run on every matter, such as a daily-hours limit or a list of administrative tasks the firm never bills, even where a client's guidelines are silent.
- The wording your firm uses in place of "on the matter" for entries whose descriptions are listed for rewording.
- Whether a flagged description is reworded by the timekeeper or by the billing coordinator.
- For a consultancy or accounting firm that bills time against a client's billing rules: replace the responsible attorney with the engagement partner, matters with engagements, and the guidelines with the client's billing terms.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI, drawing on a published billing summary method credited in the sources. Editorially reviewed. Tried on its invented example on 10 November 2026 in four runs: the instructions were revised after each of the first three, and the fourth is the run recorded; it did not reach any stop condition. After the recorded run only the example's output was edited, to match it; the instructions, the output format and the example's inputs were not changed. The trial record lists the changes. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
