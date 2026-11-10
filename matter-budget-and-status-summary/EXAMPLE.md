# Matter budget and status summary: an invented example

*Illustrative example with invented data.* The firm, its people, its client, the matter and every record below are invented. People are shown by role and letter. The firm is a small business law firm with eight lawyers. Its operations lead prepares the summary for Partner A, the responsible partner on matter M-4412, as of Friday 6 November 2026. First come the inputs, in full, then what came back.

## The inputs

### 1. The request

```
Prepare the budget and status summary for M-4412 as of Friday 6 November
2026, for Partner A. Attached: the matter plan with phases.csv, the time
export time.csv from the billing system, and Associate B's notes.
Use the default settings and column headers.
```

### 2. The matter plan, with its phase table

```
Matter plan: M-4412, dated 2026-11-02 (kept by Associate B)

Matter: M-4412 Purchase of a regional bakery business
Client: Client R
Responsible partner: Partner A
Fee arrangement: hourly, against an agreed estimate
Matter budget: $60,000, last agreed with the client 2026-08-28
In scope: due diligence on the target business; negotiating the purchase
  terms with the seller's counsel; closing and the post-closing list.
Out of scope: tax structuring; employee matters; the client's financing
  with its lender.
```

**phases.csv**

```
phase_code,phase,planned_start,planned_end,budget,status,completed_on,remaining_estimate
P1,Due diligence,2026-09-01,2026-10-09,24000,complete,2026-10-16,0
P2,Negotiation of terms,2026-10-05,2026-11-13,22000,in progress,,9000
P3,Closing and post-closing,2026-11-16,2026-12-11,14000,not started,,14000
```

### 3. The time export

**time.csv** (from the billing system; the firm's export groups each timekeeper's week on a phase into one row)

```
entry_id,matter_id,date,timekeeper,phase_code,hours,rate,amount,billed
T-01,M-4412,2026-09-02,Partner A,P1,4.0,600,2400,yes
T-02,M-4412,2026-09-03,Associate B,P1,3.0,400,1200,no
T-03,M-4412,2026-09-15,Associate B,P1,22.0,400,8800,yes
T-04,M-4412,2026-09-22,Paralegal D,P1,15.0,180,2700,yes
T-05,M-4412,2026-10-02,Associate C,P1,12.0,350,4200,yes
T-06,M-4412,2026-10-14,Associate B,P1,10.0,400,4000,yes
T-07,M-4412,2026-10-16,Partner A,P1,4.5,600,2700,yes
T-08,M-4412,2026-10-08,Partner A,P2,6.0,600,3600,yes
T-09,M-4412,2026-10-20,Associate B,P2,14.0,400,5600,yes
T-10,M-4412,2026-10-29,Associate C,P2,8.0,350,2800,no
T-11,M-4412,2026-11-03,Partner A,P2,3.5,600,2100,no
T-12,M-4412,2026-11-04,Associate B,P2,3.0,400,1200,no
T-13,M-4412,2026-11-05,Paralegal D,P3,1.0,180,180,no
T-14,M-4412,2026-11-05,Associate C,,1.5,350,525,no
T-15,M-4412,2026-11-09,Associate B,P2,2.0,400,800,no
T-16,M-4415,2026-10-21,Associate C,P1,2.0,350,700,yes
```

### 4. The matter lead's notes

```
Notes for M-4412, from Associate B, 2026-11-05

Developments:
- Due diligence closed on 16 October, a week late: the seller loaded the
  property files to the data room on 9 October instead of 25 September.
- Our second round of comments on the terms went to the seller's counsel
  on 3 November.

Risks:
- The seller has asked to add a transitional services schedule. Not in
  our scope as written; it would add negotiation time. Owner: Partner A.
- Client R's lender wants its own review of the leases before closing.

Actions:
- Ask Client R whether the transitional services schedule is in or out of
  scope, and whether a revised estimate is needed. Owner: Partner A.
  Due 2026-11-10.
- Chase the seller for the employee list. Owner: Associate C. Due 2026-11-04.
- Book the closing call with the lender.

Client decisions awaited:
- Whether to proceed with the transitional services schedule.

Other:
- Client R's finance director is on leave from 16 to 20 November.
- I think our position on the earn-out is strong and the seller will
  likely concede the cap.
```

## What came back

```
MATTER BUDGET AND STATUS SUMMARY
M-4412 Purchase of a regional bakery business | Client: Client R | Responsible partner: Partner A
As of: 2026-11-06. Prepared for: responsible partner.
Internal to the firm; not for the client.
Sources: matter plan dated 2026-11-02; time export, 16 rows, 14 used,
2 left out; notes from Associate B dated 2026-11-05.
Settings: amber share 80%; red margin 10%; schedule grace 14 days;
unbilled age 60 days; column headers default.
Defaults used for: amber share, red margin, schedule grace, unbilled age,
phase status words, billed values, column headers.

STATUS: AMBER
Budget: AMBER.
P1 Due diligence: fees to date $26,000 against a budget of $24,000, over
by $2,000
Matter: projected total $65,005 against a budget of $60,000, over by
$5,005 (8%), within the red margin of 10%
Schedule: GREEN. No rule applies.
Responsible partner's view: none given.
Developments: Due diligence closed on 16 October, a week late: the seller
loaded the property files to the data room on 9 October instead of 25
September.
Our second round of comments on the terms went to the seller's counsel on
3 November.
Client R's finance director is on leave from 16 to 20 November.

SCOPE
Fee arrangement: hourly, against an agreed estimate. Matter budget:
$60,000, last agreed with the client 2026-08-28.
In scope: due diligence on the target business; negotiating the purchase
terms with the seller's counsel; closing and the post-closing list.
Out of scope: tax structuring; employee matters; the client's financing
with its lender.

PHASES AND TIMELINE
P1 Due diligence | planned 2026-09-01 to 2026-10-09 | complete, completed
  2026-10-16 | finished 7 days after plan
P2 Negotiation of terms | planned 2026-10-05 to 2026-11-13 | in progress |
  on plan
P3 Closing and post-closing | planned 2026-11-16 to 2026-12-11 | not
  started | not yet due to start

BUDGET AGAINST FEES TO DATE
P1 Due diligence | budget $24,000 | fees to date $26,000 (108%) |
  estimate to complete $0 | projected $26,000 | over by $2,000
P2 Negotiation of terms | budget $22,000 | fees to date $15,300 (70%) |
  estimate to complete $9,000 | projected $24,300 | over by $2,300
P3 Closing and post-closing | budget $14,000 | fees to date $180 (1%) |
  estimate to complete $14,000 | projected $14,180 | over by $180
Not coded to a phase | fees to date $525 | projected $525
Matter | budget $60,000 | fees to date $42,005 (70%) | estimate to
  complete $23,000 | projected $65,005 | over by $5,005
Billed $34,000; unbilled $8,005. Unbilled older than 60 days:
T-02, 2026-09-03, Associate B, $1,200, 64 days.
Tie-out: 14 entries used, $42,005 = phases $41,480 + not coded $525.
Billed $34,000 + unbilled $8,005 = $42,005.

TEAM TIME TO DATE
Associate B | 52.0 h | $20,800
Partner A | 18.0 h | $10,800
Associate C | 21.5 h | $7,525
Paralegal D | 16.0 h | $2,880
Total | 107.5 h | $42,005

RISKS
From the notes:
- The seller has asked to add a transitional services schedule. Not in
  our scope as written; it would add negotiation time. | owner: Partner A
- Client R's lender wants its own review of the leases before closing. |
  owner not assigned
From the records:
- Unbilled time older than 60 days: T-02, $1,200.
- Phases not complete with no estimate to complete: none.

NEXT ACTIONS
- Book the closing call with the lender. | owner not assigned | due: date
  not set
- Chase the seller for the employee list. | owner: Associate C | due:
  2026-11-04 | past due
- Ask Client R whether the transitional services schedule is in or out of
  scope, and whether a revised estimate is needed. | owner: Partner A |
  due: 2026-11-10
Waiting on the client:
- Whether to proceed with the transitional services schedule.

QUESTIONS FOR THE RESPONSIBLE PARTNER
1. P1 Due diligence is complete at $26,000 against its budget of $24,000,
   over by $2,000. The notes say the seller loaded the property files on
   9 October instead of 25 September. How do you want the overrun on P1
   handled?
2. The projected total is $65,005 against the $60,000 budget last agreed
   on 2026-08-28, over by $5,005 (8%), using the estimates to complete in
   the plan: P2 is projected at $24,300 against $22,000 and P3 at $14,180
   against $14,000. How do you want the projected overrun handled?
3. The risk "Client R's lender wants its own review of the leases before
   closing" has no owner. Who owns it?
4. The action "Book the closing call with the lender" has no owner and no
   due date. Who takes it, and by when?

CHECKS ON THE RECORDS (for the billing coordinator)
- T-15: after the as-of date (2026-11-09, Associate B, $800); not counted.
- T-16: other matter (M-4415, Associate C, $700); not counted.
- T-13: coded to P3 Closing and post-closing, which the plan marks not
  started (2026-11-05, Paralegal D, $180); counted under P3.
- T-14: no phase code (2026-11-05, Associate C, $525); counted under Not
  coded to a phase.

LEFT OUT
1 note line giving a view on the merits, the likely outcome or strategy,
under Other, was not reported.

Prepared from the records named above. Nothing was sent, billed or changed
in the matter plan or the billing system.
```

How the figures were reached. P1 is the sum of T-01 to T-07: $2,400 + $1,200 + $8,800 + $2,700 + $4,200 + $4,000 + $2,700 = $26,000. P2 is T-08 to T-12: $3,600 + $5,600 + $2,800 + $2,100 + $1,200 = $15,300. P3 is T-13, $180, and the not-coded line is T-14, $525. Billed is the eight rows marked yes among the fourteen used. The matter's fees to date are 70% of its budget, under the 80% amber share, so that rule does not apply; the two budget rules that do apply set the status to amber. P1 finished on 2026-10-16 against a planned end of 2026-10-09, seven days after plan, which the schedule rules do not rate because the phase is complete. Of the two lines under Other in the notes, the first gives no view on the merits and is printed under Developments; the second is left out and counted under LEFT OUT.

What happens next belongs to the firm's people: Partner A settles the four questions, and the billing coordinator answers the four checks in the billing system. The summary itself sent nothing and changed nothing.
