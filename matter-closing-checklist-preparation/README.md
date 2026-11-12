# Matter closing checklist preparation

When the handling lawyer flags a matter for closure, the firm's closing checklist is filled from the matter record: final billing as recorded, open tasks, unreturned items and the handoffs billing and records must accept.

*Workflow template · Law firms · Operations and process improvement · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/matter-closing-checklist-preparation/)*

## The outcome

A matter does not leave the active list with loose ends nobody saw. The person closing the file opens one page that shows what the records say: how the lawyer says the matter ended, what billing still shows as open, which tasks are unfinished, which client documents and property have not gone back, and which handoffs have not been accepted by the people who must accept them.

The page also keeps visible the things that should not be tidied away: a related proceeding, an obligation the lawyer says is still running, a hold instruction. Every figure is added up from the exports, so billing and records see the same numbers the operations team sees.

The responsible attorney still decides whether the matter can close. Records owners still decide how long a file is kept. The checklist writes down the outcome the attorney supplied without judging it, sets no retention period, works out no legal deadline and gives no legal advice.

## Who starts the work, and when

The operations or records assistant starts it when the handling lawyer flags a matter for closure. The assistant runs it again each time an item is cleared, with the previous checklist supplied, so the page always shows what is left.

The responsible attorney reads the outcome line and decides whether the matter can close. The billing coordinator and the records clerk each look at their own handoff and accept it or send it back.

## What they supply

- **The closure flag.** The matter number, who flagged it and the date.
- **The attorney's outcome note.** How the matter ended, in the attorney's words, with the final order or agreement named, and any related proceeding, running obligation or hold instruction.
- **The matter record, tasks and billing exports** from your practice system, with the default column headers listed in the template. If a header does not match, the workflow template stops and asks.
- **The unreturned-items list** kept by records.
- **The firm's own closing checklist,** with who owns each item and which items are handoffs.
- **The previous checklist (optional),** on a rerun, so the new version can show what changed.

It works from supplied files and needs no connection to your practice system and no sign-in details.

## What comes out

One checklist in a fixed order: the matter, the outcome as the attorney stated it, the final billing status as recorded, open tasks, unreturned items, each line of the firm's checklist with its status, the handoffs awaiting acceptance, and the items kept explicit. Under the last line it states who decides closure and who decides retention, and what the next action is.

Good means the records clerk can accept or return the handoff without phoning anyone, and the attorney sees in one minute what stands between the matter and closure.

It is a different piece of work from [Matter-opening checklist preparation](https://fullypowered.ai/workflows/matter-opening-checklist-preparation/), which sets a matter up, and from [Weekly open-matter check](https://fullypowered.ai/workflows/weekly-open-matter-check/), which watches every open matter; this one prepares the end of a single matter. Billing figures that feed it can come from [Client billing summary](https://fullypowered.ai/workflows/client-billing-summary/).

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Law firms](https://fullypowered.ai/industries/law-firms/): the step between the attorney's decision to close and the file leaving the active list.
- [Professional services](https://fullypowered.ai/industries/professional-services/): engagement closure with billing and records handoffs.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/): project close-out, with drawings and client property returned.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/): the handoff crosses attorney, billing and records, and a checklist keeps all three on one page.
- [Finance and accounting](https://fullypowered.ai/functions/finance-and-accounting/): final invoices, unbilled time and funds held are shown as recorded before billing accepts the file.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/): a closing routine that lives in one clerk's habits is moved onto a page.

## What has to change for your company

1. **Your closing checklist.** The items, who owns each, and which are handoffs to billing, records or matter administration.
2. **Your export headers and status words.** What your system calls an open task, a finished task and an invoice that has been issued.
3. **Who accepts what.** The role that accepts each handoff and how the acceptance is recorded.
4. **Your own rules.** Whether the checklist is reviewed before it is shared, and who may close a matter with items still open.

In professional services and engineering firms the same page serves engagement or project close-out; replace "matter" with the word your firm uses.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 10 November 2026. It was tried on its invented example on 10 November 2026 in three runs: the first found defects and the instructions, output format and example were revised; after an independent review the instructions were revised again in small ways. The record of the third run, made by the model that made the revisions, is published with it. The trial exercised one of the nine acceptance tests. It has not been tested in a client environment or as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your firm means preparing checklists for a few recently closed matters and comparing them with what billing and records found, including a matter with an unpaid invoice, one with client property still out, and one flagged with no attorney outcome, which should stop. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [What we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) shows the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
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

- [Matter-opening checklist preparation](../matter-opening-checklist-preparation/)
- [Weekly open-matter check](../weekly-open-matter-check/)
- [Client billing summary](../client-billing-summary/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
