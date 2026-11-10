# Matter budget and status summary

The responsible partner sees one matter whole: scope, phases against their dates, the budget against fees to date and the projected total, a red, amber or green status with the rule behind it, risks and next actions with owners. Built from the time export and the matter plan, never a view on the merits.

*Capability template · Law firms · Operations and process improvement · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/matter-budget-and-status-summary/)*

## The outcome

The partner walks into the partners' meeting, or the budget call with the client, knowing exactly where one matter stands on money and progress. Every phase sits beside its planned dates and its budget. Fees to date tie to the time export to the dollar, and the projected total comes from the matter lead's own estimate of the work still to come.

The status is not a mood. Red, amber or green is set by rules the firm chooses, and every rule that fired is printed with its figures, so a partner can see in one line why a matter is amber. Overruns surface while there is still time to talk to the client about them, and the questions only the partner can settle are already written out.

The summary reports budget and progress. It gives no view on the legal merits, the likely outcome or strategy; any such line in the notes is left out, and the summary says so. It sends nothing, bills nothing and changes no record.

## Who starts the work, and when

The matter lead, the firm's operations lead or the billing coordinator runs it for one matter: before a partners' meeting, before a budget conversation with the client, at the end of a phase, or on a regular cycle the firm sets for its larger matters.

The responsible partner reads it, settles the questions and decides what happens next. The billing coordinator answers the checks on the time records.

## What they supply

- **The as-of date.** Schedule notes, past-due actions and the age of unbilled time are all measured from it.
- **The matter plan:** client, responsible partner, fee arrangement, the matter budget and when it was last agreed, and what is in and out of scope.
- **The phase table:** each phase with its planned dates, its budget, its status and the matter lead's estimate of the fees still to come.
- **The time and billing export** for the matter, with the column headers the template names. If a header does not match, the work stops and asks rather than guessing.
- **The matter lead's latest notes** (optional): developments, risks, actions, decisions the client owes.
- **The firm's settings,** once: when a matter turns amber or red, how late a phase may run, and how old unbilled time may get.

It works from exported files and needs no connection to the billing system and no sign-in details.

## What comes out

One summary in a fixed order. The status comes first, with each rule that set it. Then the scope, every phase with its schedule note, the budget line for each phase and for the matter (fees to date, share of budget, estimate to complete, projected total and the amount over or under), billed and unbilled time, and a tie-out line that proves the figures.

After the numbers: hours and fees by timekeeper, the risks and next actions in the matter lead's own words with their owners, what the firm is waiting on the client for, the questions for the responsible partner, the checks for the billing coordinator, and a line counting anything left out because it spoke to the merits.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Law firms](https://fullypowered.ai/industries/law-firms/), where each matter has a responsible partner and a budget agreed with the client, and an overrun found late is the hardest conversation to have.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where the same summary works for one engagement with phases, a budget and a responsible partner or lead.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), which runs the firm's reporting rhythm and the rules behind the ratings.
- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), which owns phases, dates and the estimate to complete.
- [Finance and accounting](https://fullypowered.ai/functions/finance-and-accounting/), which keeps the time and billing records the figures come from.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where matter budgets are watched by one experienced partner's instinct and deserve a written page.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when there are more matters than any partner can keep the numbers of in their head.

## What has to change for your company

Set your own thresholds for amber and red, the grace a late phase gets, and the age at which unbilled time becomes a risk. The template states the column headers it expects; replace them with the headers your billing and practice management systems really export, and your phase status words, so the summary does not stop to ask. Decide how fixed-fee and capped matters are read, and whether expenses count against the budget. Agree the headings your matter leads use in their notes and who receives the summary. Keep client updates separate: this page is internal to the firm.

## What has been checked

Fully Powered AI wrote this capability template in its own words, drawing on two openly licensed matter-reporting methods credited with it. It was editorially reviewed on 10 November 2026. It was tried on its invented example on 10 November 2026 in one run; the record is published with it. That run did not reach the stop conditions, a late phase or a phase with no estimate to complete. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past matters whose budgets your partners remember well, plus hard cases written in advance: phase budgets that do not add up, a phase with no estimate to complete, time on another matter or after the as-of date, an export with a renamed column, a note that comments on the merits. The billing coordinator checks every figure against the billing system before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) sets those cases up, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Weekly open-matter check](../weekly-open-matter-check/)
- [Client-status update preparation](https://fullypowered.ai/capabilities/client-status-update-preparation/)
- [Budget-versus-actual variance commentary](https://fullypowered.ai/capabilities/budget-versus-actual-variance-commentary/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
