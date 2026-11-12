# Matter closing checklist preparation: an invented example

*Illustrative example with invented data.* The firm, the clients, the people, the matters, the dates and every amount below are invented. The firm is an invented litigation practice with a billing coordinator and a records clerk, and the matter is a supply dispute between Client C and Party D. First come the inputs the operations assistant supplied, in full, then the checklist the workflow template returns. The unreturned-items list and the firm's checklist are supplied for this one matter, so they carry no matter number.

## The inputs

### 1. Closure flag

```
Matter 25-0187 flagged for closure by Attorney R (responsible attorney) on 2026-11-09.
Prepared on 2026-11-10 for the operations assistant.
```

### 2. Attorney's outcome note (supplied by Attorney R)

```
Settled. The parties signed a settlement agreement on 2026-10-28. Client C
received the agreed payment from Party D on 2026-11-03. The court dismissed
the claim by order dated 2026-11-05. Party D has a separate matter with us,
25-0203, which is not part of this one. The settlement requires Client C to
confirm in writing by 2026-12-15 that Party D's disclosed documents have been
returned or destroyed. No hold instructed.
```

### 3. Matter record export

```
matter_no,client,matter_name,responsible_attorney,opened,status,practice_group,hold
25-0187,Client C,Client C v Party D (supply dispute),Attorney R,2025-03-17,Open,Litigation,
25-0203,Party D,Party D collections review,Attorney S,2025-09-02,Open,Commercial,
```

### 4. Tasks export (finished words: Done, Cancelled)

```
matter_no,task,owner,due,status
25-0187,Save the court order to the file,Paralegal A,2026-11-06,Done
25-0187,Send final status letter to Client C,Attorney R,2026-11-09,Open
25-0187,Obtain Party D payment confirmation for the file,,2026-11-04,Open
25-0187,Review draft invoice 25-0187-07,Attorney R,2026-11-12,Open
25-0187,Clear calendar reminders,Paralegal A,2026-11-10,Cancelled
25-0203,Send intake reminder,Paralegal B,2026-11-11,Open
```

### 5. Billing export

```
matter_no,item,kind,amount,paid,status
25-0187,25-0187-05,invoice,12400.00,12400.00,Paid
25-0187,25-0187-06,invoice,9850.50,6000.00,Issued
25-0187,25-0187-07,invoice,3210.00,0.00,Draft
25-0187,WIP-time,unbilled time,1480.00,,Unbilled
25-0187,WIP-expenses,unbilled expense,265.75,,Unbilled
25-0187,Trust,client funds held,2500.00,,Held
25-0203,25-0203-02,invoice,4000.00,4000.00,Paid
```

### 6. Unreturned-items list (kept by records)

```
item,kind,held_by,returned_to_client,returned_on
Original supply agreement,original document,Records,Yes,2026-11-06
Client C board minutes (originals),original document,Records,No,
Exhibit binder 1,physical file,Records,Yes,2026-11-06
USB drive from Client C,client property,Attorney R,No,
Exhibit binder 2,physical file,Records,,
```

### 7. The firm's closing checklist

```
item_id,item,owner_role,handoff_to,done_on,accepted_on
C1,Final order or dismissal on file,Paralegal,,2026-11-06,
C2,Final status letter to client,Responsible attorney,,,
C3,Final invoice issued and billing balance reviewed,Billing coordinator,Billing,,
C4,Trust account balance handled,Billing coordinator,Billing,,
C5,Original documents and client property returned,Records clerk,Records,,
C6,Closing memo to records,Responsible attorney,Records,2026-11-09,
C7,Calendar entries cleared,Paralegal,,2026-11-10,
C8,Retention class assigned,Records owner,Records,,
```

## The output

The checklist is plain text, in the template's fixed order. Roles are copied from the exports as written.

```
MATTER CLOSING CHECKLIST: Matter 25-0187, Client C, Client C v Party D (supply dispute)
Version: 1, prepared 2026-11-10. Flagged for closure by Attorney R on 2026-11-09.

Sources read: closure flag; attorney's outcome note; matter record export; tasks export; billing export; unreturned-items list; the firm's closing checklist.

Outcome as supplied by Attorney R: "Settled. The parties signed a settlement agreement on 2026-10-28. Client C received the agreed payment from Party D on 2026-11-03. The court dismissed the claim by order dated 2026-11-05." Recorded as supplied, not assessed.

Final billing status as recorded:
- Invoices: 3 for this matter, invoice amounts including drafts 25,460.50, paid 18,400.00.
- Invoice 25-0187-05: 12,400.00, paid 12,400.00, Paid.
- Invoice 25-0187-06: 9,850.50, paid 6,000.00, Issued. Outstanding 3,850.50.
- Draft invoices: 25-0187-07, 3,210.00, not issued.
- Unbilled time 1,480.00 and unbilled expenses 265.75: 1,745.75 together.
- Open in billing as recorded: 3,850.50 + 3,210.00 + 1,745.75 = 8,806.25 across 3 lines.
- Client funds held: 2,500.00 (shown separately).
- Billing questions: none

Outstanding tasks: 3 open of 5 for this matter (2 finished).
- Send final status letter to Client C. Owner: Attorney R. Due 2026-11-09, date passed.
- Obtain Party D payment confirmation for the file. Owner: not assigned. Due 2026-11-04, date passed.
- Review draft invoice 25-0187-07. Owner: Attorney R. Due 2026-11-12.

Unreturned items: 3 of 5.
- Client C board minutes (originals), original document, held by Records: not returned.
- USB drive from Client C, client property, held by Attorney R: not returned.
- Exhibit binder 2, physical file, held by Records: return not recorded.

Firm closing checklist: 3 of 8 recorded done, 5 not.
- C1 Final order or dismissal on file: done 2026-11-06.
- C2 Final status letter to client: not done. Owner: Responsible attorney.
- C3 Final invoice issued and billing balance reviewed: not done. Owner: Billing coordinator.
- C4 Trust account balance handled: not done. Owner: Billing coordinator.
- C5 Original documents and client property returned: not done. Owner: Records clerk.
- C6 Closing memo to records: done 2026-11-09.
- C7 Calendar entries cleared: done 2026-11-10.
- C8 Retention class assigned: not done. Owner: Records owner.

Handoffs: 5, 0 accepted on the record.
- To Billing: C3, C4. Awaiting acceptance by Billing.
- To Records: C5, C6, C8. Awaiting acceptance by Records. C6 is marked done by its owner; acceptance is not recorded.

Kept explicit:
- Related proceeding: "Party D has a separate matter with us, 25-0203, which is not part of this one." Matter record status of 25-0203: Open.
- Unfinished obligation: "The settlement requires Client C to confirm in writing by 2026-12-15 that Party D's disclosed documents have been returned or destroyed."
- Hold instruction: "No hold instructed."; matter record hold column: blank.
- Open billing questions: none

Counts: open tasks 3; open billing lines 3 (and funds held 1 item); unreturned items 3; checklist items not done 5 of 8; handoffs awaiting acceptance 5; items kept explicit 3.

Decisions that belong to others: whether the matter can close: Attorney R, no decision recorded. How long the file is kept: records owner; no retention period is set here.

Next action: Attorney R: Send final status letter to Client C (due 2026-11-09).
Changes since last version: none

Prepared for the operations assistant. Nothing has been closed, sent, entered or changed.
```
