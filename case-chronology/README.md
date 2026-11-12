# Case chronology from the matter documents

From the document set the handling attorney approved, the paralegal or associate prepares a draft chronology for that attorney: each event with its source and Bates number or page, document dates kept apart from event dates, conflicting accounts side by side, and the gaps. What matters is left to the attorney.

*Workflow template · Law firms · Legal and contracts · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/case-chronology/)*

## The outcome

The handling attorney opens one draft and reads the matter in order. Every entry says who did what and when, quotes the words the document uses, and gives the Doc ID and the Bates number or page where those words sit, so any line can be checked against its page. The attorney’s time goes to reading and judging, not to assembling.

The chronology is careful in the places that usually go wrong. A memo written on Thursday about a Tuesday meeting puts the meeting on Tuesday and keeps Thursday as the memo’s own date. A meeting recorded in an email and a report becomes one entry with both sources listed. “Early April” stays “early April”, and “last Thursday” waits for the attorney instead of being turned into a date. When two documents disagree, both accounts stand side by side and neither is preferred.

It is preparation, and it stays preparation. It gives no legal advice. It decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines. It sends, files, signs and calendars nothing. It never marks an event as helping or hurting either side, never calls one key, and never fills a gap with what probably happened. Anything other than a letter or email is written as what its document records, never as fact. Relevance and significance are the attorney’s. It never says the draft is correct, complete or ready to sign. Asked for a view, whether an event helps, what to do, whether the draft can be signed or to add a case, it says that is for the attorney, names the attorney, points to the line of the draft where the attorney decides it, and says nothing more.

## Who starts the work, and when

A paralegal or associate at a law firm starts it when the handling attorney asks for a chronology and has approved the set of documents to build it from. An in-house team uses it the same way: the paralegal or legal operations lead prepares it for in-house counsel, or, where the company has no lawyer of its own, for the outside counsel on the matter. Then it is addressed to that outside counsel and is never an answer for the business to act on.

Before it reads a single document, it asks how the set was screened for privilege, by whom and when, and records the attorney’s answer word for word. It also asks whether any document came from the other side or another proceeding and whether the attorney has confirmed it may be used. Without those answers it prepares nothing. It is not for writing a statement of facts or a witness outline, deciding whether a document is privileged, working out a limitation date, or keeping a project’s delay timeline.

## What they supply

- **The attorney’s instruction:** the matter, the handling attorney, the approval of the document set and its date, and the period to cover.
- **The attorney’s two answers:** how the set was screened for privilege, with any documents not yet screened, and whether documents from elsewhere may be used.
- **The document index,** exported with the columns Doc ID, Bates start, Bates end, Type, Date, From, To and Custodian. If a header differs, the workflow template stops and asks how the columns match.
- **The documents,** every page, with readable text.
- **The earlier version,** when the chronology is being rebuilt.
- **Today’s date,** and the firm’s settings if it has them: the gap length worth listing (30 days unless the firm sets another) and how numeric dates in its documents are read.

## What comes out

One draft, headed for the named attorney to verify, marked as not legal advice and as deciding nothing about legal meaning, merit, validity, privilege, conflicts or deadlines, and saying that nothing has been sent, filed, signed, shared or calendared:

- **Events,** in date order. Each has the event date, the document date, the quoted words and the place, with every source of a merged event listed and every entry from an unscreened document marked.
- **Dates to place:** events whose documents give only a relative or partial date, left as written for the attorney.
- **Conflicting accounts,** quoted side by side and not resolved.
- **Gaps:** long stretches with no dated event, documents referred to but not in the set, and missing Bates numbers or pages.
- **Sources:** one line per document, with any legend copied as printed and its privilege-screening status in the attorney’s words: screened, not yet screened, or not stated in the attorney’s answer. A status the answer does not give is never guessed.
- **Changes** since the earlier version, when there is one.
- **Attorney to verify:** one line for each point the attorney must confirm, from merged entries to who may receive the chronology.
- **Check:** what was read, and confirmation that no date was counted and no event was ranked.

An empty section says “None.” The paralegal or associate spot-checks the draft against the documents and gives it to the handling attorney, and to no one else.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Legal and contracts](https://fullypowered.ai/functions/legal-and-contracts/): in-house teams build the same chronology on a business dispute, for in-house counsel or for the outside counsel they instruct.
- [Law firms](https://fullypowered.ai/industries/law-firms/), where paralegals and associates assemble a chronology on nearly every disputed matter and the attorney would rather read it than build it.
- [Insurance](https://fullypowered.ai/industries/insurance/), where a disputed claim is pieced together from adjusters’ notes, letters, reports and payment records.
- [Construction](https://fullypowered.ai/industries/construction/), where a payment or defects dispute rests on site records, delivery notes and years of correspondence. This is a record for the lawyer, not the project’s own programme.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where every dispute has a long trail of email and files behind it.

When an order arrives on the same matter, [court-order deadline notice preparation](https://fullypowered.ai/workflows/court-order-deadline-notice-preparation/) prepares the notice the attorney confirms. [Matter-opening checklist preparation](https://fullypowered.ai/workflows/matter-opening-checklist-preparation/) records who is on the matter before any of this starts.

## What has to change for your company

The attorney decides the parts that carry judgment. Name who may approve a document set and answer the two opening questions: the handling attorney alone, or also a supervising attorney. Fix, once and in writing, how your review platform’s or folder’s export maps to the index columns. Set the gap length worth listing and, if your attorneys agree one, the convention for numeric dates. Add the words your firm prints on attorney work in draft. Decide where the verified chronology is kept, how versions are numbered, and who decides who may receive it.

We sit with the paralegals who build your chronologies and the attorneys who rely on them, write down how the work is really done, and set it up in the AI product your firm or company has approved: ChatGPT, Claude, Copilot or Gemini. Check your own policy, and any order covering documents from the other side, before matter documents go into it.

## What has been checked

Fully Powered AI wrote this workflow template, and it was editorially reviewed on 11 November 2026. It has not been reviewed by a lawyer. It was tried on its invented example in Claude on 11 November 2026, and the record of that run is published with the template. It has not yet been tested in a client environment, and it has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing at your firm means running it on a closed matter whose chronology an attorney already settled, with cases written in advance: a memo dated after the meeting it records, an email that says “last Thursday”, two records of one meeting that disagree, a Bates number missing from the run, an unanswered privilege question, and a request to say which events help. The attorney checks every entry before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Court-order deadline notice preparation](../court-order-deadline-notice-preparation/)
- [Matter-opening checklist preparation](../matter-opening-checklist-preparation/)
- [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
