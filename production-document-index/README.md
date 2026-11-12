# Document production index and summaries

From a production review counsel has cleared, the paralegal prepares a draft for that counsel: an index of every document by Bates range, a short summary of each, every statement cited to its Bates page, missing documents and differing passages listed, and anything matching counsel's screen list held by number only.

*Workflow template · Law firms · Legal and contracts · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/production-document-index/)*

## The outcome

Review counsel opens one draft and knows what came in. Every document in the production has a line in the index: its Bates range, pages, type, date, who sent it to whom, its family and any designation stamped on it. Every document that can be read has a short summary that says what the document states, in the order it states it, with the Bates page after every sentence and the exact words quoted. Attachments are linked to the emails that carry them. Where one page names a report or an attachment the production does not contain, that is listed with the words that name it. Where two documents give different times, counts or amounts for the same thing, both passages are quoted side by side. Every Bates number in the cleared range is accounted for, so a gap is found before the review starts. The first read is prepared for the paralegal to check and counsel to review, and counsel's time goes to the judgment only a lawyer can make.

Anything that matches a line of counsel's own privilege screen list is held, with its whole family, and appears in the draft by Bates number only. Nothing from it is summarised, quoted or used anywhere, including in the list of differences.

**What it does not do.** It gives no legal advice. It decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines. It sends, files, signs and calendars nothing. It never says whether a document is relevant, important or privileged, never says what a document means or proves, and never says which of two passages is right. Holding a document because counsel's list matched is not a privilege call; counsel makes that. It writes no letter about missing documents, no request for production, no clawback notice, no privilege log entry and no brief section, even for counsel to edit. It names no case, statute or rule from memory, and any authority named in a document stays inside its quotation, marked to be verified by the lawyer. Asked whether a document is hot, whether it was produced by mistake, what to ask for next or what to do, it says only that this is for review counsel and points to the line of the draft concerned. Everything it prepares is a draft for the named counsel, with a line for each point counsel must confirm.

## Who starts the work, and when

A paralegal or litigation support specialist starts it once review counsel has cleared a production for review in writing, with its Bates range, and has supplied a screen list. Review counsel, the lawyer named in the clearance note, reviews it and decides. In a company with no lawyer of its own, the draft is prepared for the outside counsel on the matter and goes to that counsel, never to the business as an answer.

It is not for deciding which of your own client's documents to produce or withhold; that is counsel's privilege review. A privilege log is checked by [privilege log entry check](https://fullypowered.ai/workflows/privilege-log-entry-check/), a dated story of events is built by [case chronology from the matter documents](https://fullypowered.ai/workflows/case-chronology/), and a deposition is summarised by [deposition transcript summary](https://fullypowered.ai/workflows/deposition-transcript-summary/). A deal room and an audit request list have their own workflow templates: [property diligence index](https://fullypowered.ai/workflows/property-diligence-index/) and [audit evidence index](https://fullypowered.ai/workflows/audit-evidence-index/).

## What they supply

- **Review counsel's clearance note,** in counsel's own words: the matter and case number, the producing party, the production volume, the Bates range cleared, the date, counsel's approval to use the AI product for any designated pages, and the order to arrange the draft in (Bates order unless counsel says by date or by custodian).
- **Counsel's privilege screen list,** dated and approved by counsel: numbered lines of names, firms, email domains and words. The workflow template supplies none.
- **The production export,** as CSV with the columns BegBates, EndBates, BegAttach, EndAttach, Custodian, DocDate, DocType, From, To, Subject and Designation. If a header differs, the workflow template stops and asks how the columns match.
- **The documents,** every page with its Bates stamp and readable text, slip sheets included.

Nothing else is used: nothing remembered, nothing from the internet, nothing from another matter.

## What comes out

One draft, headed for the named counsel to review, saying that it gives no legal advice, decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines, and that nothing has been sent, filed, signed or calendared:

- **Production overview:** counts of documents, pages, summarised, held, slip sheets and not read, the span of dates, the types and the designations.
- **Index:** one line per document, with a held document shown by Bates range and hold number only.
- **Summaries:** what each document says, each sentence cited to its Bates page, with quotations, designation, related documents, missing documents and differences.
- **Held for counsel:** each held family by Bates range and the screen-list line that matched.
- **Missing documents:** each attachment or document a page mentions that the production supplied does not contain, with the words quoted and what was looked for.
- **Passages that differ:** both passages quoted and cited, and the fact they concern.
- **Not read:** pages listed in the export but not supplied, native files not supplied, pages that cannot be read, and anything outside the cleared range.
- **Counsel to confirm:** a line for the Bates accounting, each held family, the summaries, the links, each missing document, each difference, each place the export disagrees with the pages, what was not read, the designations, who may receive the draft and the cite check, and a line saying that documents not held were checked only against counsel's screen list, which is not a finding that they are not privileged.
- **Check:** every Bates number accounted for, where the export disagrees with the pages, and what was compared.

An empty section says so. If pages listed in the export were not supplied, the draft says NOT READY FOR COUNSEL at the top. If the screen list or the clearance note is missing, or the export's headers differ, nothing is prepared until they are supplied.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Legal and contracts](https://fullypowered.ai/functions/legal-and-contracts/): in-house teams receive productions in business disputes and review them with in-house counsel or the outside counsel they instruct.
- [Law firms](https://fullypowered.ai/industries/law-firms/), in litigation groups where a production arrives in the thousands of pages and the review team needs to know what is in it, page by page, before anyone forms a view.
- [Insurance](https://fullypowered.ai/industries/insurance/), where coverage and claims disputes bring productions of adjusters' files, reports and correspondence, and in-house counsel works with outside counsel on each.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where a product or supply dispute brings productions of test records, logs, invoices and plant email that have to be read against each other.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where a long-running dispute builds a document record too large for one person to hold in their head.

It pairs with [case chronology from the matter documents](https://fullypowered.ai/workflows/case-chronology/), which can be built from the documents once counsel has reviewed this draft, and with [privilege log entry check](https://fullypowered.ai/workflows/privilege-log-entry-check/) when the team prepares its own log.

## What has to change for your company

The screen list is counsel's, and it is the heart of this. Review counsel decides its lines: the lawyers and firms on the matter and their email domains, the legends the team prints on its own work, and any words counsel wants held, and redoes it when the people on the matter change. Fix once, in writing, how your review platform's export maps to the default columns. Add the words your counsel never wants to see in a summary, decide who checks the cites and how many, and say where the draft is kept and who may receive it. Counsel confirms that your policy and any protective order allow the production to be used in the AI product you have approved.

We sit with the paralegals and litigation support staff who review your productions and the counsel who rely on their work, on a production they already know well, and set it up in ChatGPT, Claude, Copilot or Gemini. Your team keeps control of how the work gets done.

## What has been checked

Fully Powered AI wrote this workflow template, drawing on a published discovery document summary method credited in its sources. It was editorially reviewed on 11 November 2026. It has not been reviewed by a lawyer. It was tried on its invented example in Claude on 11 November 2026, and the record of that run, which replaced an earlier one from the same day, is published with the template. It has not yet been tested in a client environment, and it has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your team means running it on a past production whose review your counsel already settled, plus hard cases written in advance: an email to a lawyer on the screen list with an attachment that matches nothing, a "see attached" with no attachment produced, two documents giving different times for the same event, a gap in the Bates numbers, a slip sheet for a native file, and a request to say which documents are hot. The paralegal checks the cites against the pages before the draft goes to counsel. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 11 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 11 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete workflow template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the workflow template drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related workflow templates

- [Case chronology from the matter documents](../case-chronology/)
- [Privilege log entry check](../privilege-log-entry-check/)
- [Deposition transcript summary](../deposition-transcript-summary/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
