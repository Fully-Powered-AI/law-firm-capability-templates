# Referral source follow-up: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Sonnet 5.5 (claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs were the invented example in `public/example.md` (Elena, Marcus Q., Accounting Firm B, the settings, contact record, relationship history, approved materials list and lunch notes of 3 November 2026). No client data was used. This is the second recorded run. After a pre-review, the instruction block, the output format and the example were revised in small ways (rules for missing inputs, declines, channels and sign-off added to the block; a qualifier added to the client or matter category; one separator named for the log line; the example's thanks line, held-back list and log line changed). I re-ran the revised block on the unchanged inputs and replaced the earlier record with this one. The first run's findings are summarised below where they led to a change.

Limits of this run: the model that made the revisions made this run, and it had already read the example and the first record, so it is not an independent check and the wording of the output may have been influenced by them. I did not run the acceptance tests.

After this run, a fresh review's minor points were applied to `member/template.md` as wording clarifications (numbered advertising categories, two added date conversions, one sentence each on overlap, declined answers and naming a contact's promised list, and an aligned log-line rule, plus the format line `restated. [Overlaps E[n].]`). They do not change the example's inputs or its expected output, and the run was not repeated; the output and observations below are those of the second run, unaltered.

## What came out

**REFERRAL SOURCE FOLLOW-UP: Marcus Q., Accounting Firm B**

- Conversation: Tuesday 3 November 2026, lunch, Elena and Sam (Firm A); Marcus (Accounting Firm B). Prepared Wednesday 4 November 2026 for Elena.
- Contact: Referral source. Preferred name Marcus. Preferred channel email.
- Follow-up due by: Thursday 5 November 2026 (2 working days after the conversation).
- Status: READY FOR THE PARTNER'S REVIEW.
- For the partner: F2, F3, F4, P1, E1, Q1

PROMISES MADE

Firm side:

- F1. Elena to send the sale-readiness checklist, no date stated. Notes: "I said I'd send him our sale-readiness checklist and the corporate team one-pager." In the draft: kept: "Selling your business: a readiness checklist (2026)" attached.
- F2. Elena to send the corporate team one-pager, no date stated. Notes: "I said I'd send him our sale-readiness checklist and the corporate team one-pager." In the draft: left out, needs the partner: approval ended Saturday 31 October 2026.
- F3. Elena to get Marcus the number of sales the firm did this year, no date stated. Notes: "Said I'd get him the number." In the draft: left out, needs the partner: a figure about the firm's work (advertising category 1).
- F4. Elena to introduce Marcus to Priya at Bank D, no date stated. Notes: "I said I'd introduce him to Priya at Bank D, who does acquisition lending, once I've checked with her." In the draft: left out, needs the partner: the introduction is not confirmed with the third person.
- F5. Sam to send the date of the January succession planning seminar, no date stated ("once it's fixed"). Notes: "Sam will send him the date of our January succession planning seminar once it's fixed." In the draft: restated. Overlaps E1.

Contact side:

- C1. Marcus to send a profile of the businesses, Friday 13 November 2026 ("by end of next week"). Notes: "Marcus will send me a profile of the businesses (rough sizes and sectors, no names) by end of next week." Check back: Monday 16 November 2026.

Possible, not promised:

- P1. A joint session for Marcus's clients in the spring. Notes: "Maybe a joint session for his clients in the spring?" Partner confirms whether it is a promise.

Earlier promises still open:

- E1. 2026-06-18: Elena to send seminar dates when the autumn programme is set, from the relationship history. Needs the partner: say whether it was kept.

NEXT STEP

1. A call when his list comes in. Notes: "Suggest a call when his list comes in." Chosen.
2. A joint session for his clients in the spring. Notes: "Maybe a joint session for his clients in the spring?"

Chosen: 1

FOR THE PARTNER BEFORE SENDING

Held back from the draft:

- H1. Marcus's comment on the share sale for Client C, and that Client C is pleased: client or matter.
- H2. That four of Marcus's clients are thinking of selling in 2027: client or matter.
- H3. Accounting Firm B's planned merger in the spring: told in confidence.
- H4. Marcus's daughter starting university: personal.
- H5. The name of the Bank D contact: third person not yet asked.

Advertising checklist, sentences in the draft that touch it:

- None.

Questions recorded, not answered:

- Q1. "He asked whether earn-outs are taxed differently after this year's changes."

DRAFT for Elena to review, edit and send

Channel: email
To: Marcus, Accounting Firm B
Subject: Thank you for Tuesday's lunch

Hi Marcus,

Thank you for lunch on Tuesday 3 November.

I have attached "Selling your business: a readiness checklist (2026)".

Sam will send you the date of our January succession planning seminar once it is fixed.

Once your profile of businesses arrives, I suggest we arrange a call.

Best wishes, Elena

Body words: 46 of 180

PROPOSED LOG LINE, for the person who keeps the relationship record

Date | Type | Firm person | Summary | Open promise
2026-11-03 | Lunch | Elena; Sam | Referral catch-up lunch; readiness checklist sent | Elena: corporate team one-pager (F2); Elena: sales figure (F3); Elena: introduction, third person not yet asked (F4); Sam: January seminar date (F5, overlaps E1); Marcus: business profile by 2026-11-13 (C1); Elena: seminar dates from 18 June (E1)

Prepared for Elena's review. Nothing has been sent, recorded or promised on the firm's behalf.

## What was observed

Every required part was produced and I was never told to stop. The dates, the promise list, the held-back list, the question, the status and the word count all came out of the instructions without needing outside facts. Every fact in my output is in the inputs.

Compared with the first run:

- The qualifier on the client or matter category and the sentence about a contact's own clients' plans settled the first run's one real defect. This time the held-back list and the example agree: the note about four of Marcus's clients selling is held back (H2) and appears in neither the thanks line nor the log line. The example was changed to match.
- The log line header and entry both use bars, as the block now says. The first run used commas in the header.
- The sign-off is "Best wishes, Elena" on one line, as the settings give it.
- F2 gives only the reason, as the block now says.
- Splitting the one notes line that holds two promises (F1 and F2), converting "end of next week" to Friday 13 November, treating the deal count as a promise (F3) and not a Q item, and marking F5 as overlapping E1 were each settled by a sentence in the block rather than by my own reading.

Differences from the published example, all matters of wording:

- My draft is shorter (46 words against 56), has no "As promised" or "could we", and has a different subject line.
- The example's log summary and mine differ in wording; neither holds back anything it should not.
- Everything else matched: the same promises, the same dates, the one-pager left out for an ended approval, the sales figure left out under advertising category 1, the introduction left out, the seminar date restated, the spring session as a possible and a second next-step option, the earn-out question recorded and unanswered, and the same list of items for the partner.

## Ambiguities and shortcomings that remain

- **Overlap.** Whether Sam's January seminar date (F5) "covers the same thing" as Elena's June promise of seminar dates (E1) is a judgement. I marked it as overlapping; another reader might not.
- **Declined answers.** "Told him I'd rather not answer off the cuff" is not a promise and the template says nothing about declined answers. I treated it as part of Q1.
- **Next-step dependence.** Step 5 lets the draft mention a contact's promise when the next step depends on it. How much to say about the list ("profile of businesses") is left to the writer, and the phrase could itself hint at the clients' plans.
- **Test coverage.** The proposed acceptance tests are untouched by this trial; I ran only the example.

Overall: the instructions are workable on this input and gave a complete, cautious output.
