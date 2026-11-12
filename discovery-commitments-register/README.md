# Discovery requests and commitments register

Through discovery, the litigation paralegal keeps one register for the handling attorney: each request and its response in the exact words served, the Bates ranges produced against it, every supplement promised in correspondence with its date as written, and the promises now overdue. The attorney decides what it means.

*Workflow template · Law firms · Legal and contracts · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/discovery-commitments-register/)*

## The outcome

The handling attorney opens one register and sees the whole written discovery on a matter, request by request. Each request is quoted with its page, and under it every response, amended and supplemental ones included, word for word with the date served. Then come the productions logged against it with their Bates ranges, every promise of more documents or an amended response made in a letter, an email or on a call, and every passage about narrowing what the request covers, each with the side that wrote it. A short list at the end shows the promised supplements whose stated date has passed with nothing recorded since. The promise someone made on a call six weeks ago is on the page, with the words used and whether the other side ever put it in writing.

**What it does not do.** It gives no legal advice. It decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines. It sends, files, signs and calendars nothing. It quotes and locates; it never characterises. Nothing is called deficient, evasive, late, misconduct or bad faith, and it never says whether a response or a production is complete. It writes no deficiency argument, proposed order, conferral letter, follow-up email or motion, even for the attorney to edit. It counts no deadline: a promised date is copied exactly as written, and words like "within two weeks" are left uncounted for the attorney. It names no case, statute or rule from memory; one quoted in a paper is copied as written, marked to be verified by the lawyer and given its own line for the attorney. Everything it prepares is a draft for the handling attorney, with a line for each point the attorney must confirm.

## Who starts the work, and when

The litigation paralegal or litigation support specialist runs it while written discovery is under way: after responses are served, after each production, after each conferral letter, email or call, and before the attorney's regular look at the matter. The handling attorney decides and signs. In a company's legal team that is the in-house counsel handling the case. In a company with no lawyer of its own, the register is prepared for outside counsel on the case and goes to that counsel, never to the business as an answer.

It is not for a records request sent to a client during an advisory engagement: [client document request tracker](https://fullypowered.ai/workflows/client-document-request-tracker/) does that work.

## What they supply

- **The request:** the matter, the case number, the party you act for, the handling attorney, the as-of date, the request sets to include, and any entries the attorney has closed.
- **The request sets and the responses**, as served, every page, with each certificate of service. Amended and supplemental responses too.
- **The production log**, as a spreadsheet, one row per production volume, with the Bates range and the requests the cover letter names. If a column heading does not match, it stops and asks which column holds what.
- **The correspondence and notes:** every letter and email between the parties about the requests, and your own notes of calls and meetings, each with its date and the people on it.

The workflow template reads nothing else: no court rules, nothing remembered, nothing from another matter. It reads the production log, not the documents produced.

## What comes out

One draft register, headed as a draft for the handling attorney:

- **Request by request:** each request and its responses in their own words, with page and date served, the productions logged against it, the promises and passages about scope, and whether the attorney has closed it.
- **Promises in correspondence:** each promise of further documents, an amended or supplemental response or a privilege log, in the words used, with where it was made, whether it is in a document from the promising side or only in your own call note, the date exactly as stated, any condition in the wording, and what has been recorded since.
- **Conferral history:** every letter, email, call and meeting in date order, with the passages about each request quoted.
- **Promised supplements now overdue:** each promise with a stated calendar date before the as-of date and nothing recorded against the request since, listed by the party that made it, with any later production whose cover letter names no request.
- **Items still open,** and **anything not tied to a request,** such as a production volume whose cover letter names none.
- **Attorney to confirm:** a line for each promise, each scope question, each closure and each loose end, ending with the line that leaves every judgement about the responses, and any follow-up, to the attorney.
- **Check:** the counts, and a sum proving every promise has exactly one standing.

The paralegal checks each quotation, page and Bates range against the papers and gives the register to the handling attorney. The attorney answers each line and decides whether anything follows. Any letter, call or motion is the attorney's, and people write and send it. The register stays in the matter file; it is not for the client or the other side.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Legal and contracts](https://fullypowered.ai/functions/legal-and-contracts/): discovery is litigation work the legal team owns, and this register keeps its record, request by request, for the attorney who decides.
- [Law firms](https://fullypowered.ai/industries/law-firms/), in litigation groups where several request sets run at once and a promise made on a call is easy to lose by the following month.
- [Insurance](https://fullypowered.ai/industries/insurance/), where claims litigation runs through outside firms and in-house counsel wants each matter's discovery record in the same shape.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where product and supply disputes bring requests for batch records, test reports and supplier correspondence that arrive across many productions.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where one experienced paralegal keeps the discovery record in a spreadsheet nobody else can read.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when the matters in discovery grow faster than the litigation support team.

It sits beside [deposition transcript summary](https://fullypowered.ai/workflows/deposition-transcript-summary/) and [privilege log entry check](https://fullypowered.ai/workflows/privilege-log-entry-check/) in a litigation team's discovery work. Dates set in a court order belong to [court-order deadline notice preparation](https://fullypowered.ai/workflows/court-order-deadline-notice-preparation/), not to this register.

## What has to change for your company

The production log is yours, and it is the heart of this. Decide who keeps it, what its columns are called, and the rule that it records only the requests a cover letter names, never anyone's view of what a production answers. Decide which notes of calls and meetings go in with the correspondence and who writes them, how the attorney records that an entry is closed, and where the register is kept in the matter file and who may read it, since it holds your own notes of calls. If the firm already numbers its discovery its own way, set those codes once and keep them on every run.

We sit with the paralegal who keeps your discovery record and the attorney who relies on it, write down how it is really kept, and set it up in the AI product the firm has approved: ChatGPT, Claude, Copilot or Gemini. Confirm with your own policies, and with counsel on any protective order, that the papers may be used there.

## What has been checked

Fully Powered AI wrote this workflow template in its own words, drawing on a published discovery tracking method credited in its sources, with that method's deficiency findings, proposed cures, sanctions flags and deadline counting taken out. It was editorially reviewed on 11 November 2026. It has not been reviewed by a lawyer. It was tried once on its invented example in Claude on 11 November 2026, and the record of that run, which replaced two earlier ones from the same day, is published with the template. It has not yet been tested in a client environment, and it has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing at your firm means running it on a past matter whose discovery your attorney already knows, with hard cases planted in advance: a response that answers two requests together, an amended response, a promise made only on a call, the same promise repeated in an email, "within two weeks", a promise with a condition, a production whose cover letter names no request, and a request to say whether a response is deficient. The paralegal checks every quotation and date against the papers before the attorney relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Deposition transcript summary](../deposition-transcript-summary/)
- [Privilege log entry check](../privilege-log-entry-check/)
- [Court-order deadline notice preparation](../court-order-deadline-notice-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
