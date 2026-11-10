# Outgoing work sign-off log: tried once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs were the invented example in `public/example.md` (the request, `signoff-log.csv` and the eight messages). No client data was used. The run was made by a model that did not write the template. It read the template and only the example's inputs, followed the instruction block and the output format, produced the update, and only then compared it with the example's published output and the reviewer checklist.

## What came out

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

## What was observed

- **Every required part was produced.** All headings are present, counts add up (5 + 2 + 1 + 2 = 10), and nothing in the update comments on any draft. No stop condition was triggered: today's date was given, all twelve headers matched, no item ID was duplicated, and no message contained a password or an instruction to the assistant.
- **Difference from the published example:** none of substance. The two outputs agree line for line on counts, flags, their order, the raise-with lists, the history lines and the updated file. I found no fact in either output that is not in the inputs.
- **Caveat on that agreement.** I read the example's inputs only, but the template's own acceptance tests describe several of the same situations (a decision passed on, a send before approval, an unknown item, a weekend count), and the worked rules are tightly specified. The match shows the rules are deterministic on this input. It does not show the template copes with inputs unlike the example.
- **Places where the instructions left room for a guess:**
  - "The message word for word" for an attorney's note: the example's message wraps over two lines. I joined them with a single space and kept the "S-103:" prefix as part of the message. The template does not say whether a line break or an ID prefix belongs in the note.
  - Attorney B's return says "resubmit by Friday". I did not treat that as a new send-by date, because step 3 allows a change only from a message that gives a new send-by date. The template does not say what to do with a resubmission deadline that differs from the send-by date, and the item stays flagged "due soon and returned" against 2026-11-16.
  - Open items whose send-by date has already passed (S-105) get their own date heading at the top of the open list. The format implies it by sorting on date, but never says it.
  - Ordering of items under "Closed in this update" is not stated. I used item ID.
  - The "Defaults used for" line: because every setting was supplied, I wrote "none". The template does not say how to treat "no closures" and "no covering attorneys" when the person states them explicitly, but this reading is the natural one.
  - The "For:" line wants an "operations manager role"; I wrote "Operations manager", as the example does.
  - A flagged item that is also under a different person's action (S-103 is returned, so the next move is the preparer's, not Attorney B's) is still listed under Attorney B in "To raise with each attorney". That follows the rule as written; whether it is useful is a judgment for the firm.
  - A date in the message "went to Client A by email this afternoon" gives no closed date, so the message's date (2026-11-11) was used, as the rule says.
- **Defects found in the template:** none that changed the result. The checklist item "the counts add up" and the note about "[N]" both worked. The acceptance tests in the template are still marked as proposed and were not run by this trial, which covered only the one example.
- **What this trial does not show.** It ran once, in one product, on one invented input. It does not show how the template behaves on a real firm's export, with renamed columns, covering attorneys, closed days, a first run, or the other acceptance tests. It was not tested in a law firm.

## Edits made after this run

After this run and an independent review, the same day, the template, the example's opening line, the profile and the source credits were edited by Opus 5.5 (claude-opus-5-5). These edits were not run again. Each template edit settles a point listed above in the way this run already chose, so the output recorded above conforms to the edited wording; the record above is unchanged.

- An attorney's note joins a message that runs over several lines with single spaces and keeps an item ID at its start.
- A resubmit-by date in a return, such as "resubmit by Friday", stays in the note and is not a new send-by date.
- Open items are listed earliest date first, so items past their date head the open list under their own date headings.
- Items under "Closed in this update" are in item ID order.
- The instruction block now gives "item already closed" and "decision unclear: ask the attorney" as two separate reasons, as the procedure and the output format already did.
