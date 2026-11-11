# Matter closing checklist preparation: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs for this trial are the invented example published with the template (`public/example.md`, section "The inputs", items 1 to 7). No client data was used.

## How many runs, and who made them

Three runs on 2026-11-10. The first followed the first draft of the template's instruction block and output format. It found the defects listed below; the template, its output format and the published example were then revised. The second run followed the revised block on the same inputs. After an independent review, the instruction block and output format were revised again in small ways: an exception for a related matter the attorney's note names, a tighter rule for where the quoted outcome ends, the invoice total relabelled as "invoice amounts including drafts", an optional previous checklist for reruns, copying the firm's words for a not-applicable line, and naming the owner role in the next action. The third run, recorded here, followed that block and output format on the same inputs. It was made by the model that made the revisions, with the earlier output in view, so it is not an independent check and does not show that a reader who has not seen the earlier output would reach the same result. The earlier runs' outputs are not kept; what the first found is summarised here.

## What the first run found

- The two stop messages differed between the procedure and the instruction block.
- The instruction block left out rules that sat only in the procedure: the stop when the matter number is in only some exports, the stop on figures that are not numbers, the billing question for a Paid invoice whose paid amount differs from its amount, and showing both values when the note and the matter record disagree. It also relied on default headers and finished status words that were not in the pasted text.
- The matter-number rule would have stopped on the unreturned-items list and the firm's checklist, which carry no matter number.
- The count of lines in the open-in-billing sum, the count of items kept explicit, the choice of outcome sentences, the source of the prepared date and the role it is prepared for, the choice of next action, and whether role words are copied or mapped were all left to guesswork.
- The task "Clear calendar reminders" is Cancelled while checklist line C7 is marked done; the template said nothing about comparing tasks with checklist lines.
- The published example's output did not follow the output format.

## What came out of the third run

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

## What was observed in the third run

Every part of the output format was produced, and nothing in the inputs triggered a stop condition. The unreturned-items list and the firm's checklist, which carry no matter number, did not stop the run. The figures were checked against the billing export: 8,806.25 open across 3 lines, 2,500.00 held separately, 3 unreturned items, 3 of 8 checklist lines done, 5 handoffs awaiting acceptance, which is what acceptance test 1 expects. The addition line sums correctly. No fact appears in the output that is not in the inputs.

The output differs from the second run in one line: the invoice total is now labelled "invoice amounts including drafts", because it includes the draft invoice. The quoted outcome stops before the sentence about the related matter, as the revised rule says. No previous checklist was supplied, so the run is version 1. The output published in `public/example.md` is this output, copied from the run. Its plain-text layout, line wording and counts follow the output format.

Billing questions is "none", because the only Paid invoice has paid equal to amount. The task "Clear calendar reminders" (Cancelled) and checklist line C7 (done) were reported separately and not compared, as the template now says.

Only acceptance test 1 was exercised. The other acceptance tests, including the stops, the short-payment billing question and the rerun with a previous checklist, have not been run.

## What this does not show

One recorded run on one invented example, by the model that revised the template, is not a test in a real firm. The template has not been tested in a client environment and has not been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini. The wording of the pasted instructions was read against the output format line by line after the run; no further edits were made to it after the third run.
