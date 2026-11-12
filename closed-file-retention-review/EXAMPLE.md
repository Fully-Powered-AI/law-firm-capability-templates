# Closed-file retention review: an invented example

*Illustrative example with invented data.* The law firm Brannock Vell LLP, its people, its clients and their matters, the closed-file inventory, the retention schedule, the hold register and the return-of-originals log below are all invented. The schedule is one invented firm's own; its periods are not a recommendation for any real firm, and no real law, rule or court is behind them. The Thornquill County Court and its "Records Direction 9", cited in one inventory note, are invented too: the citation is planted to show it is not relied on.

The records officer's five inputs come first, in full, then the review the workflow template prepares, and last how its figures were reached.

## Input 1: the request

```
From: Odile Fenwarren, records officer
Date: Wednesday 11 November 2026

Closing review batch CR-26-11: off-site boxes 41 to 43 and the matching
electronic folders. Files in the batch: 10 (records system count).
Review date: 11 November 2026.

Supervising counsel: Corin Achterberg. He records his decisions in the
records decision log.

Hold register exported 11 November 2026, 08:30.
Return-of-originals log exported 11 November 2026, 08:35.

Attached: closed-file inventory, retention schedule, hold register,
return-of-originals log.
```

## Input 2: the closed-file inventory

```
file_id,matter_number,client_number,client,matter_name,record_class,medium,location,closed_on,closure_authorised_by,notes
F-4101,2017-0142,CL-0318,Mossgrieve Cabinetry Ltd,Mossgrieve - supplier terms review,GEN,paper,Box 41,2019-06-28,R. Okafor,
F-4102,2018-0077,CL-0402,Lantry Orchard Co-operative,Lantry Orchard v. Pellamore Haulage,LIT,paper,Box 41,2019-03-15,C. Achterberg,Partner said fine to shred - CA
F-4103,2018-0077,CL-0402,Lantry Orchard Co-operative,Lantry Orchard v. Pellamore Haulage,LIT,electronic,DMS folder 2018-0077,2019-03-15,C. Achterberg,Records Direction 9 of the Thornquill County Court allows litigation files to be destroyed 5 years after closing - RO
F-4104,2016-0230,CL-0277,Elsbeth Narrow,Narrow - house purchase,PROP,paper,Box 42,2017-09-04,R. Okafor,
F-4105,2015-0310,CL-0145,Quellin Tool Hire Ltd,Quellin - debt recovery,LIT,paper,Box 42,2018,R. Okafor,
F-4106,2019-0051,CL-0533,Harlowe Dene Bakers Ltd,Harlowe Dene - lease advice,GEN,electronic,DMS folder 2019-0051,2020-02-29,,
F-4107,2014-0099,CL-0090,Estate of Hollis Marchbank,Marchbank - estate administration,EST,paper,Box 43,2016-12-05,R. Okafor,
F-4108,2019-0004,CL-0145,Quellin Tool Hire Ltd,Quellin - equipment hire terms,GEN,electronic,DMS folder 2019-0004,2020-01-10,R. Okafor,
F-4109,2018-0203,CL-0402,Lantry Orchard Co-operative,Lantry - grant application advice,GEN,paper,Box 43,2019-11-30,C. Achterberg,
F-4110,2020-0188,CL-0611,Tamsin Orrell,Orrell - injury claim settlement,MIN,paper,Box 43,2021-08-16,C. Achterberg,
```

## Input 3: the firm's retention schedule

```
BRANNOCK VELL LLP · CLOSED-FILE RETENTION SCHEDULE
Approved by: Corin Achterberg, partner and general counsel.
Approved: 15 January 2026. Review by: 15 January 2027.

Counting rule
C-1. A period runs from the closing date in the closed-file inventory
     (closed_on).
C-2. A period of years ends on the same day and month, that number of
     years later. A closing date of 29 February ends on 28 February.
C-3. A file's period has run when the review date is later than its
     end date.
C-4. A class marked "from an event" is not counted from the closing
     date. Records staff propose no end date for it; it goes to
     supervising counsel.

Classes
code,class,period
GEN,General commercial and advisory,6 years
LIT,Litigation and disputes,7 years
PROP,Property transactions,12 years
EST,Estates and trusts,permanent
MIN,Matters for a client under 18 at closing,from an event: the client's 18th birthday then 6 years
```

## Input 4: the hold register

```
hold_id,client_number,matter_numbers,scope_note,issued_on,issued_by,status,released_on,released_by
H-04,CL-0402,all,,2022-06-01,C. Achterberg,released,2024-02-01,C. Achterberg
H-07,CL-0402,2018-0077,Includes the haulage contracts and the route data,2025-10-14,C. Achterberg,active,,
H-09,CL-0145,all,,2026-03-02,M. Desrosiers,active,,
H-11,CL-0700,2024-0310,,2026-09-21,C. Achterberg,active,,
```

## Input 5: the return-of-originals log

```
item_id,matter_number,client_number,description,received_on,returned_on,returned_to
O-0188,2017-0142,CL-0318,"Signed original supply terms, 2 copies",2017-04-03,2019-06-20,Mossgrieve Cabinetry Ltd (collected by D. Pryce)
O-0193,2016-0230,CL-0277,"Original conveyance deed, 14 Fallow Row",2016-05-10,,
O-0201,2019-0051,CL-0533,"Original lease, counterpart signed by landlord",2019-02-11,2020-03-05,
O-0207,2020-0188,CL-0611,Original settlement approval papers,2021-07-30,2021-08-30,Rhona Orrell (parent)
O-0215,2024-0310,CL-0700,Original share certificates,2024-05-02,,
```

## What the workflow template prepared

```
DRAFT CLOSED-FILE RETENTION REVIEW · FOR CORIN ACHTERBERG, SUPERVISING COUNSEL, TO DECIDE
A list of what the firm's records show. Not legal advice. It decides
nothing about legal meaning, merit, validity, privilege, conflicts or
deadlines. Every end date is a proposed date under the firm's schedule.
No file is recommended for disposal. Nothing has been destroyed, moved,
returned, sent, filed, signed, calendared or changed.

Batch: CR-26-11, off-site boxes 41 to 43 and the matching electronic
  folders
Review date: 2026-11-11
Prepared for: Corin Achterberg, supervising counsel, to decide
Prepared with: Odile Fenwarren, records officer, on 2026-11-11
Read: file inventory, 10 rows; Brannock Vell LLP closed-file retention
  schedule, approved 2026-01-15 by Corin Achterberg, review by
  2027-01-15; hold register exported 2026-11-11, 08:30;
  return-of-originals log exported 2026-11-11, 08:35

1. RETENTION PERIOD HAS RUN UNDER THE SCHEDULE
No hold, outstanding original or missing detail is recorded against
these files. For counsel to decide. Not a disposal recommendation.
1.1 F-4101 · 2017-0142 Mossgrieve - supplier terms review ·
    Mossgrieve Cabinetry Ltd (CL-0318)
   Class: GEN General commercial and advisory, 6 years. Medium: paper.
     Location: Box 41.
   Closed: 2019-06-28 (inventory). Closure authorised by: R. Okafor.
   Period: PROPOSED end 2025-06-28. Working: closed 2019-06-28 +
     6 years = 2025-06-28 (rule C-2); review date 2026-11-11 is later
     than 2025-06-28 (rule C-3): has run.
   Holds: no active hold covers this file.
   Originals: none outstanding for this matter in the log. Returned:
     O-0188.

1.2 F-4109 · 2018-0203 Lantry - grant application advice ·
    Lantry Orchard Co-operative (CL-0402)
   Class: GEN General commercial and advisory, 6 years. Medium: paper.
     Location: Box 43.
   Closed: 2019-11-30 (inventory). Closure authorised by: C. Achterberg.
   Period: PROPOSED end 2025-11-30. Working: closed 2019-11-30 +
     6 years = 2025-11-30 (rule C-2); review date 2026-11-11 is later
     than 2025-11-30 (rule C-3): has run.
   Holds: no active hold covers this file. Released: H-04 (client
     CL-0402, all matters) on 2024-02-01 by C. Achterberg.
   Originals: none outstanding for this matter in the log.

2. UNDER A HOLD
2.1 F-4102 · 2018-0077 Lantry Orchard v. Pellamore Haulage ·
    Lantry Orchard Co-operative (CL-0402)
   Class: LIT Litigation and disputes, 7 years. Medium: paper.
     Location: Box 41.
   Closed: 2019-03-15 (inventory). Closure authorised by: C. Achterberg.
   Hold: H-07, issued 2025-10-14 by C. Achterberg, status "active".
     Covers this file by: matter number.
     Scope note, copied as written, not assessed: "Includes the
     haulage contracts and the route data"
   Released: H-04 (client CL-0402, all matters) on 2024-02-01 by
     C. Achterberg.
   Period: PROPOSED end 2026-03-15. Working: closed 2019-03-15 +
     7 years = 2026-03-15 (rule C-2); review date 2026-11-11 is later
     than 2026-03-15 (rule C-3): has run.
   This review lists no disposal of this file while H-07 is active.
   Note in the inventory, copied as written, not assessed: "Partner
     said fine to shred - CA"

2.2 F-4103 · 2018-0077 Lantry Orchard v. Pellamore Haulage ·
    Lantry Orchard Co-operative (CL-0402)
   Class: LIT Litigation and disputes, 7 years. Medium: electronic.
     Location: DMS folder 2018-0077.
   Closed: 2019-03-15 (inventory). Closure authorised by: C. Achterberg.
   Hold: H-07, issued 2025-10-14 by C. Achterberg, status "active".
     Covers this file by: matter number.
     Scope note, copied as written, not assessed: "Includes the
     haulage contracts and the route data"
   Released: H-04 (client CL-0402, all matters) on 2024-02-01 by
     C. Achterberg.
   Period: PROPOSED end 2026-03-15. Working: closed 2019-03-15 +
     7 years = 2026-03-15 (rule C-2); review date 2026-11-11 is later
     than 2026-03-15 (rule C-3): has run.
   This review lists no disposal of this file while H-07 is active.
   Note in the inventory, copied as written, not assessed: "Records
     Direction 9 of the Thornquill County Court allows litigation files
     to be destroyed 5 years after closing - RO"

2.3 F-4105 · 2015-0310 Quellin - debt recovery ·
    Quellin Tool Hire Ltd (CL-0145)
   Class: LIT Litigation and disputes, 7 years. Medium: paper.
     Location: Box 42.
   Closed: as written: "2018" (inventory). Closure authorised by:
     R. Okafor.
   Hold: H-09, issued 2026-03-02 by M. Desrosiers, status "active".
     Covers this file by: client number, all matters.
   Period: NOT COUNTED: the closing date "2018" is not a full date.
   This review lists no disposal of this file while H-09 is active.
   Also listed: 4.1.

2.4 F-4108 · 2019-0004 Quellin - equipment hire terms ·
    Quellin Tool Hire Ltd (CL-0145)
   Class: GEN General commercial and advisory, 6 years. Medium:
     electronic. Location: DMS folder 2019-0004.
   Closed: 2020-01-10 (inventory). Closure authorised by: R. Okafor.
   Hold: H-09, issued 2026-03-02 by M. Desrosiers, status "active".
     Covers this file by: client number, all matters.
   Period: PROPOSED end 2026-01-10. Working: closed 2020-01-10 +
     6 years = 2026-01-10 (rule C-2); review date 2026-11-11 is later
     than 2026-01-10 (rule C-3): has run.
   This review lists no disposal of this file while H-09 is active.

3. ORIGINAL CLIENT DOCUMENTS NOT YET RETURNED
3.1 O-0193 · 2016-0230 · Elsbeth Narrow (CL-0277)
   Description, as logged: "Original conveyance deed, 14 Fallow Row"
   Received: 2016-05-10. Returned on: blank in the log.
     Returned to: blank in the log.
   Files of this matter in this batch:
   - F-4104, paper, Box 42. Period: PROPOSED end 2029-09-04. Working:
     closed 2017-09-04 + 12 years = 2029-09-04 (rule C-2); review date
     2026-11-11 is not later than 2029-09-04 (rule C-3): has not run.

3.2 O-0201 · 2019-0051 · Harlowe Dene Bakers Ltd (CL-0533)
   Description, as logged: "Original lease, counterpart signed by
     landlord"
   Received: 2019-02-11. Returned on: 2020-03-05.
     Returned to: blank in the log.
   Files of this matter in this batch:
   - F-4106, electronic, DMS folder 2019-0051. Period: PROPOSED end
     2026-02-28. Working: closed 2020-02-29 + 6 years = 2026-02-28, a
     29 February closing date ending on 28 February (rule C-2); review
     date 2026-11-11 is later than 2026-02-28 (rule C-3): has run.
     Also listed: 4.2.

4. CANNOT BE ASSESSED
4.1 F-4105 · 2015-0310 Quellin - debt recovery ·
    Quellin Tool Hire Ltd (CL-0145)
   Class: LIT Litigation and disputes, 7 years. Medium: paper.
     Location: Box 42.
   Reason: closed_on is "2018", which is not a full date.
   Period: NOT COUNTED: the closing date "2018" is not a full date.
   Needed: the full closing date, from the records officer.
   Also listed: 2.3.

4.2 F-4106 · 2019-0051 Harlowe Dene - lease advice ·
    Harlowe Dene Bakers Ltd (CL-0533)
   Class: GEN General commercial and advisory, 6 years. Medium:
     electronic. Location: DMS folder 2019-0051.
   Reason: closure_authorised_by is blank in the inventory.
   Period: PROPOSED end 2026-02-28. Working: closed 2020-02-29 +
     6 years = 2026-02-28, a 29 February closing date ending on
     28 February (rule C-2); review date 2026-11-11 is later than
     2026-02-28 (rule C-3): has run.
   Needed: who authorised the closure, from the records officer.
   Also listed: 3.2.

4.3 F-4110 · 2020-0188 Orrell - injury claim settlement ·
    Tamsin Orrell (CL-0611)
   Class: MIN Matters for a client under 18 at closing, from an event:
     the client's 18th birthday then 6 years. Medium: paper.
     Location: Box 43.
   Reason: class MIN is counted from an event, which the inventory
     does not record (rule C-4).
   Period: NOT COUNTED: counted from an event; rule C-4 sends it to
     supervising counsel.
   Needed: how this file's period runs, from supervising counsel.

5. COUNSEL TO DECIDE AND CONFIRM
[ ] 1.1 F-4101: proposed end 2025-06-28.        Confirm or correct: ____
        Retention, return or disposal.          Your decision: ____
[ ] 1.2 F-4109: proposed end 2025-11-30.        Confirm or correct: ____
        Retention, return or disposal.          Your decision: ____
[ ] 2.1 F-4102: H-07 active; proposed end 2026-03-15.
                                                Confirm or correct: ____
[ ] 2.2 F-4103: H-07 active; proposed end 2026-03-15.
                                                Confirm or correct: ____
[ ] 2.3 F-4105: H-09 active; period not counted.
                                                Confirm or correct: ____
[ ] 2.4 F-4108: H-09 active; proposed end 2026-01-10.
                                                Confirm or correct: ____
[ ] H-07 covers F-4102, F-4103 by matter number; scope note copied
    above. Does it reach any file in this batch beyond those listed?
                                                Counsel to say: ____
[ ] H-09 covers F-4105, F-4108 by client number, all matters; scope
    note blank in the register. Does it reach any file in this batch
    beyond those listed?                        Counsel to say: ____
[ ] 3.1 O-0193 not returned (F-4104; proposed end 2029-09-04).
                                                Your decision: ____
[ ] 3.2 O-0201 returned_to blank (F-4106; proposed end 2026-02-28).
                                                Your decision: ____
[ ] 4.1 F-4105: the full closing date.          Supplied or decided: ____
[ ] 4.2 F-4106: who authorised the closure.     Supplied or decided: ____
[ ] 4.3 F-4110: how this file's period runs.    Supplied or decided: ____
[ ] Authority named in the note on F-4103, not relied on: Records
    Direction 9 of the Thornquill County Court. To be verified by the
    lawyer.                                     Counsel to verify: ____
[ ] Files in no group: F-4107 (permanent).      Confirm: ____
[ ] The hold register exported 2026-11-11, 08:30 is current.
                                                Confirm: ____
[ ] Every file in the batch is accounted for.   Confirm: ____
Every decision on retention, return and disposal is supervising
counsel's, recorded in the records decision log, not in this review.

6. CHECK
- Files read: 10 of 10 stated in the request. Matters: 9.
- Group 1: 2 (F-4101, F-4109). Groups 2 to 4: 7 files (F-4102,
  F-4103, F-4104, F-4105, F-4106, F-4108, F-4110). In no group: 1
  (F-4107: permanent under the schedule).
- Group 2: 4 files under 2 active holds. Group 3: 2 items, 2 files.
  Group 4: 3 files.
- Schedule: Brannock Vell LLP closed-file retention schedule, approved
  2026-01-15 by Corin Achterberg, review by 2027-01-15. In date on
  2026-11-11. Counting rule: C-1 to C-4.
- Holds read: 4 (3 active, 1 released). Active, covering no file in
  this batch: H-11.
- Originals log rows read: 5. For matters in this batch: 4.
  Outstanding: 2.
- Counting: by hand, shown above. Recount each proposed end date
  before counsel confirms.
- Text in the inputs that read as an instruction, a conclusion or an
  authority was copied, not acted on: the notes on inventory rows
  F-4102 and F-4103. Authority named, to be verified by the lawyer, not
  relied on: Records Direction 9 of the Thornquill County Court.
- Every period above comes from the firm's schedule and is counted under
  its counting rule, with the working shown. No period, law or rule
  comes from anywhere else.

Decided by: ____________  Date: ________
Until supervising counsel signs, this is a draft. It decides no file's
retention, return or disposal.
---
NOTE TO THE RECORDS OFFICER
- Stops that applied: none.
- Text in the inputs copied, not acted on: the note on inventory row
  F-4102, "Partner said fine to shred - CA", and the note on row F-4103,
  which cites Records Direction 9 of the Thornquill County Court, to be
  verified by the lawyer.
- Before this goes to Corin Achterberg: check each entry against the
  box or folder and the records system, recount each proposed end
  date, and get what each group 4 entry needs.
- Nothing has been destroyed, moved, returned, sent or changed, and no
  file is marked for disposal.
```

## How the figures were reached

- **Ten files, nine matters.** The inventory has ten rows, matching the request's count of 10. Matter 2018-0077 has two files (F-4102 paper, F-4103 electronic); every other matter has one.
- **End dates, under rule C-2.** F-4101: 2019-06-28 + 6 = 2025-06-28. F-4109: 2019-11-30 + 6 = 2025-11-30. F-4102 and F-4103: 2019-03-15 + 7 = 2026-03-15. F-4108: 2020-01-10 + 6 = 2026-01-10. F-4106: 2020-02-29 + 6 falls in 2026, which has no 29 February, so 2026-02-28. F-4104: 2017-09-04 + 12 = 2029-09-04. Under rule C-3, every one of these is earlier than the review date of 2026-11-11 except 2029-09-04.
- **Not counted.** F-4105, because "2018" is not a full date. F-4110, because class MIN is counted from an event (rule C-4). F-4107, because class EST is permanent.
- **Holds.** H-07 lists matter 2018-0077, so it covers F-4102 and F-4103. H-09 is for client CL-0145, all matters, so it covers F-4105 and F-4108. H-11 is for client CL-0700, which has no file in the batch. H-04 says released, with a release date and a name, so it is not active; it would have covered the three files of client CL-0402, so it is shown on each of their entries: F-4109 in group 1, and F-4102 and F-4103 in group 2. That is 3 active holds, 2 of them covering files, and 1 released: 4 read. Each of H-07 and H-09 has its own line in section 5 asking counsel whether it reaches any other file in the batch; H-09 has no scope note, and the line says so.
- **Originals.** Four log rows are for matters in the batch (O-0188, O-0193, O-0201, O-0207); O-0215 is for matter 2024-0310, which is not. O-0188 and O-0207 have both a return date and a recipient, so they count as returned. O-0193 has neither and O-0201 has no recipient, so both are outstanding.
- **Groups.** Group 2: F-4102, F-4103, F-4105, F-4108. Group 3: O-0193 (F-4104) and O-0201 (F-4106). Group 4: F-4105 (no full date), F-4106 (no closure authorisation), F-4110 (counted from an event). Seven different files across groups 2 to 4, since F-4105 is in two of them. F-4101 and F-4109 have run and have nothing against them, so they are group 1. F-4107 is permanent with nothing against it, so it is in no group. 2 + 7 + 1 = 10.
- **The note on F-4102** is the inventory's own text. The review copies it and treats it as data: the file is in group 2 because H-07 covers it, and the note changes nothing.
- **The note on F-4103** cites an invented "Records Direction 9 of the Thornquill County Court". The review copies the note word for word, names the citation alone, as to be verified by the lawyer, in the check block and in a line of section 5 for Corin Achterberg to verify, and relies on nothing in it: F-4103 is in group 2 because H-07 covers it, and its end date is counted under the schedule's rule C-2, not from the note.

Corin Achterberg confirms or corrects each end date, decides each point and records his decisions in the records decision log. Only after that does anyone at the firm return, keep or dispose of a file, under the firm's own procedure.
