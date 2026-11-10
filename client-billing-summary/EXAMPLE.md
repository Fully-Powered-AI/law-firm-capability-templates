# Client billing summary: an invented example

*Illustrative example with invented data.* The firm, the client, the other party, the vendors, every entry, every guideline and every figure below are invented. The firm is an invented 30-person business law firm. Its billing coordinator prepares the October invoice on a dispute it handles for Client A against Supplier B, and the responsible attorney, Partner A, reviews it. Timekeepers are referred to by role and letter, and vendors by letter.

The inputs come first, in full, so the template can be run on them. The summary follows.

## The inputs

### 1. Matter settings (typed by the billing coordinator)

```
Client: Client A
Matter: Dispute with Supplier B over late deliveries, matter 24-0317
Responsible attorney: Partner A
Billing period: 1 to 31 October 2026
Summary prepared: 4 November 2026
Fees billed on this matter before this invoice: $41,250.00, all for case assessment (phase P1)
```

### 2. Pre-bill totals

```
Pre-bill PB-1182, dated 3 November 2026
Client A, matter 24-0317, 1 to 31 October 2026
Fees: 13,136.00
Write-downs and discounts: 450.00
Expenses: 1,434.90
Invoice total: 14,120.90
```

### 3. Time export

```
Entry,Date,Timekeeper,Role,Task,Phase,Hours,Rate,Amount,Description
1001,2026-10-01,Partner A,Partner,T3,P1,1.0,650,650.00,Call with Client A's operations director on delivery history and the documents Client A holds
1002,2026-10-02,Associate B,Senior associate,T1,P1,3.2,450,1440.00,Reviewed Supplier B's 2026 delivery records and the delivery and notice terms of the supply agreement
1003,2026-10-05,Associate C,Associate,T1,P1,4.5,400,1800.00,"Built a chronology of orders, delivery dates and complaints from Client A's purchasing emails"
1004,2026-10-06,Associate C,Associate,T1,P1,2.0,400,800.00,Compared Client A's order records with Supplier B's delivery records for the chronology
1005,2026-10-07,Partner A,Partner,T4,P1,0.5,650,325.00,Internal conference with Associate B on the document production plan
1006,2026-10-07,Associate B,Senior associate,T4,P1,0.5,450,225.00,Internal conference with Partner A on the document production plan
1007,2026-10-09,Associate B,Senior associate,T2,P2,4.0,450,1800.00,Prepared the document production plan and search terms for the email review
1008,2026-10-14,Associate B,Senior associate,T1,P2,3.5,450,1575.00,Reviewed first production set; call with client on custodians; revised chronology
1009,2026-10-16,Partner A,Partner,T3,P2,0.8,650,520.00,Call with client on settlement range and weaknesses in the late-delivery claim
1011,2026-10-21,Associate C,Associate,T1,P2,5.0,400,2000.00,Reviewed Client A's purchasing emails for responsiveness and privilege (first batch)
1012,2026-10-22,Paralegal D,Paralegal,T2,P2,1.2,210,252.00,Organized the matter file and document index
1010,2026-10-26,Paralegal D,Paralegal,T2,P2,2.4,210,504.00,Bates-numbered the first production set
1013,2026-10-27,Associate B,Senior associate,T5,P2,0.6,450,270.00,Call with Supplier B's counsel on production dates and format
1014,2026-10-29,Partner A,Partner,T1,P2,1.5,650,975.00,Reviewed the first production set before service
```

### 4. Expense export

```
Entry,Date,Category,Vendor,Description,Amount,Receipt
E201,2026-10-09,Document hosting,Vendor A,"Hosting and processing of Client A's email collection, October",1150.00,yes
E202,2026-10-14,Meals,Café B,Lunch for the review team during document review at the firm's office,64.50,yes
E204,2026-10-23,Outside printing,Vendor D,Printing of the first production set for Client A's review,182.40,no
E203,2026-10-30,Courier,Courier C,Delivery of the first production set on a drive to Supplier B's counsel,38.00,yes
```

### 5. Adjustments export

```
Entry,Type,Amount,Approved by,Note for client
1007,write-down,450.00,Partner A,One hour of the production plan preparation written off.
```

### 6. Client A's billing guidelines (the billing sections, as supplied)

```
Client A Outside Counsel Billing Guidelines, version of 1 March 2026

2.1 Approved timekeepers and hourly rates for matter 24-0317: Partner A
    $650; Associate B $450; Associate C $380; Paralegal D $210. Rates
    may change only on 60 days' written notice and with Client A's
    consent in writing.
2.2 Every time entry carries one task code and one phase code.
    Task codes: T1 Review and analysis; T2 Preparation of documents;
    T3 Communication with client; T4 Communication within the firm;
    T5 Communication with other parties.
    Phase codes: P1 Case assessment; P2 Document production;
    P3 Depositions; P4 Trial preparation.
2.3 Time is recorded in tenths of an hour. No timekeeper bills more
    than 10 hours on one day without prior approval.
2.4 Each entry describes one task with its own time. Entries that put
    several tasks under one time are not paid.
2.5 A conference between the firm's own timekeepers is billed by one
    attendee only.
2.6 Administrative and clerical work, including scheduling, organizing
    files, indexing and copying, is not billable at any rate.
3.2 Not reimbursed: meals during local work, copying and printing
    done at the firm, office supplies, overtime.
3.4 Any single expense over $75 needs a receipt.
4.1 Budget for fees through the end of document production: $60,000.
```

## The output

**CLIENT BILLING SUMMARY: Client A, Dispute with Supplier B over late deliveries (24-0317)**

Billing period 1 to 31 October 2026. Pre-bill PB-1182, dated 3 November 2026. Prepared 4 November 2026 for Partner A.

**Status:** DRAFT. Not ready to send: 6 guideline flags, 1 description to reword, 1 other question open.

**Inputs not supplied:** none.

### PART A: FOR THE CLIENT, ONCE THE RESPONSIBLE ATTORNEY APPROVES

**1. Matter**

Client: Client A. Matter: Dispute with Supplier B over late deliveries, 24-0317. Billing period: 1 to 31 October 2026. Responsible attorney: Partner A. Billing guidelines: Client A Outside Counsel Billing Guidelines, version of 1 March 2026.

**2. Overview**

In October the work moved from case assessment to document production. In the first week the team reviewed Supplier B's delivery records and the supply agreement's delivery and notice terms, and built a chronology of orders, deliveries and complaints from Client A's own emails and order records. From 9 October it planned the production, reviewed Client A's purchasing emails, and prepared and reviewed the first production set, which was delivered to Supplier B's counsel on 30 October.

Fees \$13,136.00. Write-downs and discounts −\$450.00. Net fees \$12,686.00. Expenses \$1,434.90. Total for this invoice \$14,120.90.

**3. By timekeeper**

- Partner A, partner: 3.8 hours at \$650 = \$2,470.00. Calls with the client, the conference on the production plan, and review of the first production set before service.
- Associate B, senior associate: 11.8 hours at \$450 = \$5,310.00. Review of Supplier B's delivery records and the delivery and notice terms, the production plan and search terms, review of the first production set, a call with the client on custodians, and a call with Supplier B's counsel.
- Associate C, associate: 11.5 hours at \$400 = \$4,600.00. The chronology, built from Client A's purchasing emails and order records, and the first batch of the email review.
- Paralegal D, paralegal: 3.6 hours at \$210 = \$756.00. Bates-numbering the first production set, and the matter file and document index.

Total: 30.7 hours, \$13,136.00.

**4. By task**

- T1 Review and analysis: 19.7 hours, \$8,590.00. Review of Supplier B's delivery records and the delivery and notice terms; the chronology of orders, deliveries and complaints; review of Client A's purchasing emails for responsiveness and privilege; and review of the first production set before service.
- T2 Preparation of documents: 7.6 hours, \$2,556.00. The document production plan and the search terms for the email review, the Bates-numbering of the first production set, and the matter file and document index.
- T3 Communication with client: 1.8 hours, \$1,170.00. A call with Client A's operations director on its delivery history and the documents it holds, and a further call with the client on the matter.
- T4 Communication within the firm: 1.0 hours, \$550.00. A conference on the document production plan.
- T5 Communication with other parties: 0.6 hours, \$270.00. A call with Supplier B's counsel on production dates and format.

**5. By phase**

- P1 Case assessment, 1 to 7 October: 11.7 hours, \$5,240.00. Client A's delivery history, Supplier B's delivery records and the delivery and notice terms, the chronology, and planning for production.
- P2 Document production, 9 to 29 October: 19.0 hours, \$7,896.00. The production plan and search terms, the review of Client A's purchasing emails, and the first production set, Bates-numbered and reviewed before service.

**6. Expenses**

- 9 October, document hosting, Vendor A: hosting and processing of Client A's email collection, October, \$1,150.00.
- 14 October, meals, Café B: lunch for the review team during document review at the firm's office, \$64.50.
- 23 October, outside printing, Vendor D: printing of the first production set for Client A's review, \$182.40.
- 30 October, courier, Courier C: delivery of the first production set on a drive to Supplier B's counsel, \$38.00.

Subtotals: document hosting \$1,150.00; meals \$64.50; outside printing \$182.40; courier \$38.00. Total expenses \$1,434.90.

**7. Write-downs and discounts**

- Entry 1007, write-down: −\$450.00. One hour of the production plan preparation written off.

Fees in sections 3 to 5 are shown before write-downs.

### PART B: FOR THE RESPONSIBLE ATTORNEY ONLY. NEVER SENT TO THE CLIENT.

**Tie-out:** 14 time entries, hours times rate checked on each. Time entries \$13,136.00 = pre-bill fees \$13,136.00. Adjustments \$450.00 = pre-bill write-downs and discounts \$450.00. Expenses \$1,434.90 = pre-bill expenses \$1,434.90. \$13,136.00 − \$450.00 + \$1,434.90 = pre-bill total \$14,120.90.

**Checks run against Client A Outside Counsel Billing Guidelines, version of 1 March 2026:** 2.1, approved timekeepers and rates; 2.2, task and phase codes; 2.3, tenths of an hour and the 10-hour day; 2.4, several tasks under one time; 2.5, internal conferences; 2.6, administrative work; 3.2, expenses not reimbursed; 3.4, receipts over \$75; 4.1, budget. The firm's own: arithmetic, duplicate entries, adjustments with an approver.

**Not checkable from the inputs:** 2.1, whether 60 days' written notice of a rate change was given and Client A consented in writing; 2.3, prior approval for more than 10 hours on one day (no timekeeper billed more than 10 hours on any day).

**Budget:** \$41,250.00 billed to date + \$12,686.00 net fees this invoice = \$53,936.00 of \$60,000.00 (4.1, which covers fees through the end of document production; the fees billed to date are all case assessment, and this invoice's are case assessment and document production); \$6,064.00 remains.

**Guideline flags: 6**

1. Entries 1003, 1004 and 1011, 5 to 21 October, Associate C. Guideline 2.1: Associate C's approved rate is \$380. All three entries are billed at \$400, 11.5 hours in total. Amount affected: \$230.00. Decision: bill Associate C at \$400 or at the approved \$380?
2. Entry 1008, 14 October, Associate B. Guideline 2.4: one time for one task. The entry puts three activities under 3.5 hours: reviewing the first production set, a call with the client on custodians, and revising the chronology. Amount affected: \$1,575.00. Decision: split the entry into its activities with their own times, or another course?
3. Entries 1005 and 1006, 7 October, Partner A and Associate B. Guideline 2.5: one attendee bills a conference between the firm's own timekeepers. Both billed 0.5 hours for the same conference on the production plan: entry 1005, Partner A, \$325.00; entry 1006, Associate B, \$225.00. Amount affected: \$325.00 if entry 1006 stays, \$225.00 if entry 1005 stays. Decision: which entry stays on the invoice?
4. Entry 1012, 22 October, Paralegal D. Guideline 2.6: organizing files and indexing are not billable. The entry is "organized the matter file and document index", 1.2 hours. Amount affected: \$252.00. Decision: keep it on the invoice or take it off?
5. Expense E202, 14 October, Café B. Guideline 3.2: meals during local work are not reimbursed. The expense is a lunch during document review at the firm's office. Amount affected: \$64.50. Decision: keep it on the invoice or take it off?
6. Expense E204, 23 October, Vendor D. Guideline 3.4: a single expense over \$75 needs a receipt. The expense is \$182.40 and the export shows no receipt. Amount affected: \$182.40. Decision: find the receipt, or take the expense off?

**Descriptions to reword before the itemized detail prints: 1**

- Entry 1009, 16 October, Partner A: names a settlement position and a view of the weaknesses of a claim. Decision: reword, or approve as recorded.

**Other questions: 1**

- Guideline read two ways: entry 1010, 26 October, Paralegal D, "Bates-numbered the first production set", 2.4 hours, \$504.00. Guideline 2.6 makes administrative and clerical work not billable, "including scheduling, organizing files, indexing and copying". One reading: numbering a production set is clerical work of the same kind, and not billable. The other: it is production work that 2.6 does not name. Not checked. For: responsible attorney.

Prepared from pre-bill PB-1182 and the exports supplied. Nothing has been written down, changed, approved or sent. Partner A decides every flag and approves Part A before anyone sends it.
