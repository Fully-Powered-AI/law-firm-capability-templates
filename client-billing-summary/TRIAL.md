# Client billing summary: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-10
- **Template version:** 0.1.0

This is a record of one run of the capability template on its own invented example. The firm, the client, the other party, the vendors, the entries, the guidelines and the figures are invented, and no client data was used. It shows what the template produced once, on one set of inputs. It is not a test in any firm's environment.

This is the fourth run on the same example, all on 10 November 2026. The first three showed where the instructions left room to guess; the instructions and a few lines of the example's inputs were revised after them, and the run recorded here was made on the revised instructions. What the earlier runs found, and what was changed, is at the end.

## The inputs used

The inputs are exactly those in [the worked example](example.md), under "The inputs": the matter settings (including fees billed before this invoice of $41,250.00, all for case assessment), the pre-bill totals for PB-1182, the time export of fourteen entries, the expense export of four expenses, the adjustments export of one write-down, and the billing sections of Client A's guidelines.

The run was a fresh session started from Claude Code with no tools and no access to any file. The template's instructions for an AI assistant and its output format were given as the session's instructions, and the inputs were sent as one message. The session did not see the example's own output or the earlier runs, and it did not write or revise the template.

## What came out

The complete output, as returned:

```
CLIENT BILLING SUMMARY: Client A, Dispute with Supplier B over late deliveries (24-0317)
Billing period 1 to 31 October 2026. Pre-bill PB-1182, dated 3 November 2026. Prepared 4 November 2026 for Partner A.
Status: DRAFT. Not ready to send: 6 guideline flags, 1 description to reword, 1 other question open.
Inputs not supplied: none.

PART A: FOR THE CLIENT, ONCE THE RESPONSIBLE ATTORNEY APPROVES

1. Matter
Client: Client A. Matter: Dispute with Supplier B over late deliveries, 24-0317. Billing period: 1 to 31 October 2026. Responsible attorney: Partner A. Billing guidelines: Client A Outside Counsel Billing Guidelines, version of 1 March 2026.

2. Overview
In case assessment (1 to 7 October), the firm spoke with Client A's operations director about the delivery history and the documents Client A holds. It also reviewed Supplier B's 2026 delivery records and the delivery and notice terms of the supply agreement, and built a chronology of orders, delivery dates and complaints from Client A's purchasing emails and order records. In document production (9 to 29 October), the firm prepared the document production plan and search terms, and reviewed Client A's purchasing emails for responsiveness and privilege. It also organized the matter file and document index, and Bates-numbered and reviewed the first production set before service, and spoke with the client on custodians and on the matter and with Supplier B's counsel on production dates and format.
Fees $13,136.00. Write-downs and discounts -$450.00. Net fees $12,686.00. Expenses $1,434.90. Total for this invoice $14,120.90.

3. By timekeeper
- Partner A, Partner: 3.8 hours at $650 = $2,470.00. Call with Client A's operations director on delivery history and documents, internal conference with Associate B on the document production plan, call with the client on the matter, and review of the first production set before service.
- Associate B, Senior associate: 11.8 hours at $450 = $5,310.00. Review of Supplier B's 2026 delivery records and the supply agreement's delivery and notice terms, internal conference with Partner A, the document production plan and search terms, review of the first production set with a call with the client on custodians and revision of the chronology, and a call with Supplier B's counsel on production dates and format.
- Associate C, Associate: 11.5 hours at $400 = $4,600.00. Chronology of orders, delivery dates and complaints from Client A's purchasing emails, comparison of Client A's order records with Supplier B's delivery records, and first-batch review of Client A's purchasing emails for responsiveness and privilege.
- Paralegal D, Paralegal: 3.6 hours at $210 = $756.00. Organized the matter file and document index, and Bates-numbered the first production set.
Total: 30.7 hours, $13,136.00.

4. By task
- T1 Review and analysis: 19.7 hours, $8,590.00. Review of Supplier B's delivery records, the supply agreement and Client A's purchasing emails and order records to build the chronology. Review of Client A's purchasing emails for responsiveness and privilege, and of the first production set before service.
- T2 Preparation of documents: 7.6 hours, $2,556.00. The document production plan and search terms for the email review, the matter file and document index, and Bates numbering of the first production set.
- T3 Communication with client: 1.8 hours, $1,170.00. A call with Client A's operations director on delivery history and the documents Client A holds, and a call with the client on the matter.
- T4 Communication within the firm: 1.0 hours, $550.00. An internal conference between Partner A and Associate B on the document production plan.
- T5 Communication with other parties: 0.6 hours, $270.00. A call with Supplier B's counsel on production dates and format.

5. By phase
- P1 Case assessment, 1 to 7 October: 11.7 hours, $5,240.00. Call with Client A's operations director, review of Supplier B's delivery records and the supply agreement, the chronology from Client A's purchasing emails and order records, and an internal conference on the document production plan.
- P2 Document production, 9 to 29 October: 19.0 hours, $7,896.00. Document production plan and search terms, review of the first production set and Client A's purchasing emails, file organization and indexing, Bates numbering, and calls with the client and with Supplier B's counsel.

6. Expenses
- 9 October, Document hosting, Vendor A: Hosting and processing of Client A's email collection, October, $1,150.00.
- 14 October, Meals, Café B: Lunch for the review team during document review at the firm's office, $64.50.
- 23 October, Outside printing, Vendor D: Printing of the first production set for Client A's review, $182.40.
- 30 October, Courier, Courier C: Delivery of the first production set on a drive to Supplier B's counsel, $38.00.
Subtotals: Document hosting $1,150.00; Meals $64.50; Outside printing $182.40; Courier $38.00. Total expenses $1,434.90.

7. Write-downs and discounts
- Entry 1007, write-down: -$450.00. One hour of the production plan preparation written off.

Fees in sections 3 to 5 are shown before write-downs.

PART B: FOR THE RESPONSIBLE ATTORNEY ONLY. NEVER SENT TO THE CLIENT.

Tie-out: 14 time entries, hours times rate checked on each. Time entries $13,136.00 = pre-bill fees $13,136.00. Adjustments $450.00 = pre-bill write-downs and discounts $450.00. Expenses $1,434.90 = pre-bill expenses $1,434.90. $13,136.00 - $450.00 + $1,434.90 = pre-bill total $14,120.90.

Checks run against Client A Outside Counsel Billing Guidelines, version of 1 March 2026: 2.1, approved timekeepers and hourly rates; 2.2, one task code and one phase code on every entry, from the listed codes; 2.3, time in tenths of an hour and no more than 10 hours per timekeeper per day; 2.4, one task per entry with its own time; 2.5, internal conference billed by one attendee only; 2.6, administrative and clerical work not billable; 3.2, meals during local work, copying and printing done at the firm, office supplies and overtime not reimbursed; 3.4, receipt for any single expense over $75; 4.1, fee budget through the end of document production. The firm's own: arithmetic, duplicate entries, adjustments with an approver.
Not checkable from the inputs: 2.1, whether any rate change was made on 60 days' written notice with Client A's consent in writing.
Budget: $41,250.00 billed to date + $12,686.00 net fees this invoice = $53,936.00 of $60,000.00 (4.1, which covers fees through the end of document production; fees billed to date are all P1 and this invoice's fees are P1 and P2); $6,064.00 remains.

Guideline flags: 6
1. Entries 1003, 1004 and 1011, 5, 6 and 21 October, Associate C. Guideline 2.1: Associate C's approved rate is $380. The entries are billed at $400:
   - 1003, 4.5 hours, $1,800.00
   - 1004, 2.0 hours, $800.00
   - 1011, 5.0 hours, $2,000.00

   This is 11.5 hours at $20 above the approved rate. Amount affected: $230.00. Decision: keep these entries at $400, or bill them at the approved $380?
2. Entry 1008, 14 October, Associate B. Guideline 2.4: each entry describes one task with its own time; entries putting several tasks under one time are not paid. The entry puts three activities under one time of 3.5 hours at $450:
   - review of the first production set
   - a call with the client on custodians
   - revision of the chronology

   Amount affected: $1,575.00. Decision: keep the entry as recorded, have it split into separate entries each with its own time, or take it off?
3. Entries 1005 and 1006, 7 October, Partner A and Associate B. Guideline 2.5: a conference between the firm's own timekeepers is billed by one attendee only. Both attendees billed the internal conference on the document production plan:
   - 1005, Partner A, 0.5 hours, $325.00
   - 1006, Associate B, 0.5 hours, $225.00

   Amount affected: $225.00 if entry 1005 stays; $325.00 if entry 1006 stays. Decision: which entry stays and which comes off, or are both kept?
4. Entry 1012, 22 October, Paralegal D. Guideline 2.6: administrative and clerical work, including organizing files and indexing, is not billable at any rate. "Organized the matter file and document index," 1.2 hours at $210. Amount affected: $252.00. Decision: keep the entry or take it off?
5. Expense E202, 14 October, Café B. Guideline 3.2: meals during local work are not reimbursed. Lunch for the review team during document review at the firm's office, receipt on file. Amount affected: $64.50. Decision: keep the expense or take it off?
6. Expense E204, 23 October, Vendor D. Guideline 3.4: any single expense over $75 needs a receipt. Outside printing of the first production set for Client A's review, $182.40, receipt marked "no." Amount affected: $182.40. Decision: obtain the receipt before sending, keep the expense without it, or take it off?

Descriptions to reword before the itemized detail prints: 1
- Entry 1009, 16 October, Partner A: settlement position, and a view of the weaknesses of a position. Decision: reword, or approve as recorded.

Other questions: 1
- Guideline read two ways: 2.6, entry 1010, 26 October, Paralegal D, "Bates-numbered the first production set," 2.4 hours, $504.00. One reading: Bates numbering is administrative and clerical work under 2.6 and not billable. The other reading: it is not among the examples 2.6 lists (scheduling, organizing files, indexing, copying) and is part of preparing the production. Not checked. For: responsible attorney.

No duplicate entries, no adjustments without an approver, and no blank task codes were found.

Prepared from pre-bill PB-1182 and the exports supplied. Nothing has been written down, changed, approved or sent. Partner A decides every flag and approves Part A before anyone sends it.
```

## What was observed

The run did not reach any stop condition: the inputs were for one client, one matter and one period, every column was found under its default heading, no entry number repeated, no adjustment named an expense, and the tie-out held. Every figure ties to the pre-bill: 14 entries each checked at hours times rate, fees $13,136.00, adjustments $450.00, expenses $1,434.90, total $14,120.90. Sections 3, 4 and 5 each add to 30.7 hours and $13,136.00. Task and phase lines came only from the codes recorded, named from the guidelines' lists.

Compared with the published example:

- The six guideline flags are the same six, in the same order, on the same entries and expenses, with the same amounts affected. Flag 3 (the internal conference) gives the amount for each entry that could stay, "$225.00 if entry 1005 stays; $325.00 if entry 1006 stays", as the instructions now ask.
- The one description to reword (entry 1009, a settlement position and a view of a weakness) and the one other question (entry 1010, Bates-numbering, which guideline 2.6 can be read to cover or not) are the same. The production plan entries (1005 to 1007) were not listed for rewording.
- Expense E204 (outside printing) is flagged under 3.4 for the missing receipt only; the run did not treat 3.2's copying and printing done at the firm as reaching it.
- The overview runs to four sentences, phase by phase in date order, within the two to four the format asks for.
- The budget line compares and states the stage the budget covers, as the example does: $53,936.00 of $60,000.00, $6,064.00 remaining.
- The questions to the attorney name the courses open (keep, split, take off, obtain a receipt) without preferring one.
- Dates follow the format's style: years in the header and the matter line, "1 to 7 October" in the phase lines.

Where the run departed from the output format or the example:

- Flags 1, 2 and 3 set out their entries or activities as indented sub-lists rather than in one line each.
- It added a line before the closing line, "No duplicate entries, no adjustments without an approver, and no blank task codes were found.", which the format does not show.
- Under "Not checkable from the inputs" it listed only the 2.1 notice and consent. It did not list the prior approval in 2.3 for days over 10 hours (no timekeeper passed 10 hours on any day); the example lists it, as the procedure asks for every rule that cannot be checked.

Facts not in the inputs: none found. Every narrative uses words from the entries and expenses; the review of the first production set is described as before service, as entry 1014 says.

This is one run, by one assistant, on an invented example. It shows the instructions can be followed to a complete output that matches the example's flags and figures. It does not show how the template behaves with real exports, other guidelines or other AI products.

## The earlier runs, and what changed

**First run** (Claude Sonnet 5.5, run in Claude Code). It matched the example's six flags, its description to reword and its figures, and it raised entry 1010 under "Other questions" because guideline 2.6 can be read two ways; the example had not. It left these points open, and each was changed in the template before the later runs:

- Whether "a plan for the matter" in the descriptions to reword covers a document production plan. Now: "the firm's plan for how the matter will be argued or resolved"; ordinary work plans such as a production plan or a filing schedule are not listed.
- How open the question to the attorney may be beside "recommend nothing". Now: the question may name the courses open without preferring one.
- Whether an entry or expense reached by two guideline rules is flagged once or twice. Now: one flag citing both sections, counted once.
- Where a task or phase code's name comes from. Now: from the guidelines' list of codes, or the code alone.
- How to treat a budget limited to a stage. Now: say so on the budget line and compare only if the fees billed to date and this invoice's fees fall within the same stage; otherwise put it under "Other questions".
- How to write dates. Now: day, month name and year, with the year left out inside the billing period's lines.
- The pasted instructions now also confirm one client, one matter and one billing period, give the path for a client with no billing guidelines, and refuse to repeat a login code as well as bank details or a password.

**Second run** (Claude Opus 5.5, a fresh session started from Claude Code, as above). It followed the revised instructions, with two results that led to further changes:

- Under the first wording of the date rule it left the year out of every date, including the billing period. The rule was rewritten to the one above.
- It did not compare the budget, because the example's fees billed to date did not say which stage they came from. The example's matter settings now say they were all for case assessment.

**Third run** (Claude Opus 5.5, a fresh session started from Claude Code, as above). It matched the example's six flags, figures, description to reword and other question, and it listed the 2.3 prior approval as not checkable, which the example then did too. After it, only the example's output was edited at first: it came to count 1 other question and list entry 1010; to name the stage on the budget line; to say "for responsiveness and privilege", "reviewed before service" and "Bates-numbering" as the entries say. No figure changed. The third run also departed from the format in ways that an independent review then traced to the pasted instructions, which led to the changes below:

- Its overview ran to eleven sentences where the format asks for two to four. The pasted instructions did not state the length; step 6 now says the overview is two to four sentences.
- For flag 3 it gave the amount affected as $550.00, with each entry's amount beside it, where the procedure asks for the amount depending on which entry stays. The pasted instructions gave an amount rule only for rates; step 3 now gives the procedure's rule for each kind of flag, and for an internal conference asks for the amount "if entry [number] stays" for each entry.
- It put the section headings in bold, wrote the checks run and the rules not checkable as bulleted lists, and called the internal conference an "internal meeting". These were left as they were.

The same review led to three smaller changes before the fourth run. Narratives are now written "from the time and expense entries only", since the example's overview names a delivery date that comes from an expense. Guideline 3.2 in the example's inputs now reads "copying and printing done at the firm", where "in-house copying and printing" could be read to bar all printing. "Organised" and "organising" in the example's inputs became "organized" and "organizing".

**After the recorded run** only the example's output was edited; the instructions, the output format and the example's inputs were not changed. Flag 3's amount affected now reads "$325.00 if entry 1006 stays, $225.00 if entry 1005 stays", in the form the instructions give, and "organizing" and "organized" in flag 4 and the other question follow the inputs. No figure changed.
