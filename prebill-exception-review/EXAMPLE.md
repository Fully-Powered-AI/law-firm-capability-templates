# Prebill exception review: an invented example

*Illustrative example with invented data.* The firm, the client, the landlord, the vendors, every entry, every rate, every guideline and every figure below are invented. The firm is an invented 22-lawyer business law firm. Its billing coordinator prepares the exception sheet for the October prebill on a lease renewal it is negotiating for Client R, an invented food distributor, before the billing attorney, Partner P, reviews the prebill. Timekeepers are referred to by role and letter, and vendors by letter.

The inputs come first, in full, so the template can be run on them. The exception sheet follows.

## The inputs

### 1. Prebill header (typed by the billing coordinator)

```
Prebill: PB-2207, dated 3 November 2026
Client: Client R
Matter: Warehouse lease renewal, 26-0188
Billing period: 1 to 31 October 2026
Billing attorney: Partner P
Fees before adjustments: 12,880.00
Adjustments: 340.00
Expenses: 462.20
Prebill total: 13,002.20
```

### 2. Time export

```
Entry,Date,Timekeeper,Hours,Rate,Amount,Narrative
T501,2026-10-01,Partner P,1.2,640.00,768.00,Call with Client R's facilities director on the renewal notice and the landlord's rent increase
T502,2026-10-02,Associate Q,2.5,410.00,1025.00,Reviewed the current warehouse lease and its 2021 amendment for the renewal option and notice dates
T503,2026-10-05,Associate S,3.0,380.00,1140.00,Prepared a comparison of the landlord's proposed renewal terms with the current lease
T504,2026-10-06,Paralegal T,1.5,220.00,330.00,Organized the lease correspondence file
T505,2026-10-07,Partner P,0.8,640.00,512.00,Attention to file
T506,2026-10-08,Associate Q,3.6,410.00,1476.00,Reviewed landlord's counsel's markup of the renewal terms; prepared issues list; call with Partner P
T507,2026-10-09,Partner P,0.6,640.00,384.00,Call with Client R's CFO on the lowest rent Client R will accept and the weak points in its position if the landlord refuses to renew
T508,2026-10-12,Associate S,2.0,380.00,760.00,Reviewed the landlord's estoppel certificate request
T509,2026-10-12,Associate S,2.0,380.00,760.00,Reviewed the landlord's estoppel certificate request
T510,2026-10-14,Associate Q,6.0,410.00,2460.00,Prepared the counterproposal on renewal terms
T511,2026-10-14,Associate Q,4.8,410.00,1968.00,Call with landlord's counsel on the counterproposal and revised the counterproposal
T512,2026-10-20,Paralegal T,0.25,220.00,55.00,Calendared the landlord's response deadline for the counterproposal
T513,2026-10-26,Partner P,1.0,640.00,640.00,Review
T514,2026-10-28,Associate Q,1.4,430.00,602.00,Call with landlord's counsel on the new rent schedule
```

### 3. Expense export

```
Entry,Date,Type,Vendor,Amount,Support,Submitted by,Description
E201,2026-10-05,Title search,Vendor A,185.00,INV-A-3310,Associate S,Title and lien search on the warehouse property
E202,2026-10-09,Meals,Café D,46.80,RCPT-1009,Partner P,Lunch during the meeting with Client R's facilities team
E203,2026-10-14,Courier,Vendor C,42.00,INV-C-881,Paralegal T,Delivery of the counterproposal to landlord's counsel
E204,2026-10-15,Courier,Vendor C,42.00,INV-C-881,Paralegal T,Delivery of the counterproposal to landlord's counsel
E205,2026-10-21,Outside copying,Vendor E,128.40,,Paralegal T,"Copies of the lease, amendment and counterproposal for the client meeting"
E206,2026-10-27,Parking,Garage F,18.00,,Associate S,Parking for the meeting at Client R's warehouse
```

### 4. Adjustments export

```
Entry,Adjustment,Approved by,Reason
T503,190.00,Partner P,Half an hour of the comparison written down
T514,150.00,,Courtesy discount
```

### 5. The firm's rate table

```
Timekeeper,Rate,Applies to,Effective from,Effective to
Partner P,700.00,Standard,2026-01-01,
Partner P,640.00,Client R,2026-01-01,
Associate Q,450.00,Standard,2026-01-01,
Associate Q,410.00,Client R,2026-01-01,2026-09-30
Associate Q,430.00,Client R,2026-10-01,
Associate S,380.00,Standard,2026-01-01,
Paralegal T,220.00,Standard,2026-01-01,
Paralegal T,195.00,Client R,2026-01-01,
```

### 6. Client R's billing guidelines (as supplied)

```
Client R Billing Guidelines for Outside Counsel, 1 February 2026

1. Record time in tenths of an hour. Entries recorded in any other
   increment are not paid.
2. No timekeeper may bill more than 10.0 hours on one day.
3. Each time entry describes one task. Block entries are not paid.
4. Clerical work is not billable, including organizing files,
   scanning, copying and calendaring.
5. Research over 3.0 hours on any one issue requires Client R's prior
   written approval.
6. Not reimbursed: meals, online research charges and overtime.
7. Each expense over $50.00 must be supported by a receipt or vendor
   invoice.
```

### 7. Firm settings

```
Prepared: 4 November 2026, by the billing coordinator
Firm settings: the template's defaults
  Narrative minimum: 5 words
  Vague phrases: attention to; work on; various; miscellaneous;
    follow up; review file; file review
  Sensitive words: settle; settlement; lowest; highest; bottom line;
    walk away; weak; weakness; strong; strength; strategy; advice;
    advised; opinion; exposure
  Expense support: every expense needs a support reference
  Duplicate window: 3 days for time entries, 7 days for expenses
```

## The output

```
PREBILL EXCEPTION SHEET: Client R, Warehouse lease renewal (26-0188)
Prebill PB-2207, dated 3 November 2026. Billing period 1 to 31 October 2026. Billing attorney: Partner P. Prepared 4 November 2026 by the billing coordinator for the billing attorney's review.
Status: 16 exceptions. Time entries named: 11 of 14. Expenses named: 5 of 6. Adjustments queried: 1 of 2.
Inputs: prebill header; time export (14 entries); expense export (6 entries); adjustments export (2); rate table; client billing guidelines (Client R Billing Guidelines for Outside Counsel, 1 February 2026); firm settings (defaults).

TIE-OUT
14 time entries, hours x rate checked on each. Time entries 12,880.00 = prebill fees 12,880.00. Adjustments 340.00 = prebill adjustments 340.00. Expenses 462.20 = prebill expenses 462.20. 12,880.00 - 340.00 + 462.20 = prebill total 13,002.20.

1. RATE DIFFERENCES AGAINST THE RATE TABLE: 2
X1. Associate Q, billed at 410.00. Table rate 430.00 (Client R row, effective 1 October 2026). Entries T502, T506, T510, T511, 16.9 hours. Difference: 338.00 below the table. The billed rate matches the Client R 410.00 row, which ended 30 September 2026. For: billing attorney.
X2. Paralegal T, billed at 220.00. Table rate 195.00 (Client R row, effective 1 January 2026). Entries T504, T512, 1.75 hours. Difference: 43.75 above the table. The billed rate matches the Standard 220.00 row. For: billing attorney.

2. POSSIBLE DUPLICATES: 2
X3. Entries T508, T509, Associate S, 12 October: same timekeeper, date, hours (2.0) and narrative. Amount at stake: 760.00 if T509 is the duplicate. For: billing attorney.
X4. Expenses E203, E204, Vendor C, 14 and 15 October: the same support reference (INV-C-881), and the same vendor and amount (42.00) one day apart. Amount at stake: 42.00 if E204 is the duplicate. For: billing attorney.

3. OUTSIDE THE CLIENT'S BILLING GUIDELINES: 4
X5. Entry T512, 20 October, Paralegal T. Guideline 1: time in tenths of an hour; entries in any other increment are not paid. Guideline 4: clerical work is not billable, calendaring named. Recorded as 0.25 hours; the narrative is "Calendared the landlord's response deadline for the counterproposal". Amount at stake: 55.00; under guideline 4: 55.00. For: billing attorney.
X6. Entries T510, T511, 14 October, Associate Q. Guideline 2: no more than 10.0 hours on one day. 6.0 + 4.8 = 10.8 hours, 0.8 over the limit. Amount at stake: 328.00 (0.8 x 410.00, the rate on T511). For: billing attorney.
X7. Entry T504, 6 October, Paralegal T. Guideline 4: clerical work is not billable, organizing files named. The narrative is "Organized the lease correspondence file". Amount at stake: 330.00. For: billing attorney.
X8. Expense E202, 9 October, Café D. Guideline 6: meals are not reimbursed. Type Meals, 46.80. Amount at stake: 46.80. For: billing attorney.

4. NARRATIVES TO CLARIFY: 5
X9. Entry T505, 7 October, Partner P, 0.8 hours: "Attention to file". Unclear: 3 words, under the 5-word minimum, and the vague phrase "attention to". Back to: Partner P, to rewrite.
X10. Entry T506, 8 October, Associate Q, 3.6 hours: "Reviewed landlord's counsel's markup of the renewal terms; prepared issues list; call with Partner P". Block entry: three activities separated by semicolons (reviewing the markup, preparing the issues list, a call with Partner P). Also guideline 3: each entry describes one task, and block entries are not paid; amount at stake 1,476.00. Back to: Associate Q, to split with a time for each task.
X11. Entry T507, 9 October, Partner P, 0.6 hours. Sensitive detail: words from the firm's list: lowest, weak. Not judged here. For: billing attorney.
X12. Entry T511, 14 October, Associate Q, 4.8 hours: "Call with landlord's counsel on the counterproposal and revised the counterproposal". Block entry: a call together with revising the counterproposal. Also guideline 3: each entry describes one task, and block entries are not paid; amount at stake 1,968.00. Back to: Associate Q, to split with a time for each task.
X13. Entry T513, 26 October, Partner P, 1.0 hours: "Review". Unclear: 1 word, under the 5-word minimum. Back to: Partner P, to rewrite.

5. EXPENSES WITHOUT SUPPORT: 2
X14. Expense E205, 21 October, Outside copying, Vendor E, 128.40: no support reference. Also guideline 7: each expense over 50.00 needs a receipt or vendor invoice; amount at stake 128.40. Back to: Paralegal T, for the receipt or invoice.
X15. Expense E206, 27 October, Parking, Garage F, 18.00: no support reference. The client's rule (7) does not reach it. Back to: Associate S, for the receipt or invoice.

6. ADJUSTMENTS WITHOUT APPROVAL OR REASON: 1
X16. Adjustment on T514, 150.00, reason "Courtesy discount": no approver. For: billing attorney.

GUIDELINE RULES
Checked: 1 (G1, time increment); 2 (G2, hours per day); 3 (G3, one task per entry); 4 (G4, work not billable); 6 (G6, expense types not reimbursed); 7 (G7, receipt threshold).
Not checked:
- 5: research over 3.0 hours on any one issue needs Client R's prior written approval. Needs something not in the exports: the approvals, and which issue each entry concerns.
- 4: clerical work is not billable, including organizing files, scanning, copying and calendaring. Names words after "including": only those words are checked, and only in time narratives, not in expense descriptions; the rest of the rule is not.

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

Entries T501 and T503 raised no exception, nor did T514 itself (only its adjustment is queried), nor expense E201. The adjustment on T503 has both an approver and a reason, so it is not listed.
