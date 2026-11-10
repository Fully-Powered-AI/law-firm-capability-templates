# Court-order deadline notice preparation: one trial on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Fable 5.2
- **Date:** 2026-11-09
- **Runs:** one, on the template and example as they now stand

The inputs are the invented example published with this template. The firm, its people, its client, the court, the order, the rule file and the court-closure list are all invented, and no client data was used. This is a record of one run on that example. It is not a test in any firm's environment, and the invented rule file is not any real court's rule.

This record replaces an earlier one from the same day. The earlier run, on the first text of the template, proposed no date for the meet and confer while the published example proposed one, because the template did not say what a "mixed" sentence was. The template now defines it, the example follows the cautious reading, and several smaller choices the earlier run had to make are now written down. The run below was made after those changes.

## Inputs used

Exactly the four inputs the legal assistant supplies in [the example](example.md), and nothing else:

- the request of Monday 9 November 2026, which says the order is saved to the matter file and gives the matter name, the case number and the four people on the matter;
- the three-page order of the invented Superior Court of Eastmere, entered November 6, 2026;
- the invented firm's order deadline rule file, dated 1 October 2026, with rules R-0 and R-1 and its list of counts it does not cover;
- the court-closure list, covering 1 October 2026 to 31 December 2027.

The template's instructions for an AI assistant were given as written, followed by the output format and the five lines on how to fill it in, then these inputs. Two cautions about this record. The example's own output sits in the same file as the inputs, so it was in view. And the session that made this run had just revised the template and the example after review, so it knew what the example's output said. The run was worked from the instructions, and the dates were counted separately with a calculation tool, but it was not a blind run and it is not an independent check of the example.

## What came out

No stop applied. The order was reported as saved, so the question about saving was not asked. The text was readable, the order is signed and carries an entry stamp with its date, the caption and case number match, 3 of 3 pages were read against the footer, a handling attorney is named, and the rule file is dated, approved, in date and names this court. The complete output:

> Dalia, the draft notice for Copperline is below. I read 3 of 3 pages and no stop applied. Two dates are proposed under your rule R-1. Three counts are not computed. Your rule file does not cover a count from service (the payment). It does not cover a count in court days or a count backwards from a conference (the joint statement). The meet-and-confer count of 14 days is in the same sentence as that court-day count, so the sentence is mixed: your rule file sends a sentence that holds two kinds of count to the attorney, and I have proposed no date for either part of it. Two directives are outside the numbered list: one in footnote 1 on page 1 and one in the discussion on page 2.
>
> Still to do, by people: read the draft against the order, recount the two proposed dates on a calendar, and give the draft to Marcus Thibault. I have sent nothing and calendared nothing. Nothing is circulated or calendared until he confirms.

```
DRAFT ORDER NOTICE · FOR THE ATTORNEY TO CONFIRM
Proposed dates only. Not legal advice. Nothing has been calendared or sent.

Matter: Copperline Bakery Supply Co. v. Ostrander Freight, Inc.
Case no.: LC-CV-26-01873
Prepared for: Marcus Thibault, handling attorney, to confirm
After confirmation, to: Helen Voss, supervising partner; Joan Abara,
  paralegal; Petra Lindahl, docketing. Not to the client.

ORDER
- Court: Superior Court of Eastmere, County of Linden (p. 1)
- Title: Order on Discovery Dispute and Resetting Case Management
  Conference (p. 1)
- Signed: November 5, 2026 (p. 3)
- Entered: November 6, 2026 (ENTERED stamp, p. 1)

WHAT THE COURT ORDERED
1. "Any party seeking a protective order covering the route data shall file
   its request within 10 days of entry of this order." (p. 1, fn. 1)
2. "Counsel shall meet and confer regarding the delivery-log custodians within
   14 days of this order, and shall file a joint statement of any remaining
   dispute no later than 5 court days before the conference set below."
   (p. 2, para. 1)
3. "Defendant shall produce all documents responsive to Requests for
   Production Nos. 7 through 15 within 20 days of entry of this order."
   (p. 2, ¶ 1)
4. "Defendant shall serve a privilege log no later than December 4, 2026."
   (p. 2, ¶ 2)
5. "Defendant shall pay $3,180.00 to plaintiff's counsel within 30 days of
   service of this order." (p. 2, ¶ 3)
6. "The case management conference set for December 10, 2026 is vacated."
   (p. 3, ¶ 4)
7. "A further case management conference is set for January 14, 2027 at 9:00
   a.m. in Department 4." (p. 3, ¶ 4)

DATES
A. PROPOSED: Monday 16 November 2026. Any party seeking a protective order
   covering the route data to file its request.
   "within 10 days of entry of this order" (p. 1, fn. 1).
   Working: entered Friday 6 November 2026 (ENTERED stamp, p. 1); entry day
   not counted; calendar days counted, so Wednesday 11 November (Veterans
   Day) is counted like any other day; day 10 is Monday 16 November 2026;
   not a Saturday or Sunday; not on the closure list; no closed day moved
   the last day. Rule R-1.
B. NOT COMPUTED: counsel to meet and confer regarding the delivery-log
   custodians. "within 14 days of this order" (p. 2, para. 1). The rule file
   does not cover a sentence that holds two kinds of count: this sentence
   holds a count of days from the order and a count in court days backwards
   from a conference. Attorney to supply the date.
C. NOT COMPUTED: counsel to file a joint statement of any remaining dispute.
   "no later than 5 court days before the conference set below" (p. 2,
   para. 1). The rule file does not cover a count in court days or a count
   backwards from a conference. Attorney to supply the date.
D. PROPOSED: Monday 30 November 2026. Defendant to produce all documents
   responsive to Requests for Production Nos. 7 through 15.
   "within 20 days of entry of this order" (p. 2, ¶ 1).
   Working: entered Friday 6 November 2026 (ENTERED stamp, p. 1); entry day
   not counted; calendar days counted, 11 November included; day 20 is
   Thursday 26 November 2026, on the closure list (Thanksgiving Day); Friday
   27 November is on the closure list (Day after Thanksgiving); 28 and 29
   November are a Saturday and a Sunday; the next day that is none of these
   is Monday 30 November 2026. Rule R-1.
E. COPIED: December 4, 2026. Defendant to serve a privilege log. Stated in
   the order (p. 2, ¶ 2). Not recounted.
F. NOT COMPUTED: defendant to pay $3,180.00 to plaintiff's counsel. "within
   30 days of service of this order" (p. 2, ¶ 3). The rule file does not
   cover a count from service of the order. Attorney to supply the date.

HEARINGS
- VACATED: December 10, 2026, case management conference (p. 3, ¶ 4)
- SET: January 14, 2027, 9:00 a.m., Department 4, further case management
  conference (p. 3, ¶ 4)

AMOUNTS
- $3,180.00, paid by defendant to plaintiff's counsel, "within 30 days of
  service of this order" (p. 2, ¶ 3)

ATTORNEY TO CONFIRM
[ ] A. Proposed Monday 16 November 2026 (rule R-1).  Confirm or correct: ____
[ ] B. Not computed: meet and confer.                Your date: ____
[ ] C. Not computed: joint statement.                Your date: ____
[ ] D. Proposed Monday 30 November 2026 (rule R-1).  Confirm or correct: ____
[ ] E. Copied December 4, 2026 (p. 2).               Confirm: ____
[ ] F. Not computed: payment of $3,180.00.           Your date: ____
[ ] Hearings: December 10, 2026 VACATED; January 14, 2027 SET.  Confirm: ____
[ ] Every directive in the order is listed above.    Confirm: ____

CHECK
- Pages: read 3 of 3 (footer: "of 3").
- Directives listed: 7. Dates: 1 copied, 2 proposed, 3 not computed.
  Hearings: 2.
- Rule file: Tallis Marrow LLP order deadline rule file, dated 1 October
  2026, review by 31 March 2027, covers this court. In date on 9 November
  2026.
- Closure list: dated 1 October 2026, covers 1 October 2026 to 31 December
  2027. Every proposed date falls inside it.
- Counting: with a calculation tool. Recount on a calendar before the
  attorney confirms.
- Every date above appears in the order on the page cited or is a proposed
  date with its working. No other date appears.

Confirmed by: ____________  Date: ________
Until this line is signed, this is a draft and no date in it is final.
```

## What was observed

**Every required part was produced.** The note to the legal assistant, the draft marking, all the headings, the attorney-to-confirm list, the check block and the confirmation line are there. Both directives outside the numbered list were found, the one in footnote 1 and the one in the discussion on page 2. Dates were counted from the entry stamp, not the signature date. The count that lands on Thanksgiving moved forward past four closed days to Monday 30 November 2026. Nothing was sent, calendared or changed.

**The run and the published example now agree on every date.** Two proposed (16 and 30 November 2026), one copied, three not computed, seven directives, two hearings. The meet and confer got no proposed date: the instructions now say a sentence is mixed when it also holds a count of another kind, even for a different task, and the invented rule file says the same. That costs the attorney one date that rule R-1 would have covered had the court written two sentences. It is the cautious side, and the template says so.

**Differences from the example's output that remain.** They are wording, not dates. The run counted with a calculation tool and its check block says so; the example shows counting day by day. The run's lines for who must do what are a little longer than the example's. Both name 11 November as a closed day inside the count that is counted; the instructions require naming only a closed day that moved the last day, so another run could leave that out.

**Places where the instructions still leave a choice.**

- *What counts as a directive.* "The objection is overruled" and "an award of expenses is appropriate" are rulings that tell nobody to do anything. They were left out, as the example leaves them out, but "when unsure, include it" could pull them in. Including them would do no harm.
- *How wide "mixed" reaches.* The definition names counts of another kind and the word "whichever". A sentence that holds a covered count and merely mentions a hearing, with no count from it, is not named. This run would have treated such a sentence as covered; a firm that wants it sent to the attorney should say so in its rule file.
- *A moved hearing.* The order vacates one conference and sets another. The run listed one VACATED line and one SET line and counted two hearings. The format has no separate word for "moved".
- *The short label on a "Not computed" confirmation line.* The format says "[what is due]"; the run shortened it to a few words.

**Using it.** The instruction block does not contain the output format; the template tells the person to paste the format and its five fill-in lines after it, and the block now tells the assistant to ask for the format if it is missing. That request was not exercised here, because the format was supplied.

**Shortcomings of this trial.** It is one run, on one invented order that was written to fit the template, by the session that had just revised the template and the example, with the example's output in view. None of the stops was exercised: no missing page, no missing footer, no proposed or unsigned order, no signed order without an entry date, no caption mismatch, no rule file past its review date, no request to send. The template's own acceptance tests have not been run. No attorney reviewed the output, and the legal assistant's recount on a calendar, which the template relies on, was not part of the run.
