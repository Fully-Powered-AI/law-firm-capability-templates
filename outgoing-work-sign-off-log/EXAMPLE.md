# Outgoing work sign-off log: an invented example

*Illustrative example with invented data.* The firm, its people, its clients, its matters and every record and message below are invented. People are shown by role: three attorneys (Attorney A, B and C), two associates, two paralegals and a billing coordinator. The firm's operations manager updates the sign-off log on the morning of Thursday 12 November 2026. The inputs come first, in full, then the update the capability is meant to return.

## What the operations manager supplied

**The request**

```
Update the sign-off log as of Thursday 12 November 2026.
Attached: signoff-log.csv, saved after yesterday's update, and the
messages that came in since then, pasted below.
Settings: warning window 2 working days; we work Monday to Friday; no
office closures this month; no covering attorneys this week; column
headers are the defaults.
```

**signoff-log.csv** (the log as it stood after Wednesday's update)

```
item_id,matter,item,drafted_by,attorney,goes_to,send_by,submitted,status,attorney_note,decided_on,closed_on
S-101,M-310,Engagement letter,Paralegal 1,Attorney A,client,2026-11-11,2026-11-06,approved,"Approved.",2026-11-09,
S-102,M-312,Status letter,Associate 1,Attorney A,client,2026-11-13,2026-11-09,waiting,,,
S-103,M-315,Response to document requests,Associate 2,Attorney B,other side,2026-11-16,2026-11-10,waiting,,,
S-104,M-318,Filing cover letter and exhibit index,Paralegal 2,Attorney B,court,2026-11-12,2026-11-10,waiting,,,
S-105,M-320,Invoice cover letter,Billing coordinator,Attorney C,client,2026-11-10,2026-11-05,returned,"Use the agreed fee cap figure, not the hourly total.",2026-11-06,
S-106,M-322,Client meeting agenda,Associate 1,Attorney C,client,2026-11-20,2026-11-11,waiting,,,
S-107,M-325,Letter enclosing signed documents,Paralegal 1,Attorney A,other side,2026-11-18,2026-11-11,waiting,,,
S-108,M-331,Letter confirming meeting date,Associate 1,Attorney C,other side,2026-11-12,2026-11-11,waiting,,,
```

**The messages since the last update** (gathered from the sign-off mailbox)

```
1. From: Paralegal 1 | 2026-11-11 16:40
S-101 engagement letter went to Client A by email this afternoon.

2. From: Attorney B | 2026-11-12 08:15
S-103: returning this one. Please use the definitions from our earlier
letter and resubmit by Friday.

3. From: Paralegal 2 | 2026-11-12 08:50
Attorney B said S-104 is fine to file today.

4. From: Attorney A | 2026-11-12 09:05
S-107 approved, go ahead.

5. From: Associate 1 | 2026-11-12 09:30
S-108 went out to the other side this morning.

6. From: Attorney C | 2026-11-12 09:45
S-111 approved.

7. From: Paralegal 2 | 2026-11-12 10:10
New for sign-off. ID: S-109. Matter: M-327. Item: Certificate of
service. Attorney: Attorney B. Goes to: court. Send by: 2026-11-17.

8. From: Associate 2 | 2026-11-12 10:20
New for sign-off. ID: S-110. Matter: M-329. Item: Client update email.
Goes to: client. Send by: 2026-11-13.
```

## What came back

```
OUTGOING WORK SIGN-OFF LOG as of 2026-11-12, Thursday
For: Operations manager. Log: signoff-log.csv, 8 items before this update. Messages: 8 (6 recorded, 2 not recorded).
Settings: warning window 2 working days; working days Monday to Friday; closed days none; covering attorneys none; column headers default. Defaults used for: none.

COUNTS
Items in the log: 10. Waiting 5. Returned 2. Approved, not yet sent 1. Sent 2. Withdrawn 0. Could not read 0.
Flagged: 6.

FLAGGED
1. S-108 Letter confirming meeting date | M-331 | attorney Attorney C | goes to other side | send by 2026-11-12 | sent on 2026-11-12 | FLAG: sent without recorded approval. Sent on 2026-11-12, reported by Associate 1.
2. S-105 Invoice cover letter | M-320 | attorney Attorney C | goes to client | send by 2026-11-10 | returned on 2026-11-06 | FLAG: past its date. Send by 2026-11-10; today 2026-11-12; 2 days past.
3. S-104 Filing cover letter and exhibit index | M-318 | attorney Attorney B | goes to court | send by 2026-11-12 | waiting | FLAG: due soon and not reviewed; decision passed on by someone else. 0 working days left. Decision passed on by Paralegal 2 at 2026-11-12 08:50.
4. S-102 Status letter | M-312 | attorney Attorney A | goes to client | send by 2026-11-13 | waiting | FLAG: due soon and not reviewed. 1 working day left.
5. S-110 Client update email | M-329 | attorney not named | goes to client | send by 2026-11-13 | waiting | FLAG: due soon and not reviewed; no attorney named. 1 working day left.
6. S-103 Response to document requests | M-315 | attorney Attorney B | goes to other side | send by 2026-11-16 | returned on 2026-11-12 | FLAG: due soon and returned. 2 working days left.

OPEN ITEMS BY SEND-BY DATE
2026-11-10, Tuesday
S-105 Invoice cover letter | M-320 | drafted by Billing coordinator | attorney Attorney C | goes to client | submitted 2026-11-05 | returned on 2026-11-06 | attorney's note: "Use the agreed fee cap figure, not the hourly total." | FLAG: past its date
2026-11-12, Thursday
S-104 Filing cover letter and exhibit index | M-318 | drafted by Paralegal 2 | attorney Attorney B | goes to court | submitted 2026-11-10 | waiting | no note | FLAG: due soon and not reviewed; decision passed on by someone else
2026-11-13, Friday
S-102 Status letter | M-312 | drafted by Associate 1 | attorney Attorney A | goes to client | submitted 2026-11-09 | waiting | no note | FLAG: due soon and not reviewed
S-110 Client update email | M-329 | drafted by Associate 2 | attorney not named | goes to client | submitted 2026-11-12 | waiting | no note | FLAG: due soon and not reviewed; no attorney named
2026-11-16, Monday
S-103 Response to document requests | M-315 | drafted by Associate 2 | attorney Attorney B | goes to other side | submitted 2026-11-10 | returned on 2026-11-12 | attorney's note: "S-103: returning this one. Please use the definitions from our earlier letter and resubmit by Friday." | FLAG: due soon and returned
2026-11-17, Tuesday
S-109 Certificate of service | M-327 | drafted by Paralegal 2 | attorney Attorney B | goes to court | submitted 2026-11-12 | waiting | no note
2026-11-18, Wednesday
S-107 Letter enclosing signed documents | M-325 | drafted by Paralegal 1 | attorney Attorney A | goes to other side | submitted 2026-11-11 | approved on 2026-11-12 | attorney's note: "S-107 approved, go ahead."
2026-11-20, Friday
S-106 Client meeting agenda | M-322 | drafted by Associate 1 | attorney Attorney C | goes to client | submitted 2026-11-11 | waiting | no note
No send-by date
- none

CLOSED IN THIS UPDATE
S-101 Engagement letter | M-310 | attorney Attorney A | sent on 2026-11-11, reported by Paralegal 1
S-108 Letter confirming meeting date | M-331 | attorney Attorney C | sent on 2026-11-12, reported by Associate 1 | FLAG: sent without recorded approval
Closed before this update and kept in the file: 0.

COULD NOT READ
- none

TO RAISE WITH EACH ATTORNEY
Attorney A: S-102 (due soon and not reviewed; send by 2026-11-13)
Attorney B: S-104 (due soon and not reviewed; decision passed on by someone else; send by 2026-11-12); S-103 (due soon and returned; send by 2026-11-16)
Attorney C: S-108 (sent without recorded approval; send by 2026-11-12); S-105 (past its date; send by 2026-11-10)
No attorney named: S-110 (due soon and not reviewed; no attorney named; send by 2026-11-13)

NOT RECORDED
- Paralegal 2, 2026-11-12 08:50, S-104: not from the attorney named on the item.
- Attorney C, 2026-11-12 09:45, S-111: no item S-111 in the log.

HISTORY LINES TO ADD
2026-11-11 16:40 | S-101 | approved to sent | from Paralegal 1
2026-11-12 08:15 | S-103 | waiting to returned, note: "S-103: returning this one. Please use the definitions from our earlier letter and resubmit by Friday." | from Attorney B
2026-11-12 09:05 | S-107 | waiting to approved, note: "S-107 approved, go ahead." | from Attorney A
2026-11-12 09:30 | S-108 | waiting to sent, without recorded approval | from Associate 1
2026-11-12 10:10 | S-109 | submitted for sign-off | from Paralegal 2
2026-11-12 10:20 | S-110 | submitted for sign-off | from Associate 2

UPDATED LOG FILE
item_id,matter,item,drafted_by,attorney,goes_to,send_by,submitted,status,attorney_note,decided_on,closed_on
S-101,M-310,Engagement letter,Paralegal 1,Attorney A,client,2026-11-11,2026-11-06,sent,"Approved.",2026-11-09,2026-11-11
S-102,M-312,Status letter,Associate 1,Attorney A,client,2026-11-13,2026-11-09,waiting,,,
S-103,M-315,Response to document requests,Associate 2,Attorney B,other side,2026-11-16,2026-11-10,returned,"S-103: returning this one. Please use the definitions from our earlier letter and resubmit by Friday.",2026-11-12,
S-104,M-318,Filing cover letter and exhibit index,Paralegal 2,Attorney B,court,2026-11-12,2026-11-10,waiting,,,
S-105,M-320,Invoice cover letter,Billing coordinator,Attorney C,client,2026-11-10,2026-11-05,returned,"Use the agreed fee cap figure, not the hourly total.",2026-11-06,
S-106,M-322,Client meeting agenda,Associate 1,Attorney C,client,2026-11-20,2026-11-11,waiting,,,
S-107,M-325,Letter enclosing signed documents,Paralegal 1,Attorney A,other side,2026-11-18,2026-11-11,approved,"S-107 approved, go ahead.",2026-11-12,
S-108,M-331,Letter confirming meeting date,Associate 1,Attorney C,other side,2026-11-12,2026-11-11,sent,,,2026-11-12
S-109,M-327,Certificate of service,Paralegal 2,Attorney B,court,2026-11-17,2026-11-12,waiting,,,
S-110,M-329,Client update email,Associate 2,,client,2026-11-13,2026-11-12,waiting,,,

Draft for the Operations manager to check and save. The log has not been saved, nothing has been sent, no one has been contacted, no item has been approved, returned or released by the assistant, and no draft was read.
```

How the figures were reached. Working days left count Monday to Friday after Thursday 12 November: Friday 13 is 1 and Monday 16 is 2, so S-102 and S-110 (due Friday) and S-103 (due Monday) fall inside the two-day window, while S-109, due Tuesday 17 with 3 working days left, does not. S-107 is approved and not yet due, so it carries no flag. Paralegal 2's message about S-104 reports Attorney B's view second-hand, so S-104 stays waiting until Attorney B says so in their own message. The counts add up: 5 waiting, 2 returned, 1 approved and 2 sent make the 10 items in the file.

The capability never saw any of the drafts. Everything above comes from the log, the eight messages and the settings.
