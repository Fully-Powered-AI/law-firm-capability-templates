# Prebill exception review: tried once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (`claude-sonnet-5-5`)
- **Date:** 2026-11-10

The inputs are the invented example in [example.md](example.md) (Client R, Partner P, Associates Q and S, Paralegal T). No client data was used. The run was a single attempt by a model that did not write the template. It followed the instruction block and the output format in `member/template.md` and read the example's output only after producing its own.

## Inputs used

The "The inputs" part of [example.md](example.md): the prebill header (PB-2207), the time export (14 entries), the expense export (6), the adjustments export (2), the rate table (8 rows), Client R's billing guidelines (seven rules) and the firm settings (the template's defaults).

## What came out

```
PREBILL EXCEPTION SHEET: Client R, Warehouse lease renewal (26-0188)
Prebill PB-2207, dated 3 November 2026. Billing period 1 October to 31 October 2026. Billing attorney: Partner P. Prepared 4 November 2026 by the billing coordinator for the billing attorney's review.
Status: 16 exceptions. Time entries named: 11 of 14. Expenses named: 5 of 6. Adjustments queried: 1 of 2.
Inputs: prebill header; time export (14 entries); expense export (6 entries); adjustments export (2); rate table; client billing guidelines (Client R Billing Guidelines for Outside Counsel, 1 February 2026); firm settings (defaults).

TIE-OUT
14 time entries, hours x rate checked on each. Time entries 12,880.00 = prebill fees 12,880.00. Adjustments 340.00 = prebill adjustments 340.00. Expenses 462.20 = prebill expenses 462.20. 12,880.00 - 340.00 + 462.20 = prebill total 13,002.20.

1. RATE DIFFERENCES AGAINST THE RATE TABLE: 2
X1. Associate Q, billed at 410.00. Table rate 430.00 (Client R row, effective 1 October 2026). Entries T502, T506, T510, T511, 16.9 hours. Difference: 338.00 below the table. The billed rate matches the Client R row, which ended 30 September 2026. For: billing attorney.
X2. Paralegal T, billed at 220.00. Table rate 195.00 (Client R row, effective 1 January 2026). Entries T504, T512, 1.75 hours. Difference: 43.75 above the table. The billed rate matches the Standard row. For: billing attorney.

2. POSSIBLE DUPLICATES: 2
X3. Entries T508, T509, Associate S, 12 October: same date and narrative (and the same hours, 2.0). Amount at stake: 760.00 if T509 is the duplicate. For: billing attorney.
X4. Expenses E203, E204, Vendor C, 14 and 15 October: the same support reference (INV-C-881), and the same vendor and amount (42.00) one day apart. Amount at stake: 42.00 if E204 is the duplicate. For: billing attorney.

3. OUTSIDE THE CLIENT'S BILLING GUIDELINES: 4
X5. Entry T512, 20 October, Paralegal T. Guideline 1: time in tenths of an hour; other increments are not paid. Guideline 4: clerical work is not billable, calendaring named. Recorded as 0.25 hours; the narrative is "Calendared the landlord's response deadline for the counterproposal". Amount at stake: 55.00; under guideline 4: 55.00. For: billing attorney.
X6. Entries T510, T511, 14 October, Associate Q. Guideline 2: no more than 10.0 hours on one day. 6.0 + 4.8 = 10.8 hours, 0.8 over the limit. Amount at stake: 328.00 (0.8 x 410.00, the rate on T511). For: billing attorney.
X7. Entry T504, 6 October, Paralegal T. Guideline 4: clerical work is not billable, organizing files named. The narrative is "Organized the lease correspondence file". Amount at stake: 330.00. For: billing attorney.
X8. Expense E202, 9 October, Café D. Guideline 6: meals are not reimbursed. Type Meals, 46.80. Amount at stake: 46.80. For: billing attorney.

4. NARRATIVES TO CLARIFY: 5
X9. Entry T505, 7 October, Partner P, 0.8 hours: "Attention to file". Unclear: 3 words, under the minimum of 5, and the vague phrase "attention to". Back to: Partner P, to rewrite.
X10. Entry T506, 8 October, Associate Q, 3.6 hours: "Reviewed landlord's counsel's markup of the renewal terms; prepared issues list; call with Partner P". Block entry: three activities separated by semicolons. Also guideline 3: one task per entry, block entries not paid; amount at stake 1,476.00. Back to: Associate Q, to split with a time for each task.
X11. Entry T507, 9 October, Partner P, 0.6 hours. Sensitive detail: words from the firm's list: lowest, weak. Not judged here. For: billing attorney.
X12. Entry T511, 14 October, Associate Q, 4.8 hours: "Call with landlord's counsel on the counterproposal and revised the counterproposal". Block entry: a call together with revising the counterproposal. Also guideline 3: one task per entry, block entries not paid; amount at stake 1,968.00. Back to: Associate Q, to split with a time for each task.
X13. Entry T513, 26 October, Partner P, 1.0 hours: "Review". Unclear: 1 word, under the minimum of 5. Back to: Partner P, to rewrite.

5. EXPENSES WITHOUT SUPPORT: 2
X14. Expense E205, 21 October, Outside copying, Vendor E, 128.40: no support reference. Also guideline 7: expenses over 50.00 need a receipt or vendor invoice; amount at stake 128.40. Back to: Paralegal T, for the receipt or invoice.
X15. Expense E206, 27 October, Parking, Garage F, 18.00: no support reference. The client's rule (7) does not reach it. Back to: Associate S, for the receipt or invoice.

6. ADJUSTMENTS WITHOUT APPROVAL OR REASON: 1
X16. Adjustment on T514, 150.00, reason "Courtesy discount": no approver. For: billing attorney.

GUIDELINE RULES
Checked: 1 (G1, time increment); 2 (G2, hours per day); 3 (G3, one task per entry); 4 (G4, work not billable); 6 (G6, expense types not reimbursed); 7 (G7, receipt threshold).
Not checked:
- 5: research over 3.0 hours on any one issue needs Client R's prior written approval. Needs something not in the exports: the approvals, and which issue each entry concerns.

WHO HAS WHAT
Back to the timekeeper or submitter:
- Partner P: X9, X13.
- Associate Q: X10, X12.
- Paralegal T: X14.
- Associate S: X15.
For the billing attorney (Partner P): X1, X2, X3, X4, X5, X6, X7, X8, X11, X16; and X10, X12, X14 once returned, for the billability decision.
Finance: approves the invoice preparation once those decisions are entered.

Amounts at stake are not added together: one entry can appear under several checks.
Prepared from prebill PB-2207 and the exports supplied. No entry, rate, narrative, expense or adjustment has been changed, written down or approved, and nothing has been sent. The billing attorney decides billability and every narrative change; finance approves the invoice preparation.
```

## What was observed

- **Every required part was produced:** the heading, status line, inputs line, tie-out, six numbered sections, the guideline rules, who has what, and the closing lines. The tie-out passed on every line (all 14 entries multiply out, the sums match the header), so the run did not stop. Nothing in the inputs triggered a stop condition, and no stop was needed for a missing column or file.
- **It matches the published example in substance.** The same 16 exceptions, in the same order, with the same amounts, the same routing and the same counts. Rule 5 of the guidelines went under "Not checked" in both.
- **Differences from the published example:**
  - The billing period is written "1 October to 31 October 2026" here and "1 to 31 October 2026" there. The template does not say how to write a range, so both are defensible.
  - The duplicate exception X3 is worded "same date and narrative (and the same hours, 2.0)" against "same timekeeper, date, hours (2.0) and narrative". The facts are the same.
  - X1 and X2 say the billed rate matches "the Client R row" and "the Standard row" without repeating the 410.00 and 220.00 figures, which the example does. The facts are the same.
  - Small wording changes in the guideline summaries in X5, X10, X12 and X14. No figure, entry or routing differs.
- **Facts not in the inputs:** none in this run's output. In the published example, every figure and entry traces to the inputs. The derived figures (16.9 and 1.75 hours, 10.8 hours, 338.00, 43.75, 328.00) all recompute from them.
- **Where the instructions were ambiguous, and a guess was needed:**
  - The order of exceptions within section 1 is not stated. This run ordered them by first entry; ordering by timekeeper name would give the same result here.
  - In section 4, sensitive-detail exceptions are "always their own exception" and the section is "listed by date". This run interleaved them by date with the other narrative exceptions. A reader could instead put them last.
  - Guideline sections and the template's G-labels coincide in this example (guideline 2 is G2, guideline 6 is G6). On a client whose guidelines are numbered differently, the output's "Guideline [section]" and the "G1" to "G8" labels could be confused. The format uses both without saying which appears where.
  - Guideline 4 says clerical work "including" four named kinds. The template says to use only the words the guideline names, so only those four were searched for, and the rule was not put under "Not checked" as readable two ways. That follows the template, but a reader might expect the broader reading to be flagged.
  - The G4 check is defined on narratives only. Expense E205 (Outside copying) involves copying, a named kind, and was not flagged under G4. The template is silent on expense descriptions.
  - Guideline 6 refuses "online research charges". The only research-like expense is a title search. The template matches on the expense `Type` and the guideline's named types, so it was not flagged, and no instruction says to ask.
  - Partner P is both a timekeeper (X9, X11, X13) and the billing attorney. Nothing says what to do when the sheet routes an entry back to, or for review by, the same person.
  - Block entries are listed under narratives (section 4), not under "Outside the client's billing guidelines" (section 3), even when guideline 3 is cited. The section 3 title and count therefore leave them out. The template says this, but a reader may not expect it.
  - Whether the routing line "once returned, for the billability decision" applies to an expense returned for support that cites guideline 7 (X14) is only implied by "a returned entry". This run applied it.
- **Told to stop:** nothing.
- **Shortcomings:** the run is one attempt by one model on one invented example. It shows the instructions can be followed to the published result. It does not show how the template behaves on a real prebill, on other client guidelines, or in other AI products.

## After this run

The template was edited after this run, on the points above, to settle the order of exceptions, where sensitive-detail exceptions sit, which guideline label appears where, how a rate match, a billing period and a rule that says "including" are written, that guideline 4 is checked on time narratives only, and what happens when the billing attorney is also the timekeeper. The published example now carries one added line under "Not checked" for guideline 4. The template was not run again after these edits, so this record, including its output and observations, is of the earlier text and is unchanged. A few smaller edits followed a review: the instruction block now says what guideline 5 flags and no longer offers neutral wording for a narrative, the template's customization list gained a note on mapping expense types to a guideline's wording (the ambiguity noted above for guideline 6), and the example's "Not checked" line for guideline 4 was reworded. The template has still not been run again.
