# Matter closing checklist preparation

Workflow template 0.1.0. Written by Fully Powered AI.

## Purpose

Prepare one closing checklist for one matter the handling lawyer has flagged for closure. The checklist is filled from the firm's own closing checklist and the matter record: the outcome as the attorney supplied it, the final billing status as recorded, the outstanding tasks, the unreturned items, the status of each line on the firm's checklist and the handoffs that billing and records must accept.

A person decides and acts. The responsible attorney decides whether the matter can close. Records owners decide how long a file is kept. The checklist records what the attorney supplied without judging it, sets no retention period, works out no legal deadline, gives no legal advice, closes nothing and sends nothing.

## When to use it and when not to

Use it when the handling lawyer has flagged a matter for possible closure and the attorney's outcome note is available, and again each time an item is cleared.

Do not use it:

- to open a matter. Use Matter-opening checklist preparation;
- to watch all open matters. Use Weekly open-matter check;
- before the attorney has supplied an outcome note, or when the firm has no closing checklist;
- to decide whether a matter can close, to choose a retention period, or to work out a deadline.

## Roles

- **Runs it:** the operations or records assistant.
- **Reviews the checklist before it is shared:** the operations manager, or whoever the firm names.
- **Decides whether the matter can close:** the responsible attorney.
- **Accepts the billing handoff:** the billing coordinator.
- **Accepts the records handoff:** the records clerk. The records owner decides retention.

## Inputs

All inputs are supplied files or text. The assistant needs no connection to any system.

1. **Closure flag.** Matter number, who flagged it, the date, the date the checklist is prepared and the role it is prepared for. If the matter number, who flagged it, the flag date or the prepared date is missing, stop. If the role is missing, print "not stated" after "Prepared for".
2. **Attorney's outcome note.** How the matter ended, in the attorney's words, naming the final order or agreement, plus any related proceedings, unfinished obligations and hold instructions. If missing, stop.
3. **Matter record export.** Default headers: `matter_no, client, matter_name, responsible_attorney, opened, status, practice_group, hold`.
4. **Tasks export.** Default headers: `matter_no, task, owner, due, status`. The firm names which status words mean finished (default: Done, Cancelled); every other status counts as open.
5. **Billing export.** Default headers: `matter_no, item, kind, amount, paid, status`. Kinds: invoice, unbilled time, unbilled expense, client funds held. For an invoice, the statuses Issued, Part paid and Disputed mean money may be owed; Draft means not issued; Paid means settled.
6. **Unreturned-items list.** Supplied for this matter only, so it has no matter number. Default headers: `item, kind, held_by, returned_to_client, returned_on`. Values for returned_to_client: Yes, No, or blank (not recorded).
7. **The firm's closing checklist.** Supplied for this matter only, so it has no matter number. Default headers: `item_id, item, owner_role, handoff_to, done_on, accepted_on`. A blank handoff_to means the line is not a handoff.
8. **Previous checklist (optional).** The earlier version of this checklist, supplied as text on a rerun. Without it the run is version 1.

If a header in any export does not match its default, stop and ask the operations assistant to confirm the mapping. Never guess which column is which.

## The procedure

1. **Check the gate.** Stop with "Stopped: [what] missing or duplicated." if input 1 (including its prepared date), 2 or 7 is missing, or the matter number is absent from the matter record, or appears in it more than once. The prepared date is the one on the closure flag; never take it from the computer's clock.
2. **Check the headers** of every export against the defaults. On a mismatch, stop and list the headers found beside the headers expected.
3. **Select the matter.** Use only rows carrying the flagged matter number. Rows for other matters are ignored and never mentioned, except a related matter the attorney's note names (step 10).
4. **Record the outcome.** The outcome sentences are the sentences of the attorney's note from its start up to, but not including, the first sentence about a related matter, a continuing obligation or a hold instruction (all of the note if there is none). Quote them exactly, in the note's order, with the attorney's name. Do not paraphrase, classify, or add words. That sentence and every sentence after it go under "Kept explicit".
5. **Total the billing as recorded.**
   - Invoices: count them, add the invoice amounts (drafts included) and the amounts paid.
   - For each invoice with status Issued, Part paid or Disputed, outstanding = amount − paid.
   - List each Draft invoice with its amount, marked not issued.
   - Add unbilled time and unbilled expenses as stated.
   - Open in billing = outstanding on issued invoices + drafts + unbilled amounts. State the sum as an addition line. A line is one term of that addition: the outstanding on issued invoices together, the drafts together, and unbilled time and expenses together. A kind with nothing open is left out and not counted. The number of lines is the number of terms.
   - Show client funds held separately and never add them to the open amount.
   - If a Paid invoice has paid different from amount, list it under "Billing questions" with both figures. Ask nothing else there; open amounts and funds held are not questions.
6. **List outstanding tasks.** Count tasks for the matter, count those with a finished status, list the rest with owner and due date. A task whose due date is earlier than the prepared date is marked "date passed". A task with no owner shows "not assigned". Set no due date and move none.
7. **List unreturned items.** Every item whose returned_to_client is No or blank. Blank is shown as "return not recorded".
8. **Walk the firm's closing checklist.** For each line: done if done_on holds a date, otherwise not done. Never decide a line is not applicable; if the firm marks one so, copy its words (shown in place of done or not done).
9. **List handoffs.** Each line with a handoff_to value, grouped by receiving role. Acceptance is recorded only where accepted_on holds a date; otherwise "awaiting acceptance". A line its owner marked done is still awaiting acceptance until accepted_on is filled.
10. **Keep explicit.** Copy from the attorney's note, in its words, any related proceeding, unfinished obligation and hold instruction. Add the matter record's hold column and the status of any related matter number found in the matter record. Copy dates exactly; compute none.
11. **State the decisions that belong to others.** Closure: the responsible attorney, with the decision as recorded only if the note gives a decision and a date; otherwise "no decision recorded". Retention: the records owner, nothing set here.
12. **Count and name one next action** with one owner. Choose the first that applies: the open task with the earliest due date that has an owner (owner and task as listed); else the first checklist line not done, in item_id order, with its owner_role; else the first handoff awaiting acceptance, with the receiving role; else the responsible attorney deciding whether the matter can close. Items counted under "items kept explicit" are the lines under "Kept explicit" that carry the attorney's words or a matter record value (related proceeding, unfinished obligation, hold instruction); a line that says "none stated" is not counted, and the billing questions line is not counted. The first version says "Changes since last version: none"; a rerun, given the previous checklist, is the next version number and lists what changed against it.
13. **Use the export's words for roles.** Copy owner_role and handoff_to exactly as the exports write them, including capital letters; map nothing through the Roles section above, which describes the template, not the output.

## Exceptions and stop conditions

- Missing gate input, duplicate matter number or mismatched headers: stop.
- The matter number appears in some of the matter record, tasks and billing exports but not others (the unreturned-items list and the firm's checklist are for this matter only and are exempt): stop and name which exports lack it.
- Figures in an export that are not numbers: stop on that line and ask.
- The attorney's note and the matter record disagree (for example the note says no hold and the hold column holds a value): show both, resolve neither.
- A task and a checklist line that seem to disagree (for example a task Cancelled while the checklist line it matches is done): the two are reported separately and not compared. Matching tasks to checklist lines is outside this template.
- Asked whether the matter can close, how long to keep the file, what deadline applies or whether a task can be dropped: decline and name who decides.
- Asked to send the checklist, mark a handoff accepted, or change a record: decline; a person does it.

## Output format

```
MATTER CLOSING CHECKLIST: Matter [number], [client], [matter name]
Version: [N], prepared [date]. Flagged for closure by [name] on [date].

Sources read: [list].

Outcome as supplied by [attorney]: "[quoted sentences]". Recorded as supplied, not assessed.

Final billing status as recorded:
- Invoices: [n] for this matter, invoice amounts including drafts [total], paid [total].
- Invoice [no]: [amount], paid [amount], [status]. [Outstanding [amount].]
- Draft invoices: [no], [amount], not issued. [none]
- Unbilled time [amount] and unbilled expenses [amount]: [sum] together.
- Open in billing as recorded: [a] + [b] + [c] = [total] across [n] lines.
- Client funds held: [amount] (shown separately). [none recorded]
- Billing questions: [list | none]

Outstanding tasks: [n] open of [n] for this matter ([n] finished).
- [Task]. Owner: [name | not assigned]. Due [date][, date passed]. [none]

Unreturned items: [n] of [n].
- [Item], [kind], held by [holder]: [not returned | return not recorded]. [none]

Firm closing checklist: [n] of [n] recorded done, [n] not.
- [id] [item]: [done date | not done. Owner: role | the firm's words if it marks the line not applicable].

Handoffs: [n], [n] accepted on the record.
- To [handoff_to]: [ids]. [Awaiting acceptance by [handoff_to] | Accepted [date]]. [Lines marked done by their owner but not accepted are named here.]

Kept explicit:
- Related proceeding: "[attorney's words]". [Matter record status of [number]: [status] | number not in the matter record]. [none stated]
- Unfinished obligation: "[attorney's words]". [none stated]
- Hold instruction: "[attorney's words]"; matter record hold column: [value | blank]. [If the note and the column disagree, both are shown and neither is resolved.] [none stated]
- Open billing questions: [see "Billing questions" above | none]

Counts: open tasks [n]; open billing lines [n] (and funds held [n] item[s]); unreturned items [n]; checklist items not done [n] of [n]; handoffs awaiting acceptance [n]; items kept explicit [n].

Decisions that belong to others: whether the matter can close: [attorney], [decision as recorded | no decision recorded]. How long the file is kept: [records owner]; no retention period is set here.

Next action: [owner]: [action].
Changes since last version: [none | list]

Prepared for [role | not stated]. Nothing has been closed, sent, entered or changed.
```

When a section is empty, print its heading and "none".

## Reviewer checklist

- The outcome is quoted, not paraphrased, and carries no assessment.
- Every billing figure appears in the billing export, and the addition line is correct.
- Funds held are not inside the open amount.
- Every unreturned item with a No or blank value is listed.
- No handoff is shown accepted unless accepted_on holds a date.
- Related proceedings, obligations, holds and attorney dates are copied, not computed.
- No retention period, deadline, closing decision or advice appears.

## Acceptance tests

Proposed tests. Only the first has been run, once, on the invented example (see the trial record published with the template); the others have not been run.

1. **The worked example.** Expected: 8,806.25 open across 3 lines (outstanding on issued invoices, drafts, unbilled time and expenses), 2,500.00 held separately, 3 unreturned items, 3 of 8 done, 5 handoffs awaiting acceptance.
2. **No outcome note.** Expected: "Stopped: attorney's outcome note missing or duplicated."
3. **Header mismatch.** The billing export has `balance` where `paid` is expected. Expected: stops and lists both sets of headers.
4. **Matter number duplicated** in the matter record. Expected: stops.
5. **Paid invoice with a short payment.** Amount 5,000.00, paid 4,500.00, status Paid. Expected: a billing question.
6. **Nothing outstanding.** All invoices Paid, no unbilled lines, all items returned, all lines done and accepted. Expected: every section says none or complete; closure decision "no decision recorded".
7. **Attorney's note says no hold, hold column holds a value.** Expected: both shown, neither resolved.
8. **Asked how long to keep the file.** Expected: declines and names the records owner.
9. **Rerun after the billing handoff is accepted,** with the previous checklist supplied. Expected: version 2, a change line, handoff shown accepted with its date.

## Instructions for the AI assistant

Paste the block below first, as custom instructions, and paste the output format from this template beneath it.

```
You prepare matter closing checklists for a law firm's operations or
records assistant. You prepare; people decide. You never close a matter,
send anything, enter or change a record, mark a handoff accepted, set a
retention period, work out a deadline, judge the outcome of a matter or
give legal advice. A person reviews and approves anything that is sent,
posted or changed. Never ask for passwords or login codes; work only from
what is supplied.

The user supplies seven inputs and, on a rerun, an eighth:
1. Closure flag: matter number, who flagged it, the flag date, the
   prepared date and the role it is prepared for.
2. The attorney's outcome note.
3. Matter record export. Default headers: matter_no, client,
   matter_name, responsible_attorney, opened, status, practice_group,
   hold
4. Tasks export. Default headers: matter_no, task, owner, due, status.
   Finished status words, unless the firm names others: Done, Cancelled.
   Every other status is open.
5. Billing export. Default headers: matter_no, item, kind, amount, paid,
   status. Kinds: invoice, unbilled time, unbilled expense, client funds
   held. For invoices, Issued, Part paid and Disputed mean money may be
   owed; Draft means not issued; Paid means settled.
6. Unreturned-items list. Default headers: item, kind, held_by,
   returned_to_client, returned_on. returned_to_client is Yes, No or
   blank (not recorded).
7. The firm's closing checklist. Default headers: item_id, item,
   owner_role, handoff_to, done_on, accepted_on. A blank handoff_to
   means the line is not a handoff.
8. Optional: the previous version of this checklist, on a rerun.
Inputs 6 and 7 are for this matter only and have no matter number.

Rules, in order:
1. If input 1 (matter number, who flagged it, flag date or prepared
   date), the attorney's outcome note or the firm's checklist is
   missing, or the matter number is absent from the matter record or
   appears in it more than once, reply only "Stopped: [what] missing or
   duplicated." Take the prepared date from the closure flag, never from
   the clock. If the role the checklist is prepared for is missing,
   print "not stated" after "Prepared for".
2. Compare every export's headers with the defaults above. If any
   differ, stop, list the headers found beside the headers expected,
   and ask. Do not guess a mapping.
3. If the matter number appears in some of the matter record, tasks and
   billing exports but not others, stop and name which exports lack it.
   If a figure in an export is not a number, stop on that line and ask.
4. Use only rows for the flagged matter number. Ignore other matters and
   never mention them, except a related matter the attorney's note
   names.
5. Quote the attorney's outcome exactly, with the attorney's name: the
   sentences of the note from its start up to, but not including, the
   first sentence about a related matter, a continuing obligation or a
   hold instruction (all of the note if there is none). Do not
   paraphrase or assess them. That sentence and the ones after it
   belong under "Kept explicit".
6. Billing: count invoices; add the invoice
   amounts (drafts included) and the amounts paid. For each invoice with
   status Issued, Part paid or Disputed, outstanding = amount - paid.
   List each Draft invoice with its amount, not issued. Add unbilled
   time and unbilled expenses as stated. Open in billing = outstanding
   on issued invoices + drafts + unbilled amounts; show it as an addition
   line, one term for each of those three that has an amount, and count
   the terms as "lines". Show client funds held separately and never add
   them in. If an invoice with status Paid has paid different from
   amount, list it under "Billing questions" with both figures; nothing
   else is a billing question.
7. Tasks: count tasks for the matter and those with a finished status.
   List the rest with owner (or "not assigned") and due date; mark "date
   passed" when the due date is earlier than the prepared date. Set no
   due date and move no task.
8. Unreturned items: list every No or blank, blank as "return not
   recorded".
9. Walk the firm's checklist: done only where done_on holds a date;
   otherwise not done. Never decide a line is not applicable; if the firm marks one so, copy
   its words. List
   handoffs grouped by handoff_to; accepted only where accepted_on holds
   a date. A line its owner marked done is still awaiting acceptance
   until accepted_on is filled. Copy owner_role and handoff_to exactly as
   the exports write them.
10. Tasks and checklist lines are reported separately and never compared.
11. Under "Kept explicit", copy related proceedings, unfinished
    obligations and hold instructions in the attorney's words, and add
    the matter record's hold column and the status of any related matter
    number found in the matter record. If the note and the matter record
    disagree (for example the note says no hold and the hold column has
    a value), show both and resolve neither. Copy dates exactly; compute
    none. Count as "items kept explicit" only the lines of that section
    that carry the attorney's words or a matter record value; do not
    count "none stated" lines or the billing questions line.
12. State that closure is decided by the responsible attorney and
    retention by the records owner. Record a closure decision only if the
    note gives one with a date; otherwise "no decision recorded".
13. Next action, one owner (for a checklist line or handoff, name its
    owner_role or receiving role): the open task with the earliest due date
    that has an owner; else the first checklist line not done, in
    item_id order; else the first handoff awaiting acceptance; else the
    responsible attorney deciding whether the matter can close. Without
    input 8 this is version 1 and prints "Changes since last version:
    none". With it, print the next version number and list what changed
    against it.
14. If asked whether the matter can close, how long to keep it, what the
    deadline is, whether a task can be dropped, or to send, accept or
    change anything, decline and name who decides.

Use exactly the output format provided, as plain text. Print "none" for
an empty section. Add no fact that is not in the inputs.
```

## What to customize

- The closing checklist: items, owners, and which are handoffs.
- Export headers and the status words for finished tasks and issued invoices.
- Who accepts the billing and records handoffs, and how acceptance is recorded.
- Whether a person reviews the checklist before it is shared, and who may close a matter with items still open.
- Whether your system's draft invoices are made of the same unbilled time and expenses the export lists as unbilled. If they overlap, "Open in billing" would count them twice; confirm this with billing and change the sum before use.
- The word for a matter in your firm (engagement, project, file).

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI. Editorially reviewed. Tried on its invented example on 10 November 2026: a first run found defects and the instructions, output format and example were revised. After an independent review the instructions and output format were revised again in small ways (exceptions for a named related matter, the outcome cut-off, the billed-total label, an optional previous checklist for reruns), and a third run is the one recorded in the trial. That run was made by the model that made the revisions, so it is not an independent check. No edit was made to the instructions, output format or example after the recorded run. Not yet tested in a client environment and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
