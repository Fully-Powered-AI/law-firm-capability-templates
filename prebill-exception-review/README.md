# Prebill exception review

Before the billing attorney opens a prebill, the billing coordinator has every awkward entry marked: rates that differ from the firm's rate table, possible duplicates, entries outside the client's billing guidelines, unclear narratives and expenses without support, each sent to the person who acts next.

*Capability template · Law firms · Finance and accounting · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/prebill-exception-review/)*

## The outcome

In a fully powered firm, the prebill review is spent on decisions, not on searching. The billing attorney sits down with one exception sheet for the matter: every entry billed at a rate the firm's table does not show for that date, every pair of entries that look like the same work twice, every entry the client's billing guidelines would refuse, every narrative that is vague, packs several tasks under one time or says more than an invoice should, every expense with no receipt or invoice behind it, and every adjustment entered with no approver or no reason. Each line carries the facts and the amount at stake.

The sheet also does the sorting. Narratives to rewrite or split go back to the timekeeper who wrote them, missing receipts go to whoever submitted the expense, and the decisions on rates, duplicates, guideline breaches and adjustments go to the billing attorney. Your billing team clears a month of prebills with the hours it already has, and the questions reach the right desk the same day.

The capability prepares the sheet and nothing more. The billing attorney decides what is billable and every change to a narrative, finance approves the invoice preparation, and the sheet changes, writes down and sends nothing.

## Who starts the work, and when

The billing coordinator runs it as soon as the prebill for a matter is generated, before the billing attorney's review, and again from the updated prebill once corrections and decisions are entered. It comes before the client ever sees anything: the summary the client reads with the invoice is [Client billing summary](https://fullypowered.ai/capabilities/client-billing-summary/), prepared after the billing attorney's decisions, and a matter's budget and progress for the responsible partner is [Matter budget and status summary](https://fullypowered.ai/capabilities/matter-budget-and-status-summary/).

## What they supply

- **The prebill header:** number, date, client, matter, billing period, billing attorney, and the totals for fees, adjustments and expenses.
- **Three exports from the billing system:** time entries, expenses with their receipt or invoice reference, and the adjustments already entered. The template names the column headings it expects and stops to ask when one does not match.
- **The firm's rate table,** with the agreed client rates and the dates each applies. Rates come from the table only, never from reading an engagement letter.
- **The client's billing guidelines,** or a note that the client has none.
- **The firm's settings,** if it wants its own: the shortest acceptable narrative, the vague phrases and sensitive words to look for, and when an expense needs support.

## What comes out

One exception sheet for the matter. It opens with a tie-out proving the exports add up to the prebill; if they do not, nothing else is prepared until the billing coordinator finds why. Then six sections, each reading "None." when it is empty: rate differences against the rate table, possible duplicates, entries outside the client's guidelines, narratives to clarify, expenses without support, and adjustments without an approver or a reason. Every line has a number, the facts, the amount at stake where there is one, and who has it next.

The sheet closes with the guideline rules it checked and those it could not check from the exports, and a list of who has what: each timekeeper's returns, the billing attorney's decisions, and finance's approval once those are in.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Law firms](https://fullypowered.ai/industries/law-firms/): the monthly step between generating the prebill and the billing attorney's review, for every matter billed by the hour.
- [Professional services](https://fullypowered.ai/industries/professional-services/): any firm that bills time against a client's billing rules, with the engagement partner in the billing attorney's place.
- [Finance and accounting](https://fullypowered.ai/functions/finance-and-accounting/): the billing team owns the prebill, the rate table and the exports.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/): when more matters and more client rulebooks arrive than one billing coordinator can hold in their head.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/): when the prebill checks live in one long-serving coordinator's memory and should live on a page.

## What has to change for your company

1. **Your exports.** Map your billing system's column headings once, so every run reads them the same way.
2. **Your rate table.** Decide who keeps it and how agreed client rates reach it, with the dates they start and end.
3. **Your lists.** Set your own vague phrases, sensitive words and narrative minimum, and whether small expenses need a receipt.
4. **Your house rules.** Add the checks your firm runs on every matter whatever the client's guidelines say, such as a daily-hours limit.
5. **Who answers.** Name who picks up a returned entry when the timekeeper is away or has left.

We set this up with your billing coordinator and a billing attorney, on past prebills your team remembers. This capability template is written for ChatGPT, Claude, Copilot and Gemini, and your firm keeps control of how the work gets done.

## What has been checked

Fully Powered AI wrote this capability template from its own published map of law-firm billing work. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026, and the record of that run is published with it. It has not been tested in a client environment or as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your firm means running it on two or three past prebills whose problems your billing coordinator already found, plus hard cases written in advance: exports that do not add up to the prebill, a timekeeper still billed at last year's client rate, the same entry recorded twice, a day over the client's hours limit, a narrative that names a negotiating position, an expense with no receipt. The billing coordinator checks every line against the prebill before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) builds that test set, and [What we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) shows the record we keep.

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

- [Client billing summary](../client-billing-summary/)
- [Matter budget and status summary](../matter-budget-and-status-summary/)
- [Overdue-invoice follow-up preparation](https://fullypowered.ai/capabilities/overdue-invoice-follow-up-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
