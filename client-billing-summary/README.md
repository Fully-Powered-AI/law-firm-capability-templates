# Client billing summary

Before an invoice goes out, the billing coordinator has a summary the client can read: fees by timekeeper, task and phase, expenses and write-downs, tied to the pre-bill. Every entry that breaks the client's billing guidelines reaches the responsible attorney as a decision, with the amount at stake.

*Capability template · Law firms · Finance and accounting · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/client-billing-summary/)*

## The outcome

In a fully powered firm, invoices go out right the first time. The client opens a clear account of the month: who worked, on what, at which stage of the matter, and what it cost. The firm finds the entries the client's billing rules would refuse before the client's reviewers do, so fewer invoices come back with deductions and fewer weeks pass between sending and payment. That is 10X what your billing team can do with the hours it has.

The capability prepares two things from the pre-bill. The first is the summary for the client, written from the time entries in plain words, with every total tied to the pre-bill. The second is a review for the responsible attorney alone: each entry that breaks a guideline, with the section, the facts and the amount affected, and each time entry description that says more than an invoice should, such as a settlement position. The attorney decides every one. The capability writes nothing down, changes nothing in the billing system and sends nothing.

## Who starts the work, and when

The billing coordinator runs it as soon as the pre-bill for a matter is generated, so the responsible attorney reviews the flags and the client summary at the same sitting. It runs again from the updated pre-bill once the attorney's decisions are entered. It comes before the invoice goes out: chasing an unpaid invoice afterward is [Overdue-invoice follow-up preparation](https://fullypowered.ai/capabilities/overdue-invoice-follow-up-preparation/), and a matter's billing terms are captured earlier, in [Matter-opening checklist preparation](https://fullypowered.ai/capabilities/matter-opening-checklist-preparation/).

## What they supply

- **The pre-bill** for the matter and period, with its totals.
- **Three exports from the billing system:** the time entries, the expenses, and the write-downs and discounts already decided. The template names the column headings it expects and stops to ask when one does not match.
- **The client's billing guidelines:** approved timekeepers and rates, task and phase codes, limits, expenses the client will not pay, and any budget.
- **The matter's settings:** the responsible attorney, and the fees billed before this invoice, for the budget check.

## What comes out

One document in two parts. Part A, for the client once the attorney approves it: an overview of the period with the totals, then fees by timekeeper, by task and by phase, the expenses with subtotals, and the write-downs with the note the firm chose for the client. Part B, never sent: the tie-out to the pre-bill, the guideline rules checked and those that cannot be checked from the exports, the budget position, the numbered flags with a question for the attorney on each, and the descriptions to reword before the itemized detail prints.

If the exports do not add up to the pre-bill, nothing is drafted until the billing coordinator finds why. A good result lets the attorney clear the month's billing in one review, with no surprises from the client afterward.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Law firms](https://fullypowered.ai/industries/law-firms/): the monthly step between the pre-bill and the invoice, for clients whose billing rules are strict.
- [Finance and accounting](https://fullypowered.ai/functions/finance-and-accounting/): the billing team owns the pre-bill, the exports and the tie-out.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/): when more clients arrive with their own billing rules than one billing coordinator can hold in their head.

## What has to change for your company

1.  **Your exports.** Map your billing system's column headings once, so every run reads them the same way.
2.  **Your house rules.** Add the checks your firm runs on every matter, whatever the client's guidelines say, such as a daily-hours limit or work the firm never bills.
3.  **Who does what.** Name who rewords a flagged description, who enters the attorney's decisions, and who sends the invoice, by email or through the client's billing portal.

We set this up with the billing coordinator and a responsible attorney, on past months your team remembers. This capability template is written for ChatGPT, Claude, Copilot and Gemini, and your firm keeps control of how the work gets done.

## What has been checked

Fully Powered AI wrote this capability template, drawing on a published billing summary method credited in its sources. It was editorially reviewed on 10 November 2026. It was tried on its invented example on 10 November 2026 in four runs; the instructions were revised after each of the first three, and the record of the fourth is published with it. That run did not reach any stop condition. After that run only the example's own output was edited, to agree with the instructions; the instructions were not changed. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your firm means running it on two or three past pre-bills whose client deductions you already know, plus hard cases written in advance: exports that do not add up to the pre-bill, a rate above the approved rate, two people billing the same internal meeting, a description that names a settlement position. The billing coordinator checks every figure against the pre-bill before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) builds that test set, and [What we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) shows the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete capability template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the capability drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related capabilities

- [Overdue-invoice follow-up preparation](https://fullypowered.ai/capabilities/overdue-invoice-follow-up-preparation/)
- [Matter-opening checklist preparation](../matter-opening-checklist-preparation/)
- [Weekly receivables summary](https://fullypowered.ai/capabilities/weekly-receivables-summary/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
