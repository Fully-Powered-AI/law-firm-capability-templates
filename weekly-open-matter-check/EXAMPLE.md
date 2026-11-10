# Weekly open-matter check: an invented example

*Illustrative example with invented data.* The firm, its people, its clients, its matters and every record below are invented. People are shown by role. The firm is a small practice with three attorneys and two paralegals; its operations manager runs the check on Monday 2 November 2026.

## What the operations manager supplied

**The request**

```
Run the weekly open-matter check as of Monday 2 November 2026.
Attached: roster.csv from the billing coordinator, and this morning's two
exports from the case system, matters.csv and tasks.csv.
Our settings: the roster may be up to 7 days old; the attention list holds
at most 10 matters; open tasks have the status "open" and finished tasks
"done". Use the standard note layout and sign the notes "Operations manager".
The summary goes to the managing partner.
```

**roster.csv** (from billing: every matter the firm is billing)

```
matter_id,client,responsible_attorney,roster_as_of
M-201,Client A,Attorney A,2026-11-02
M-202,Client B,Attorney B,2026-11-02
M-203,Client C,Attorney A,2026-11-02
M-204,Client D,Attorney C,2026-11-02
M-205,Client E,Attorney B,2026-11-02
M-206,Client F,Attorney C,2026-11-02
M-207,Client G,Attorney A,2026-11-02
```

**matters.csv** (export from the case system)

```
id,name,client,responsible_attorney,status
M-201,Supply dispute,Client A,Attorney A,open
M-202,Lease renewal,Client B,Attorney B,open
M-203,Insurance claim,Client C,Attorney A,open
M-204,Property boundary dispute,Client D,Attorney C,open
M-205,Regulatory inquiry,Client E,Attorney B,open
M-207,Partnership dissolution,Client G,Attorney A,open
M-208,Estate administration,Client H,Attorney C,open
```

**tasks.csv** (export from the case system)

```
id,matter_id,title,owner,due,status
T-01,M-201,File reply brief,,2026-10-23,open
T-02,M-201,Prepare exhibit list,Paralegal 1,2026-10-28,open
T-03,M-201,Send client status letter,Attorney A,2026-11-13,open
T-04,M-201,Collect signed engagement letter,Paralegal 1,2026-09-18,done
T-05,M-202,Request landlord's ledger,Paralegal 2,2026-10-30,open
T-06,M-202,Schedule client call,,2026-11-06,open
T-07,M-203,Send client status letter,Paralegal 1,,open
T-08,M-203,Order adjuster's file,Paralegal 2,2026-11-02,open
T-09,M-205,Assemble document production,Paralegal 2,2026-10-19,open
T-10,M-205,Calendar response date,Attorney B,2026-11-09,open
T-11,M-207,Close out file index,Paralegal 1,2026-10-09,done
T-12,M-207,Return original documents,Paralegal 1,2026-10-16,done
T-13,M-208,Request account statements,,2026-11-10,open
```

## What came back

```
WEEKLY OPEN-MATTER CHECK as of 2026-11-02
Input: export (matters.csv, 7 matters; tasks.csv, 13 tasks).
Roster: dated 2026-11-02, from the billing coordinator, 7 matters, 0 days old
(check date 2026-11-02 minus roster date 2026-11-02 = 0 days; limit 7 days).
Settings: roster age limit 7 days; list size 10; status words open/done;
column headers default.
Defaults used for: column headers.

Coverage: expected 7 open matters per roster dated 2026-11-02 (billing
coordinator); assessed 6 of them; could not assess 1: M-206, Client F,
Attorney C (on the roster, not in the matters export).
In the system but not on the roster: M-208, Estate administration, Client H
(assessed).
On the roster with a status other than open in the system: none.

Outcome: partial. One roster matter, M-206, could not be assessed.

Totals: 7 matters assessed (6 on the roster, 1 not on it); 10 open tasks;
4 overdue; 3 unowned; 1 with no due date. 3 finished tasks were left out.

MATTERS ASSESSED
M-201 Supply dispute | Attorney A | open 3 | overdue 2 | unowned 1 |
  no due date 0 | earliest open due 2026-10-23
M-202 Lease renewal | Attorney B | open 2 | overdue 1 | unowned 1 |
  no due date 0 | earliest open due 2026-10-30
M-203 Insurance claim | Attorney A | open 2 | overdue 0 | unowned 0 |
  no due date 1 | earliest open due 2026-11-02
M-204 Property boundary dispute | Attorney C | open 0 | overdue 0 |
  unowned 0 | no due date 0 | earliest open due none | no tasks recorded
M-205 Regulatory inquiry | Attorney B | open 2 | overdue 1 | unowned 0 |
  no due date 0 | earliest open due 2026-10-19
M-207 Partnership dissolution | Attorney A | open 0 | overdue 0 |
  unowned 0 | no due date 0 | earliest open due none | no open tasks
M-208 Estate administration | Attorney C | open 1 | overdue 0 | unowned 1 |
  no due date 0 | earliest open due 2026-11-10 | not on the roster
Not assessed, not open in the system and not on the roster: none.

COULD NOT ASSESS
- M-206, Client F, Attorney C: on the roster, not in the matters export

COULD NOT READ
- none
Tasks for a matter that is not in the matters export, counted nowhere: none.

ATTENTION LIST (4 of at most 10)
1. M-201 Supply dispute (Attorney A): 2 overdue, 1 unowned
2. M-202 Lease renewal (Attorney B): 1 overdue, 1 unowned
3. M-205 Regulatory inquiry (Attorney B): 1 overdue, 0 unowned
4. M-208 Estate administration (Attorney C): 0 overdue, 1 unowned
Rule: matters with at least one overdue or unowned task; most overdue
first; then most unowned; then the earliest open due date; then matter ID.
Client size plays no part.

DRAFT NOTES

DRAFT, not sent
To: Attorney A
Subject: M-201 Supply dispute (Client A): tasks needing attention as of
2026-11-02
I am going through the open matters as of 2026-11-02. On M-201:
Overdue:
- File reply brief (T-01), no owner: due 2026-10-23; check date 2026-11-02;
  10 days late
- Prepare exhibit list (T-02), Paralegal 1: due 2026-10-28; check date
  2026-11-02; 5 days late
Who is taking these, and when will they be done?
Operations manager

DRAFT, not sent
To: Attorney B
Subject: M-202 Lease renewal (Client B): tasks needing attention as of
2026-11-02
I am going through the open matters as of 2026-11-02. On M-202:
Overdue:
- Request landlord's ledger (T-05), Paralegal 2: due 2026-10-30; check date
  2026-11-02; 3 days late
Not yet due, no owner:
- Schedule client call (T-06), due 2026-11-06
Who is taking these, and when will they be done?
Operations manager

DRAFT, not sent
To: Attorney B
Subject: M-205 Regulatory inquiry (Client E): tasks needing attention as of
2026-11-02
I am going through the open matters as of 2026-11-02. On M-205:
Overdue:
- Assemble document production (T-09), Paralegal 2: due 2026-10-19; check
  date 2026-11-02; 14 days late
Who is taking this, and when will it be done?
Operations manager

DRAFT, not sent
To: Attorney C
Subject: M-208 Estate administration (Client H): tasks needing attention as
of 2026-11-02
I am going through the open matters as of 2026-11-02. On M-208:
Not yet due, no owner:
- Request account statements (T-13), due 2026-11-10
Who is taking this, and when will it be done?
Operations manager

DRAFT SUMMARY

DRAFT, not sent
To: Managing partner
Subject: Weekly open-matter check as of 2026-11-02
Coverage: expected 7 open matters per roster dated 2026-11-02 (billing
coordinator); assessed 6 of them; could not assess 1: M-206, Client F,
Attorney C (on the roster, not in the matters export).
In the system but not on the roster: M-208, Estate administration, Client H
(assessed).
On the roster with a status other than open in the system: none.
Totals: 7 matters assessed (6 on the roster, 1 not on it); 10 open tasks;
4 overdue; 3 unowned; 1 with no due date. 3 finished tasks were left out.
The matters that most need attention (4):
1. M-201 Supply dispute (Attorney A): 2 overdue, 1 unowned
2. M-202 Lease renewal (Attorney B): 1 overdue, 1 unowned
3. M-205 Regulatory inquiry (Attorney B): 1 overdue, 0 unowned
4. M-208 Estate administration (Attorney C): 0 overdue, 1 unowned
Could not assess: M-206, Client F, Attorney C.
Could not read: none.
Also on the sheet: M-204 has no tasks recorded; M-207 has no open tasks;
M-203 has a task with no due date (T-07).
I am writing to the responsible attorney on each matter on the list.
Operations manager

FOR THE OPERATIONS MANAGER
- Find M-206 (Client F, Attorney C). It is on the billing roster and not in
  the matters export.
- Ask the billing coordinator about M-208 (Estate administration, Client H),
  which is open in the case system and not on the roster.
- M-204 has no tasks recorded, and M-207 has only finished tasks. Neither is
  shown as clear.
- T-07 on M-203 has no due date. M-203 is not on the attention list, so no
  note was drafted; Attorney A sets the date.
- T-08 on M-203 is due on the check date and is not overdue.

Nothing was sent and nothing in the case system was changed.
```

The operations manager read the four drafts, sent them from their own email, and went to find M-206. The days late in each note are plain calendar days, shown with their working so the attorney can confirm or correct them. The three files use the column headers the template expects by default; a firm whose files are headed differently says so in its settings, and the check stops and asks if it meets a header it was not told about.
