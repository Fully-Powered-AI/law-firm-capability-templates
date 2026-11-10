# Trial: Matter budget and status summary, run once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-10

The inputs are the invented example in `public/example.md` (the request, the matter plan and phase table, the time export and the matter lead's notes). No client data was used. The run read the template's fenced instruction block, its output format and the notes on how the format is filled in, as they stand after the independent review, and the example's inputs. The arithmetic was done in code: row selection, phase totals, the tie-out, billed and unbilled, the age of unbilled time, the schedule day counts and the team time.

This record replaces an earlier one. A first run on the same day, by a different model that had not written the template, followed the template as it stood before the review and found eight ambiguities and defects. The template was then edited to settle them (a blank phase code is also listed under the checks; the pasted block now carries the format notes and the rules it had left out; the order of actions without an owner; what "Prepared for" names; a phase named by code and name in a rule line; a missing Partner's rating read as "none given"; where a line under Other that is not about the merits goes; questions that offer no options), and the example gained one line under Other to show that last case. Because those edits change what the block produces, the run was made again and is recorded here.

This run is weaker evidence than the first in one way: it was made by the model that made the edits after the review, and that model had read the first run's output and the published example's output before running. It is a check that the revised template can be followed to the published result, not an independent reading of it.

## What came out

The output is printed in full, as produced.

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
1. P1 Due diligence is complete with fees to date of $26,000 against its
   budget of $24,000, over by $2,000. How do you want the overrun on P1
   handled?
2. The matter's projected total is $65,005 against the $60,000 budget last
   agreed with the client on 2026-08-28, over by $5,005 (8%), within the
   red margin of 10%. How do you want the projected overrun handled?
3. The risk "Client R's lender wants its own review of the leases before
   closing" has no owner. Who owns it?
4. The action "Book the closing call with the lender" has no owner and no
   due date. Who owns it, and by when is it due?

CHECKS ON THE RECORDS (for the billing coordinator)
- T-15: dated 2026-11-09, after the as-of date (Associate B, $800); not
  counted.
- T-16: other matter, M-4415 (2026-10-21, Associate C, $700); not counted.
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

## What was observed

- **Every required part was produced,** in the template's order, with every heading. The run did not stop: the plan added up (phase budgets $60,000 against a matter budget of $60,000), all needed columns were present, no row's amount differed from hours times rate, and nothing in the files read like an instruction.
- **Figures and ratings matched the published example.** 14 of 16 rows used; fees to date $42,005, of which $34,000 billed and $8,005 unbilled; phases $41,480 plus $525 not coded; projected total $65,005, over by $5,005 (8%); budget amber on two rules; schedule green; T-02 unbilled for 64 days. The team time, the actions' order and the LEFT OUT count were the same.
- **The edited rules showed in the output.** T-14, with a blank phase code, was listed under the checks, making four checks. "Prepared for" printed "responsible partner", although the narrative has the operations lead preparing it. The rule lines named each phase by code and name. The missing Partner's rating heading printed "none given". The non-merits line under Other was printed under Developments, and the merits line was counted under LEFT OUT by heading only.
- **No fact was added, and no option offered.** Every figure and name comes from the inputs. The questions state facts from the records and ask how the partner wants each overrun handled, or who owns each ownerless item.
- **Differences from the published example, all wording.** Question 1 here gives only the figures, where the example also cites the data room date from the notes. Question 2 here gives the red margin, where the example gives the two phase projections behind the total. Question 4 here asks "Who owns it, and by when is it due?" where the example asks "Who takes it, and by when?". The checks lines for T-15 and T-16 order their details differently and wrap differently.
- **Nothing was told to stop for, and nothing was declined.**

## Ambiguities and limits found

1. The questions may cite context from the notes or not; the template allows both, and the run and the example differ. Neither recommends an answer.
2. The run did not reach any stop condition, the not-supplied estimate path, a late phase, an export with no entries for the matter, or text that reads like an instruction. Those paths remain untried.
3. The acceptance tests are marked proposed and none has been run; this trial is only the ordinary-matter case, on one input, in one product.
