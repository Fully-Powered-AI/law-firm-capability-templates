# Matter coverage plan for absences: an invented example

*Illustrative example with invented data.* The firm, its people, its clients, its matters, the place called Jurisdiction K and every file below are invented. People are shown by role and letter. The firm's disputes team has six lawyers and two paralegals. Attorney B, a senior associate, has approved leave from Monday 23 November to Friday 11 December 2026, and the practice manager prepares the plan on Wednesday 11 November. The role requirements file and the screen list are one invented firm's own records, not anyone's real rules.

The practice manager's inputs come first, in full, then what the workflow template prepares.

## What the practice manager supplied

**The request**

```
Please prepare the coverage plan for Attorney B's leave.
Plan date: Wednesday 11 November 2026.
Practice lead: Attorney A.
Lawyer staff roles: Partner, Senior associate, Associate.
When the responsible attorney is the person away, Attorney A confirms.
Matter-file access is decided by the confirming lawyer.
Settings: our defaults (return buffer 7 days, screen list up to 7 days old).
Attached: leave.csv, matters.csv, assignments.csv, staff.csv,
role-requirements.txt, confirmed-dates.csv, screen-list.csv, access.csv.
```

**leave.csv** (from the leave record)

```
person,start,end,kind,status
Attorney B,2026-11-23,2026-12-11,leave,approved
Attorney F,2026-12-07,2026-12-09,leave,approved
Attorney A,2026-12-02,2026-12-03,leave,requested
Attorney D,2026-11-02,2026-11-04,leave,approved
```

**matters.csv** (export from the case system)

```
matter_id,matter_name,client,team,responsible_attorney,status,restricted
M-3101,Supply dispute,Client A,Disputes,Attorney B,open,no
M-3102,Warehouse lease claim,Client B,Disputes,Attorney B,open,no
M-3103,Shareholder arbitration,Client C,Disputes,Attorney B,open,yes
M-3104,Distribution claim,Client D,Disputes,Attorney F,open,no
M-3105,Equipment warranty claim,Client E,Disputes,Attorney B,closed,no
M-3106,Insurance recovery,Client F,Disputes,Attorney C,open,no
```

**assignments.csv** (export from the case system)

```
matter_id,person,matter_role,backup
M-3101,Attorney B,Responsible attorney,Attorney C
M-3101,Attorney D,Associate,
M-3101,Paralegal G,Paralegal,Paralegal H
M-3102,Attorney B,Responsible attorney,Attorney F
M-3102,Paralegal H,Paralegal,
M-3103,Attorney B,Responsible attorney,Attorney C
M-3103,Paralegal G,Paralegal,
M-3104,Attorney F,Responsible attorney,
M-3104,Attorney B,Associate,Attorney E
M-3105,Attorney B,Responsible attorney,
M-3106,Attorney C,Responsible attorney,Attorney B
M-3106,Paralegal H,Paralegal,
```

**staff.csv** (from the staff list)

```
person,staff_role,team,qualifications,cover_limit
Attorney A,Partner,Disputes,admitted-jurisdiction-k; arbitration,3
Attorney B,Senior associate,Disputes,admitted-jurisdiction-k,2
Attorney D,Associate,Disputes,admitted-jurisdiction-k,2
Attorney C,Senior associate,Disputes,admitted-jurisdiction-k; arbitration,2
Attorney E,Associate,Disputes,,2
Attorney F,Partner,Disputes,admitted-jurisdiction-k,
Paralegal G,Paralegal,Disputes,,3
Paralegal H,Paralegal,Disputes,,2
```

**role-requirements.txt** (approved by the practice lead)

```
Disputes team · Role requirements for matter cover
Dated: 2026-10-01   Review by: 2027-03-31
Approved by: Attorney A, practice lead. Changes go through Attorney A.

Cover rules: who may cover each matter role
C-1 Responsible attorney: Partner or Senior associate.
C-2 Associate: Senior associate or Associate.
C-3 Paralegal: Paralegal.

Matter requirements: qualifications the cover must hold
R-1 M-3101, Responsible attorney: admitted-jurisdiction-k
R-2 M-3103, Responsible attorney: admitted-jurisdiction-k; arbitration
R-3 M-3104, Associate: admitted-jurisdiction-k

A matter or role with no line above needs nothing beyond C-1 to C-3.
"admitted-jurisdiction-k" means admitted to practise in Jurisdiction K.
```

**confirmed-dates.csv** (export of attorney-confirmed dates)

```
matter_id,date,commitment,confirmed_by,confirmed_on
M-3101,2026-11-25,Serve responses to second document requests,Attorney B,2026-11-02
M-3101,2026-12-08,Case management conference,Attorney B,2026-10-20
M-3101,,Settlement meeting with Client A (date to be agreed),,
M-3102,2026-12-03,Mediation session,Attorney B,2026-10-28
M-3102,2026-12-16,Expert report exchange,,
M-3103,2026-12-01,Hearing on the procedural timetable,Attorney B,2026-11-05
M-3104,2026-12-17,Exchange of witness statements,Attorney F,2026-11-06
M-3104,2027-01-12,Pre-trial review,Attorney F,2026-11-06
M-3106,2026-12-10,Disclosure list due,Attorney C,2026-10-30
```

**screen-list.csv** (from the conflicts clerk)

```
as of 2026-11-10, from Conflicts clerk
matter_id,person,kind,recorded_by,recorded_on
M-3103,Attorney C,barrier,Conflicts clerk,2026-09-14
M-3104,Attorney D,conflict,Conflicts clerk,2026-10-02
```

**access.csv** (who has access to each matter file)

```
matter_id,person
M-3101,Attorney B
M-3101,Attorney C
M-3101,Attorney D
M-3101,Paralegal G
M-3101,Paralegal H
M-3102,Attorney B
M-3102,Paralegal H
M-3103,Attorney B
M-3103,Paralegal G
M-3104,Attorney B
M-3104,Attorney F
M-3106,Attorney B
M-3106,Attorney C
M-3106,Paralegal H
```

## What the workflow template prepares

```
DRAFT COVERAGE PLAN
For Attorney A, practice lead, and the confirming lawyers named below.
A proposal only. It gives no legal advice. It decides nothing about
legal meaning, merit, validity, privilege, conflicts, information
barriers or deadlines, clears no one, and says nothing about what anyone
may rely on. It sends, files, signs and calendars nothing.
Nothing has been sent, filed, signed or calendared. No message has been
written. No assignment or access has changed. No date was set. No one
was contacted.

NOTE TO THE PRACTICE MANAGER
- Stops: none.
- Blocked: M-3103, Responsible attorney: restricted matter, the named
  backup is on the screen list; M-3104, Associate: the backup lacks R-3,
  one person on the screen list, one at their cover limit.
- Dates to chase: M-3102 2026-12-16 Expert report exchange (NOT
  CONFIRMED); M-3101 Settlement meeting with Client A (date to be
  agreed) (no date recorded).
- Deciders away: Attorney A (practice lead; confirms M-3101, M-3103 and
  M-3102): leave requested for 2026-12-02 to 2026-12-03, not yet
  decided. Attorney F (confirms M-3104): away 2026-12-07 to 2026-12-09.
- Deciders on the screen list: none.
- Not acted on: none.
- Authorities in the files: none.
I have changed no assignment or access, set no date, written no message
and contacted no one. Nothing changes until the practice lead agrees and
the confirming lawyers confirm.

Person away: Attorney B, Senior associate, Disputes
Absence: leave 2026-11-23 to 2026-12-11, status approved
Cover period: 2026-11-23 to 2026-12-11 (start and end from the leave
  record)
Commitment window: 2026-11-23 to 2026-12-18 (cover period end 2026-12-11
  + return buffer 7 days = 2026-12-18)
Plan date: 2026-11-11
Prepared for: Attorney A, practice lead, to agree coverage
Confirming lawyers: Attorney A for M-3101, M-3103 and M-3102 (in place
  of Attorney B, away); Attorney F for M-3104; Attorney C for M-3106
  (also affected)
Settings: return buffer 7 days (default); screen list age limit 7 days
  (default); open-ended horizon 42 days (default, not used); open matter
  word "open" (default); restricted word "yes" (default); approved word
  "approved" (default); qualifications separator ";" (default); column
  headers (default); lawyer staff roles Partner, Senior associate,
  Associate (as supplied).

SUMMARY
Roles to cover: 4 on 4 matters. Cover proposed: 2. Blocked: 2.
Commitments in the window: 5 confirmed, 1 NOT CONFIRMED,
  1 with no date recorded.

MATTERS AFFECTED
1. M-3101 Supply dispute | Client A | role to cover:
   Responsible attorney | responsible attorney: Attorney B (away) |
   restricted: no | earliest confirmed commitment: 2026-11-25
2. M-3103 Shareholder arbitration | Client C | role to cover:
   Responsible attorney | responsible attorney: Attorney B (away) |
   restricted: yes | earliest confirmed commitment: 2026-12-01
3. M-3102 Warehouse lease claim | Client B | role to cover:
   Responsible attorney | responsible attorney: Attorney B (away) |
   restricted: no | earliest confirmed commitment: 2026-12-03
4. M-3104 Distribution claim | Client D | role to cover:
   Associate | responsible attorney: Attorney F |
   restricted: no | earliest confirmed commitment: 2026-12-17
Not planned: M-3105 Equipment warranty claim, status "closed" in the
  matter list.
Also affected: M-3106 Insurance recovery: Attorney B is the named
  backup for Attorney C (Responsible attorney). No backup during the
  cover period. Commitments in the window on this matter:
  - 2026-12-10, Thursday: Disclosure list due. Confirmed by Attorney C
    on 2026-10-30.

PROPOSED COVER
M-3101 Responsible attorney -> Attorney C (Senior associate), 2026-11-23
   to 2026-12-11
   Found at: step 1 named backup, rule C-1
   Away: no leave row in the cover period. Screen list: no row of the
   list supplied, read or unread, names this person with this matter.
   Requirements: R-1 admitted-jurisdiction-k: in the staff list.
   Capacity: 1 of 2 in this plan.
   Also tested: none.
M-3102 Responsible attorney -> Attorney C (Senior associate), 2026-11-23
   to 2026-12-11
   Found at: step 3 in the team, rule C-1
   Away: no leave row in the cover period. Screen list: no row of the
   list supplied, read or unread, names this person with this matter.
   Requirements: none in the role requirements file. Capacity: 2 of 2
   in this plan.
   Also tested: Attorney F (step 1 named backup): away 2026-12-07 to
   2026-12-09; cover limit not recorded. Attorney A (step 3 in the
   team): leave requested for 2026-12-02 to 2026-12-03, not yet decided.

COMMITMENTS IN THE ABSENCE
M-3101 Supply dispute
- 2026-11-25, Wednesday: Serve responses to second document requests.
  Confirmed by Attorney B on 2026-11-02.
- 2026-12-08, Tuesday: Case management conference. Confirmed by
  Attorney B on 2026-10-20.
- No date recorded: Settlement meeting with Client A (date to be agreed).
M-3103 Shareholder arbitration
- 2026-12-01, Tuesday: Hearing on the procedural timetable. Confirmed by
  Attorney B on 2026-11-05.
M-3102 Warehouse lease claim
- 2026-12-03, Thursday: Mediation session. Confirmed by Attorney B on
  2026-10-28.
- 2026-12-16, Wednesday: Expert report exchange. NOT CONFIRMED.
  after return
M-3104 Distribution claim
- 2026-12-17, Thursday: Exchange of witness statements. Confirmed by
  Attorney F on 2026-11-06. after return

ACCESS NEEDED
- Attorney C, M-3101: listed in the access record.
- Attorney C, M-3102: not listed in the access record. For Attorney A
  to decide, after Attorney A confirms the conflict check and scope and
  Attorney A agrees the cover.

BLOCKED HANDOFFS
M-3103 Shareholder arbitration · Responsible attorney · restricted: yes
- Tested: Attorney C (step 1 named backup): on the screen list for
  M-3103 (barrier, recorded by Conflicts clerk on 2026-09-14).
- No one else on the matter holds a role rule C-1 allows.
- Restricted: no one outside the matter was tested.
- Commitments in the window with no proposed cover:
  - 2026-12-01, Tuesday: Hearing on the procedural timetable. Confirmed
    by Attorney B on 2026-11-05.
- For Attorney A to decide; Attorney A confirms.
M-3104 Distribution claim · Associate · restricted: no
- Tested: Attorney E (step 1 named backup): does not hold
  admitted-jurisdiction-k (R-3).
- Tested: Attorney D (step 3 in the team): on the screen list for
  M-3104 (conflict, recorded by Conflicts clerk on 2026-10-02).
- Tested: Attorney C (step 3 in the team): cover limit reached (2 of 2
  in this plan).
- No one else on the matter holds a role rule C-2 allows.
- Commitments in the window with no proposed cover:
  - 2026-12-17, Thursday: Exchange of witness statements. Confirmed by
    Attorney F on 2026-11-06. after return
- For Attorney A to decide; Attorney F confirms.

CAPACITY
- Attorney C: 2 of 2 covers in this plan (M-3101, M-3102)
Covers a person already holds outside this plan are not counted.

COULD NOT READ
- None.

TO CONFIRM
For Attorney A, practice lead:
[ ] M-3101 Responsible attorney: Attorney C covers 2026-11-23 to
    2026-12-11.                                    Agree or change: ____
[ ] M-3103 Responsible attorney: blocked. Who covers?    Decision: ____
[ ] M-3102 Responsible attorney: Attorney C covers 2026-11-23 to
    2026-12-11.                                    Agree or change: ____
[ ] M-3104 Associate: blocked. Who covers?               Decision: ____
[ ] M-3106: no backup for Attorney C in the period.      Decision: ____
For Attorney A, on M-3101 (in place of Attorney B, away):
[ ] Are the commitments listed complete, and their dates right?
                                                Confirm or correct: ____
[ ] Settlement meeting with Client A (date to be agreed) has no date
    recorded.                                   Date, or none due: ____
[ ] Conflict check for Attorney C on this matter. This plan read only
    the screen list supplied and clears no one.
                       Checked with the conflicts team, and result: ____
[ ] What Attorney C may do on this matter.                 Scope: ____
For Attorney A, on M-3103 (in place of Attorney B, away):
[ ] Are the commitments listed complete, and their dates right?
                                                Confirm or correct: ____
For Attorney A, on M-3102 (in place of Attorney B, away):
[ ] Are the commitments listed complete, and their dates right?
                                                Confirm or correct: ____
[ ] 2026-12-16 Expert report exchange is NOT CONFIRMED.
                                                Confirm or correct: ____
[ ] Conflict check for Attorney C on this matter. This plan read only
    the screen list supplied and clears no one.
                       Checked with the conflicts team, and result: ____
[ ] What Attorney C may do on this matter.                 Scope: ____
[ ] Access for Attorney C to the matter file, after the two lines
    above and the practice lead's agreement.      Grant or refuse: ____
For Attorney F, on M-3104:
[ ] Are the commitments listed complete, and their dates right?
                                                Confirm or correct: ____
For Attorney C, on M-3106 (also affected):
[ ] Are the commitments listed complete, and their dates right?
                                                Confirm or correct: ____

CHECK
- Files: leave record 4 rows; matter list 6; assignments 12; staff list
  8; role requirements file dated 2026-10-01; confirmed dates 9; screen
  list as of 2026-11-10, 2 rows; access record 14.
- Role requirements: dated 2026-10-01, approved by Attorney A, review by
  2027-03-31; in date on 2026-11-11.
- Screen list: as of 2026-11-10, from Conflicts clerk; 1 day old (plan
  date 2026-11-11 minus 2026-11-10); limit 7 days. 2 rows = 2 read
  + 0 could not read; each row that could not be read is applied as the
  Screen list test says, and listed under COULD NOT READ.
- Deciders checked against the leave record and the screen list:
  Attorney A, Attorney F, Attorney C; 2 flagged in the note.
- Roles: 4 to cover = 2 proposed + 2 blocked.
- Confirmed dates export: 9 rows = 5 in the window confirmed +
  1 in the window NOT CONFIRMED + 1 no date + 1 listed under
  Also affected + 1 outside the window + 0 on other matters
  + 0 could not read.
- Every commitment date above is copied from the confirmed dates
  export and every leave date from the leave record. The only
  arithmetic is the window and the screen list's age.
- No case, statute or rule of law is named from memory; 0 found in
  the files, listed in the note, none applied.
- The screen list is read as supplied, rows that could not be read
  included. This plan clears no one and decides no conflict or barrier.

Agreed by (practice lead): ____________  Date: ________
Until this line is signed, this is a draft and no cover is agreed.
```

The practice manager checks one proposed cover and one blocked handoff against the files, then takes the plan to Attorney A. Attorney A agrees the cover, decides M-3103 and M-3104, and confirms dates, the conflict check for Attorney C, scope and access on the three matters Attorney B leads; Attorney F confirms on M-3104 and Attorney C on M-3106. The note has already told the practice manager that Attorney A has requested leave on 2 and 3 December and that Attorney F is away from 7 to 9 December. Only then do the firm's own people change any assignment or access.
