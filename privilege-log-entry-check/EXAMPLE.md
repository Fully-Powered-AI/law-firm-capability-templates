# Privilege log entry check: an invented example

*Illustrative example with invented data.* Bramblecote Ashby LLP, its people, its client Quillmere Pumps Ltd, the other side Corvane Metals Inc., the Superior Court of Eastmere, the case, the log, the export, the role map and the approved log format below are all invented. The format and basis codes are one invented review counsel's choices for one invented matter. They are not any real court's requirements and must not be used for a real log.

The paralegal's five inputs come first, in full, then what the workflow template prepares. In the draft log, each filled Description cell holds review counsel's own text. It is shown here as `[counsel's text]`, because the check reads only whether that cell is filled and never reads, judges or copies what it says.

## Input 1: the request

Sent by Tomas Wrenfield, paralegal, on Tuesday 10 November 2026.

```
Quillmere: draft 3 of our privilege log is attached, with today's
designation export from the review platform, Ilse's approved log format
and the role map. Please run the entry check before the log goes to her.

Matter: Quillmere Pumps Ltd v. Corvane Metals Inc., case no.
EM-CV-26-04417, Superior Court of Eastmere. We act for Quillmere.
Review counsel: Ilse Marrable.

Tomas Wrenfield, paralegal
```

## Input 2: counsel's approved log format

```
Bramblecote Ashby LLP · Privilege log format · Quillmere v. Corvane
Approved by: Ilse Marrable, review counsel. Dated: 2 November 2026.
Changes go through her.

Columns, in this order. Every column is filled, except where a line
below says it may be blank.
  Entry No | Doc ID | Parent Doc ID | Doc Date | Doc Type | Author | To |
  CC | BCC | Treatment | Basis Code | Description
Doc ID: QPL- followed by seven digits, as assigned by the review platform.
Parent Doc ID: the parent's Doc ID for an attachment; blank for a parent.
Doc Date: YYYY-MM-DD, as the review platform holds it. Never estimated.
Names: as written on the role map, separated by "; ". Anyone the role map
  marks Counsel = Y is written with " *" after the name, in every column.
To, CC and BCC: each blank only when the record has no one in that field.
Treatment: Withheld (export: Withhold) or Redacted (export: Redact).
Basis Code: 01, 02 or 01+02, as defined in my code list. No other code.
Description: written or approved by review counsel only. Staff check only
  that it is filled.
Attachments: each attachment is its own entry.
```

## Input 3: the role map

```
Quillmere v. Corvane · Role map
Approved by: Ilse Marrable, 2 November 2026.

Name           | Email                         | Organisation       | Role                 | Counsel
Gideon Pask    | gpask@quillmere.example       | Quillmere Pumps    | Operations director  | N
Ruth Calloway  | rcalloway@quillmere.example   | Quillmere Pumps    | In-house counsel     | Y
Joel Fenner    | jfenner@quillmere.example     | Quillmere Pumps    | Finance manager      | N
Mara Quist     | mquist@quillmere.example      | Quillmere Pumps    | Quality lead         | N
Ilse Marrable  | imarrable@bramblecote.example | Bramblecote Ashby  | Outside counsel      | Y
```

## Input 4: the designation export

```
Quillmere v. Corvane · Designation export · exported 10 November 2026

Doc ID      | Family ID | Parent Doc ID | Attachment Count | Doc Date   | Doc Type      | Author        | To                       | CC          | BCC       | Designation
QPL-0001021 | F-0021    |               | 2                | 2026-03-04 | Email         | Gideon Pask   | Ruth Calloway            | Joel Fenner |           | Withhold
QPL-0001022 | F-0021    | QPL-0001021   | 0                | 2026-03-03 | Spreadsheet   | Joel Fenner   |                          |             |           | Withhold
QPL-0001023 | F-0021    | QPL-0001021   | 0                | 2026-03-02 | PDF           | Mara Quist    |                          |             |           | Withhold
QPL-0001040 | F-0040    |               | 0                | 2026-03-11 | Email         | Ruth Calloway | Gideon Pask; Mara Quist  |             |           | Redact
QPL-0001057 | F-0057    |               | 1                | 2026-04-02 | Email         | Ilse Marrable | Ruth Calloway            | Gideon Pask |           | Withhold
QPL-0001058 | F-0057    | QPL-0001057   | 0                | 2026-04-01 | Word document | Ilse Marrable |                          |             |           |
QPL-0001066 | F-0066    |               | 0                | 2026-04-15 | Email         | Joel Fenner   | Ruth Calloway            |             | Dana Wilk | Withhold
QPL-0001071 | F-0071    |               | 0                | 2026-05-06 | Memo          | Ruth Calloway | Gideon Pask              |             |           | Withhold
QPL-0001080 | F-0080    |               | 0                | 2026-05-20 | Email         | Gideon Pask   | Mara Quist               |             |           | Produce
```

## Input 5: the draft log, version 3

```
Quillmere v. Corvane · Privilege log · draft 3 · 10 November 2026

Entry No | Doc ID      | Parent Doc ID | Doc Date   | Doc Type    | Author          | To                      | CC          | BCC | Treatment | Basis Code | Description
1        | QPL-0001021 |               | 2026-03-04 | Email       | Gideon Pask     | Ruth Calloway *         | Joel Fenner |     | Withheld  | 01         | [counsel's text]
2        | QPL-0001022 | QPL-0001021   | 2026-03-30 | Spreadsheet | Joel Fenner     |                         |             |     | Withheld  | 01         | [counsel's text]
3        | QPL-0001040 |               | 2026-03-11 | Email       | Ruth Calloway * | Gideon Pask; Mara Quist |             |     | Redacted  | 01         | [counsel's text]
4        | QPL-0001057 |               | 2026-04-02 | Email       | Ilse Marrable * | Ruth Calloway *         | Gideon Pask |     | Withheld  | 02         |
5        | QPL-0001066 |               | 2026-04-15 | Email       | Joel Fenner     | Ruth Calloway           |             |     | Withheld  | 01         | [counsel's text]
6        | QPL-0001080 |               | 2026-05-20 | Email       | Gideon Pask     | Mara Quist              |             |     | Withheld  | 03         | [counsel's text]
```

## What the workflow template prepares

A short note to the paralegal, then the check.

> Tomas, the check of draft 3 is below. No stop applied: every header matched the approved format and the defaults, and I read all 6 entries and all 9 export records. Two entries are complete. Four are incomplete, with 7 issues between them. Two attachments of logged emails have no entry, and one memo designated Withhold has no entry.
>
> Lines you can check yourself against the export and the role map: entry 2's date, and entry 5's missing BCC and missing counsel marker. The rest are Ilse Marrable's: the blank description on entry 4, the code 03 on entry 6, entry 6 being logged although the export says Produce, a role for Dana Wilk, and the three records with no entry: QPL-0001023 and QPL-0001071, which the export designates Withhold, and QPL-0001058, which has no designation recorded.
>
> I have changed nothing in the log, sent, served, filed, signed or calendared nothing, and made no privilege call. The log is not served until Ilse Marrable approves it.

```
DRAFT PRIVILEGE LOG CHECK · FOR REVIEW COUNSEL TO CONFIRM
Metadata only. Not legal advice. Nothing is decided about legal meaning,
merit, validity, privilege, conflicts or deadlines; no privilege call is
made or suggested.
Nothing has been changed, sent, served, filed, signed or calendared.

Matter: Quillmere Pumps Ltd v. Corvane Metals Inc., EM-CV-26-04417
Log checked: Quillmere v. Corvane · Privilege log · draft 3 ·
  10 November 2026, 6 entries
Prepared for: Ilse Marrable, review counsel, to confirm
Run by: Tomas Wrenfield, paralegal

MEASURED AGAINST
- Approved log format: Bramblecote Ashby LLP · Privilege log format ·
  Quillmere v. Corvane, dated 2 November 2026, approved by Ilse Marrable
- Role map: Quillmere v. Corvane · Role map, approved by Ilse Marrable
  on 2 November 2026, 5 people
- Designation export: Quillmere v. Corvane · Designation export,
  exported 10 November 2026, 9 records:
  6 Withhold, 1 Redact, 1 Produce, 1 none recorded

A. ENTRY-BY-ENTRY CHECKLIST
Entry 1 · QPL-0001021 · Withheld · COMPLETE · family: 1 of 2 attachments
  have no entry (B1)
  - No issues.
Entry 2 · QPL-0001022 · Withheld · INCOMPLETE: 1 issue
  - R2, Doc Date: log 2026-03-30; export 2026-03-03.
Entry 3 · QPL-0001040 · Redacted · COMPLETE
  - No issues.
Entry 4 · QPL-0001057 · Withheld · INCOMPLETE: 1 issue · family: 1 of 1
  attachments have no entry (B2)
  - R9, Description: log blank; format requires it.
Entry 5 · QPL-0001066 · Withheld · INCOMPLETE: 3 issues
  - R4, BCC: log blank; export Dana Wilk.
  - R5, To: log Ruth Calloway, no " *"; role map Counsel Y.
  - R5, BCC: Dana Wilk in the export; not on the role map (E1).
Entry 6 · QPL-0001080 · Withheld · INCOMPLETE: 2 issues
  - R7, Treatment: log Withheld; export Produce (D1).
  - R8, Basis Code: log 03; format permits 01, 02, 01+02.

B. ATTACHMENTS OF LOGGED PARENTS WITH NO ENTRY
B1. QPL-0001023 · attachment to QPL-0001021 (entry 1) · family F-0021
   Export: 2026-03-02 · PDF · author Mara Quist · designation
   Withhold. No entry in the log.
B2. QPL-0001058 · attachment to QPL-0001057 (entry 4) · family F-0057
   Export: 2026-04-01 · Word document · author Ilse Marrable ·
   designation none recorded: for review counsel to decide. No entry in
   the log.

C. DESIGNATED RECORDS WITH NO ENTRY
C1. QPL-0001071 · 2026-05-06 · Memo · author Ruth Calloway · designation
   Withhold. No entry in the log.

D. ENTRIES WITH NO MATCHING DESIGNATION
D1. Entry 6 · QPL-0001080 · logged Withheld · export: Produce. See entry 6.

E. PEOPLE NOT ON THE ROLE MAP
E1. Dana Wilk · BCC of QPL-0001066 in the export · no role recorded. See
   entry 5.

REVIEW COUNSEL TO CONFIRM
[ ] Entry 2, Doc Date: log 2026-03-30; export 2026-03-03.
      Confirm: ____
[ ] Entry 4, Description: blank.
      Write or approve: ____
[ ] Entry 5, BCC: Dana Wilk is in the export and not on the log.
      Confirm: ____
[ ] Entry 5, To: Ruth Calloway has no " *"; role map Counsel Y.
      Confirm: ____
[ ] Entry 5, BCC / E1: Dana Wilk is not on the role map.
      Supply: ____
[ ] Entry 6, Treatment / D1: logged Withheld; export Produce.
      Decide: ____
[ ] Entry 6, Basis Code: 03 is not on the approved list.
      Supply: ____
[ ] B1: QPL-0001023, designated Withhold, has no entry.
      Confirm: ____
[ ] B2: QPL-0001058, no designation recorded, has no entry.
      Decide: ____
[ ] C1: QPL-0001071, designated Withhold, has no entry.
      Confirm: ____
[ ] Every privilege call, designation, basis code and description on the
    log is review counsel's.                         Confirm: ____
[ ] Log approved for service.          Approved by: ____  Date: ____

CHECK
- Headers: log matches the approved format; export matches; role map
  matches.
- Entries: 6 read. 2 complete, 4 incomplete, 7 issues.
- Designated records (Withhold or Redact): 7. With an entry: 5.
  Designated records in B or C: 2. 5 + 2 = 7.
- Other export records: 1 Produce, 1 none recorded.
- Attachments of logged parents with no entry: 2, of which 1 with no
  designation recorded. Designated records with no entry: 1. Entries
  with no matching designation: 1. People not on the role map: 1.
- Roles are taken from the role map only. None is inferred from a name,
  title, department or email address.
- No description, subject line or document text is copied into this check.

Reviewed by: ____________  Date: ________
Until review counsel signs, this is a draft and the log is not approved.
```

Two lines are worth a second look. Entry 1 is complete on its own, yet its family is not: the export gives the email two attachments and the log carries one. And QPL-0001058 has no designation at all, so the check lists it as an attachment with no entry and no designation recorded, and leaves to Ilse Marrable both what it is and whether it goes on the log. The export names outside counsel as its author, and the check draws nothing from that.

Tomas Wrenfield checks the metadata lines against the export and the role map, then gives the log and the check to Ilse Marrable. She confirms, decides or supplies each line, writes or approves the description for entry 4, and approves the log. The check is run again on the corrected draft, and only after her approval do people at the firm serve the log.
