# Weekly open-matter check: one trial on its invented example

- **Product:** Claude (run in Claude Code, its command-line coding tool)
- **Model:** Claude Fable 5.2
- **Date:** 2026-11-09
- **Runs:** one on this version of the instructions. An earlier run the same day, on the first draft, is summarised at the end.

The inputs are the invented example published with this template. The firm, its people, its clients, its matters and every record are invented, and no client data was used. This is a record of one run on that example. It is not a test in any firm's environment.

## Inputs used

Exactly what the operations manager supplies in [the example](example.md), and nothing else:

- the request, with the check date (Monday 2 November 2026) and the firm's settings: a roster up to 7 days old, a list of at most 10 matters, the status words "open" and "done", the standard note layout, the sign-off "Operations manager", and the summary going to the managing partner. The request says nothing about column headers;
- `roster.csv` from the billing coordinator, 7 matters, dated 2026-11-02;
- `matters.csv`, 7 matters, and `tasks.csv`, 13 tasks, both exported from the case system.

The template's instructions for an AI assistant and its output format were given to a new session as written, followed by the request and the three files. That session was given nothing else from this template: not the example's output, not the rest of the template and not the record of the earlier run.

## What came out

The run finished without stopping. The assistant read the three files directly. The one shell command it asked to run was not permitted in the session, so the counts and the date arithmetic were worked out without code; every figure was then recomputed from the files in code for this record. The complete output, as produced (the assistant did not wrap long lines):

```
WEEKLY OPEN-MATTER CHECK as of 2026-11-02
Input: export (matters.csv, 7 matters; tasks.csv, 13 tasks).
Roster: dated 2026-11-02, from the billing coordinator, 7 matters, 0 days old
(check date 2026-11-02 minus roster date 2026-11-02 = 0 days; limit 7 days).
Settings: roster age limit 7 days; list size 10; status words
open/done; column headers default.
Defaults used for: column headers.

Coverage: expected 7 open matters per roster dated 2026-11-02 (billing coordinator); assessed 6 of them; could not assess 1: M-206, Client F, Attorney C (on the roster but not in the matters export).
In the system but not on the roster: M-208, Estate administration, Client H (assessed).
On the roster with a status other than open in the system: none.

Outcome: partial: roster matter M-206 is not in the matters export and could not be assessed.

Totals: 7 matters assessed (6 on the roster, 1 not on it); 10 open tasks; 4 overdue; 3 unowned; 1 with no due date. 3 finished tasks were left out.

MATTERS ASSESSED
M-201 Supply dispute | Attorney A | open 3 | overdue 2 | unowned 1 | no due date 0 | earliest open due 2026-10-23
M-202 Lease renewal | Attorney B | open 2 | overdue 1 | unowned 1 | no due date 0 | earliest open due 2026-10-30
M-203 Insurance claim | Attorney A | open 2 | overdue 0 | unowned 0 | no due date 1 | earliest open due 2026-11-02
M-204 Property boundary dispute | Attorney C | open 0 | overdue 0 | unowned 0 | no due date 0 | earliest open due none | no tasks recorded
M-205 Regulatory inquiry | Attorney B | open 2 | overdue 1 | unowned 0 | no due date 0 | earliest open due 2026-10-19
M-207 Partnership dissolution | Attorney A | open 0 | overdue 0 | unowned 0 | no due date 0 | earliest open due none | no open tasks
M-208 Estate administration | Attorney C | open 1 | overdue 0 | unowned 1 | no due date 0 | earliest open due 2026-11-10 | not on the roster
Not assessed, not open in the system and not on the roster: none.

COULD NOT ASSESS
- M-206, Client F, Attorney C: on the roster but not in the matters export

COULD NOT READ
- none
Tasks for a matter that is not in the matters export, counted nowhere: none.

ATTENTION LIST (4 of at most 10)
1. M-201 Supply dispute (Attorney A): 2 overdue, 1 unowned
2. M-202 Lease renewal (Attorney B): 1 overdue, 1 unowned
3. M-205 Regulatory inquiry (Attorney B): 1 overdue, 0 unowned
4. M-208 Estate administration (Attorney C): 0 overdue, 1 unowned
Rule: matters with at least one overdue or unowned task; most overdue first; then most unowned; then the earliest open due date; then matter ID. Client size plays no part.

DRAFT NOTES

DRAFT, not sent
To: Attorney A
Subject: M-201 Supply dispute (Client A): tasks needing attention as of 2026-11-02
I am going through the open matters as of 2026-11-02. On M-201:
Overdue:
- File reply brief (T-01), no owner: due 2026-10-23; check date 2026-11-02; 10 days late
- Prepare exhibit list (T-02), Paralegal 1: due 2026-10-28; check date 2026-11-02; 5 days late
Who is taking these, and when will they be done?
Operations manager

DRAFT, not sent
To: Attorney B
Subject: M-202 Lease renewal (Client B): tasks needing attention as of 2026-11-02
I am going through the open matters as of 2026-11-02. On M-202:
Overdue:
- Request landlord's ledger (T-05), Paralegal 2: due 2026-10-30; check date 2026-11-02; 3 days late
Not yet due, no owner:
- Schedule client call (T-06), due 2026-11-06
Who is taking these, and when will they be done?
Operations manager

DRAFT, not sent
To: Attorney B
Subject: M-205 Regulatory inquiry (Client E): tasks needing attention as of 2026-11-02
I am going through the open matters as of 2026-11-02. On M-205:
Overdue:
- Assemble document production (T-09), Paralegal 2: due 2026-10-19; check date 2026-11-02; 14 days late
Who is taking this, and when will it be done?
Operations manager

DRAFT, not sent
To: Attorney C
Subject: M-208 Estate administration (Client H): tasks needing attention as of 2026-11-02
I am going through the open matters as of 2026-11-02. On M-208:
Not yet due, no owner:
- Request account statements (T-13), due 2026-11-10
Who is taking this, and when will it be done?
Operations manager

DRAFT SUMMARY

DRAFT, not sent
To: Managing partner
Subject: Weekly open-matter check as of 2026-11-02
Coverage: expected 7 open matters per roster dated 2026-11-02 (billing coordinator); assessed 6 of them; could not assess 1: M-206, Client F, Attorney C (on the roster but not in the matters export).
In the system but not on the roster: M-208, Estate administration, Client H (assessed).
On the roster with a status other than open in the system: none.
Totals: 7 matters assessed (6 on the roster, 1 not on it); 10 open tasks; 4 overdue; 3 unowned; 1 with no due date. 3 finished tasks were left out.
The matters that most need attention (4):
1. M-201 Supply dispute (Attorney A): 2 overdue, 1 unowned
2. M-202 Lease renewal (Attorney B): 1 overdue, 1 unowned
3. M-205 Regulatory inquiry (Attorney B): 1 overdue, 0 unowned
4. M-208 Estate administration (Attorney C): 0 overdue, 1 unowned
Could not assess: M-206, Client F, Attorney C.
Could not read: none.
Also on the sheet: M-204 Property boundary dispute (no tasks recorded); M-207 Partnership dissolution (no open tasks); M-203 Insurance claim (T-07 Send client status letter has no due date)
I am writing to the responsible attorney on each matter on the list.
Operations manager

FOR THE OPERATIONS MANAGER
- Matter to find: M-206 (Client F, Attorney C) is on the roster but not in this morning's matters export, so none of its tasks could be checked.
- Question for the billing coordinator: M-208 Estate administration (Client H, Attorney C) is open in the system but not on the roster dated 2026-11-02. Should it be on the roster?
- Mismatches to settle: the roster and the export name the same responsible attorney on every matter that appears in both.
- No tasks recorded: M-204 Property boundary dispute (Attorney C). This is not the same as clear.
- No open tasks: M-207 Partnership dissolution (Attorney A) has only finished tasks (T-11, T-12), yet its status in the system is open. This is not the same as clear.
- Task with no due date: T-07 Send client status letter on M-203 (owner Paralegal 1, Attorney A responsible). M-203 has no overdue or unowned task, so it is not on the attention list and no note was drafted.
- Record text that reads like an instruction: none found.
- The managing partner's name was not supplied, so the summary is addressed by title.
- You asked for the notes to be signed "Operations manager"; I used the same sign-off on the summary.

Nothing was sent and nothing in the case system was changed.
```

## What was observed

**Every part of the output format was produced, in order:** the header with the roster-age working and the settings line, the three coverage lines before any row, the outcome, the totals, one row for each of the seven assessed matters, the line for matters neither open nor on the roster, the matter that could not be assessed, Could not read with "- none", the line for tasks whose matter is not in the export, the attention list with its rule, four draft notes, the draft summary, the list for the operations manager and the closing line.

**The figures are right and match the published example exactly:** the coverage line (7 expected, 6 assessed, M-206 could not be assessed, M-208 in the system and not on the roster), the outcome (partial), the totals (7 matters assessed, 6 on the roster and 1 not; 10 open tasks, 4 overdue, 3 unowned, 1 with no due date, 3 finished tasks left out), every row, the ranking, and the days late in every note (10, 5, 3 and 14).

**The column headers were handled as the instructions now say.** The three files carry the default headers, the request supplied none, and the settings line reports "column headers default" and "Defaults used for: column headers". Nothing had to be guessed.

**Against the reviewer checklist,** the points that can be checked from the files alone hold: the expected count equals the roster; every roster matter is a row or is named as not assessed; no finished task is counted; the task due on the check date (T-08) is not shown as overdue; the rows add up to the totals; the list follows the printed rule and holds no clean matter; every note goes to the responsible attorney, is marked as a draft and suggests no date or owner; the summary carries the coverage lines and the matter that could not be assessed. The checks that need a person opening the case system, and the attorney confirming the days late, could not be made in a trial on invented files.

**The points the format now fixes were followed:** the closing question is in the plural on the two notes that list two tasks and in the singular on the two that list one; the note subject says "tasks needing attention"; T-03, which has an owner and a future date, is counted on M-201's row and listed in no note; rows without a fixed note end after the earliest due date; the summary repeats the coverage lines and the totals line word for word and carries the "Could not assess" and "Could not read" lines; M-207, whose tasks are all finished, is on the "Also on the sheet" line; every date is printed as YYYY-MM-DD.

**Nothing made the run stop.** The roster was 0 days old, both exports were present with the expected headers, every task had a readable status and date, no task pointed at a matter missing from the export, and no record held text that read like an instruction. The assistant was not asked to send or change anything, so the refusals were not exercised. Those paths were not tried in this run. In particular, the stop on a header that matches neither the defaults nor the settings was not tried.

**Where the instructions still left a choice to the assistant:**

1. **The wording of a reason.** The format asks for a reason beside a matter that could not be assessed and for the reason an outcome is partial, and gives no fixed words for either. The assistant wrote "on the roster but not in the matters export" and "partial: roster matter M-206 is not in the matters export and could not be assessed".
2. **The wording of "Also on the sheet".** The format says which matters belong on the line and not how each is described. The assistant put the reason in brackets after each matter and named the task and its title.
3. **How much goes under "For the operations manager".** The instructions list what belongs there and send any remark with no other place to the same list. The assistant wrote nine lines, three of them reporting that nothing was found or explaining a choice: that the roster and the export agree on every responsible attorney, that no record text read like an instruction, and that the summary is addressed by title and carries the same sign-off as the notes because no name or separate sign-off was supplied. A firm that wants a shorter list will need to say so.
4. **Line length.** The format is shown wrapped. The assistant printed each line unwrapped.

**Differences from the published example,** all in wording and none in any figure:

- The reason beside M-206 reads "on the roster but not in the matters export" in this run and "on the roster, not in the matters export" in the example. The outcome sentence is worded differently.
- "Also on the sheet" names the same three matters in both. This run adds each matter's name and T-07's title.
- This run's list for the operations manager is longer, as described in point 3 above. The example's list has a line this run's does not: that T-08 is due on the check date and is not overdue.
- This run's lines are not wrapped. The example's are.

The example's output was brought into line with the revised output format in the same editing session that set up this run, after the run had finished, so the agreement in layout between the two is not independent evidence. The example's figures were not changed.

**Shortcomings of this trial.** One run, on one small example of 7 matters and 13 tasks, in one product, with the counting done without code. The example exercises a matter missing from the export, a matter missing from the roster, a task due on the check date, a blank due date, a matter with no tasks and a matter with only finished tasks. It does not exercise an old roster, a missing roster, a missing or renamed column, column headers supplied in the settings, an unreadable task, a task whose matter is not in the export, a status mismatch, a differing responsible attorney, ties in the ranking, a list longer than the limit, or a request to send or change something.

## The earlier run, and what it changed

The first draft of the instructions was run once on the same inputs, in the same product, earlier on 9 November 2026. Its figures were the same as above. It showed nine places where that draft left a choice to the assistant, and the instructions and the output format were revised on each before the run recorded here:

1. **Column headers.** The draft described the fields in words and said never to guess at a renamed column, without saying which headers it expected. The assistant read `id`, `due` and `roster_as_of` as the named fields and carried on, where a stricter reading would have stopped. The template now states the default headers for all three files, lets the firm's settings replace them, and stops on any needed column whose header matches neither.
2. **The settings line** was to appear "only if defaults were used", which did not cover stated settings that equal the defaults. It is now always printed, with each value in use and the settings that fell back to a default.
3. **The roster-age working** had no place in the header. The roster line now carries it.
4. **Two meanings of "assessed".** The coverage line counted roster matters and the totals counted all matters, with nothing to tell them apart. The totals line now splits its count into matters on the roster and matters not on it.
5. **Empty blocks of the sheet.** Nothing said whether they are printed. They now are, with "- none".
6. **The closing question** was fixed in the plural and read wrongly on a note with one task. It now follows the number of tasks.
7. **The date format** was not stated. It is now YYYY-MM-DD.
8. **"Also on the sheet"** did not say whether a matter with only finished tasks belongs there. It now does.
9. **The note's subject** said "open tasks" although the note lists only overdue, unowned and undated tasks. It now says "tasks needing attention", and the template says an owned task with a date not yet passed is left out of the note.

## Edits after the recorded run

**9 November 2026.** The template was edited after the run recorded above, following its independent review, and was not run again. The recorded output and observations above are unchanged and describe the instructions as they stood at the run. What changed:

- The settings gained a status word for an open matter (default "open"), and the settings line now prints it. The recorded run's settings line does not have it.
- Fixed wording was given for the reason beside a matter that could not be assessed, for the reasons of a partial outcome and for the entries of "Also on the sheet", which were points 1 and 2 of the choices left to the assistant. The recorded run's wording of those three differs from the fixed wording.
- The instructions now say what a stopped check prints: the coverage line with the expected count and "assessed 0", and the outcome "stopped".
- They now say that a task that could not be read is left out of the open counts and the finished count, that an unowned task due on the check date goes under "Not yet due, no owner", and that every line of the format ending "or none" is always printed.
- In the published example, the settings line and the outcome line were brought into line with these edits, and the line saying that T-08 is due on the check date and is not overdue was removed from the list for the operations manager, because the instructions do not ask for it. The example's figures were not changed.

None of these edits has been tried in a run.
