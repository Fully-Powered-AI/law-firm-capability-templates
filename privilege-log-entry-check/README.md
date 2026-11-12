# Privilege log entry check

Before a draft privilege log goes to review counsel, the paralegal gets an entry-by-entry check against counsel’s approved format and role map, and a list of logged documents’ attachments with no entry. It checks metadata only: review counsel makes every privilege call and writes or approves every description.

*Workflow template · Law firms · Legal and contracts · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/privilege-log-entry-check/)*

## The outcome

Review counsel opens a log whose housekeeping has already been checked line by line. Every entry has been held up against the review platform’s own record: the document ID, the date, the type, the author, every recipient down to the BCC line, each person’s role as counsel’s role map records it, the treatment counsel designated, and each attachment tied to its parent. The email logged with an entry for only one of its two attachments, the memo designated for withholding that has no entry, the person on a BCC line nobody has mapped: each one is found before the log leaves the firm, and each one is a line for counsel to answer.

The line it holds is the one that matters. The check gives no legal advice and decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines. It never says or hints whether a record is privileged, never treats a lawyer’s name as a reason for anything, never reads a description for meaning, never judges or copies it, and never copies a subject line or a word of any document. It never states, counts or estimates the date a log is due. It never names a case, statute or rule from memory; an authority anyone raises is left to be verified by the lawyer. It edits, serves, sends, files, signs and calendars nothing. Everything it produces is a draft for review counsel, with a line for each point counsel must confirm.

## Who starts the work, and when

The paralegal or litigation support specialist assembling the log starts it once review counsel has designated the withheld and redacted records and a draft log exists, and runs it again after each round of corrections. Review counsel, the responsible attorney for the review, decides and signs. In a company running its own review with no lawyer of its own, that is outside counsel, and the check is addressed to outside counsel, never to the business as an answer.

It is not for deciding what to withhold, writing descriptions, reviewing documents or serving the log.

## What they supply

- **The draft log**, exported as a spreadsheet, with the columns counsel’s format names.
- **The designation export** from the review platform: each designated record and the rest of its family, with ID, family, parent, attachment count, date, type, author, recipients and counsel’s designation.
- **Counsel’s role map**: every person who may appear on the log, with the role counsel has given them.
- **Counsel’s approved log format**: the columns and which are required, the ID pattern, the date form, how names and counsel are marked, the permitted treatments and basis codes, and how attachments are logged.
- The matter, the case number and the name of review counsel.

The workflow template ships no log format, no role list and no rules about privilege. It uses what the firm and its review counsel supply, with a few fallback defaults for layout (dates written year-month-day, names separated by semicolons, a star after counsel’s names) that counsel’s format overrides. If the format does not say how attachments are logged, it stops and asks. If a column heading does not match, it stops and asks which column holds what.

## What comes out

One draft check, headed as a draft for review counsel:

- **Entry by entry:** each entry marked complete or incomplete, with one plain line per problem: what the log says and what the export, format or role map says. Values are metadata only; a description shows only as filled or blank.
- **Attachments of logged documents with no entry:** every attachment of a logged document that has no entry of its own, with its date, type, author and designation as the export records them. One with no designation recorded is marked for review counsel to decide; the check never says whether it belongs on the log.
- **Designated records with no entry,** **entries with no matching designation,** and **people not on the role map.**
- **Review counsel to confirm:** a line to confirm, decide or supply for every problem found, and the lines saying every privilege call and description is counsel’s and the log is approved for service.
- **Check:** the counts, and a sum proving every designated record is either on the log or on one of the lists.

The paralegal checks the metadata lines, then gives the log and the check to review counsel. Counsel answers every line and approves the log. Only then do people serve it.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Legal and contracts](https://fullypowered.ai/functions/legal-and-contracts/): a log is a record counsel signs, and this check holds its metadata against the review platform and counsel’s approved format before counsel sees it.
- [Law firms](https://fullypowered.ai/industries/law-firms/), in litigation groups where logs run long and each entry is checked against the review platform and counsel’s format before an attorney signs.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where one senior paralegal knows how the firm checks a log and nobody has written it down.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when reviews grow faster than the team that builds the logs.

It sits beside [court-order deadline notice preparation](https://fullypowered.ai/workflows/court-order-deadline-notice-preparation/), which turns an entered court order into a draft notice for the attorney to confirm, and [outgoing work sign-off log](https://fullypowered.ai/workflows/outgoing-work-sign-off-log/), which tracks the attorney’s sign-off before the log leaves the firm.

## What has to change for your company

Review counsel’s format and role map are the measure, and they are yours. Counsel decides the columns, which are required, how a document ID looks, how dates and names are written, how counsel are marked, which treatments and basis codes are allowed, and whether an attachment gets its own entry. Decide who keeps the role map and how aliases are added, which saved search in your review platform produces the export, and whether staff may correct dates and names from the export before counsel sees the check.

We sit with the paralegal who builds your logs and the attorney who signs them, write down how a log is really checked, and set it up in the AI product the firm has approved: ChatGPT, Claude, Copilot or Gemini. Confirm with your own policies, and with counsel on any protective order, that the log and export may be used there.

## What has been checked

Fully Powered AI wrote this workflow template from its own published map of law-firm work, and it was editorially reviewed on 11 November 2026. It has not been reviewed by a lawyer. It was tried on its invented example in Claude on 11 November 2026, in a run after the last of that day’s revisions, followed by seven tests that asked for a verdict, a case, a due date and advice for a business with no lawyer, and that planted an instruction in the log, an instruction in the role map and an invented rule. The record of that run is published with the template, and the instructions and output format published are the ones that were run. It has not yet been tested in a client environment, and it has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing at your firm means running it on a past log counsel has already approved, with problems planted in advance: an attachment with no entry, a transposed date, a dropped BCC, a missing counsel marker, an entry for a record designated for production, a renamed column, a description holding an instruction to the assistant. Review counsel checks every line before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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
- [Outgoing work sign-off log](../outgoing-work-sign-off-log/)
- [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
