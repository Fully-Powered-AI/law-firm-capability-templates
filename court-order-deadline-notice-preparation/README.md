# Court-order deadline notice preparation

When a court order arrives, the legal assistant has a draft notice ready for the attorney: every directive in the court’s own words, every date copied from the order or proposed under the firm’s own written rule file, and a list for the attorney to confirm. Nothing is calendared or sent until the attorney confirms.

*Workflow template · Law firms · Operations and process improvement · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/court-order-deadline-notice-preparation/)*

## The outcome

The attorney opens one page and sees everything the order asks of anyone: each directive quoted with its page, each date, each hearing set or vacated, each amount. The careful first reading arrives prepared, footnotes included, and the attorney’s time goes to the judgment only an attorney can make.

This is preparation, and it stays preparation. It does not give legal advice and it does not decide when anything is due. A date the order states is copied. A date that has to be counted is a proposed date, counted only by the firm’s own written rule file, with the working shown, on a list the attorney answers line by line. Where the rule file does not cover a count, the workflow template stops on that line and says so. No date is final until the attorney confirms it.

## Who starts the work, and when

A legal assistant or docketing clerk starts it when a signed, entered order arrives on a matter and has been saved to the matter file. The handling attorney confirms. It is not for a proposed order, a letter from the other side, a clerk’s notice with no order in it, or explaining an order to a client.

## What they supply

- The order, as text or a PDF with readable text, every page.
- The matter name and case number they expect, and the people on the matter: handling attorney, supervising attorney, paralegal, docketing.
- The firm’s own written deadline rule file, dated and approved by an attorney: which kinds of count the firm lets staff propose, and exactly how each is counted.
- The court-closure list the firm’s docketing keeps for that court, with the period it covers.

The workflow template ships no court rules and uses none from memory. A firm without a rule file still gets the directives, the copied dates, the hearings and the amounts; every counted date goes to the attorney.

## What comes out

One draft notice, marked as a draft, for the matter team:

- **What the court ordered:** each directive in the court’s sentence, with page and paragraph, from the discussion and footnotes as well as the numbered list.
- **Dates:** copied from the order, or proposed under a named rule with the count shown, or marked “Not computed” with the reason.
- **Hearings:** set, moved and vacated, so docketing can see what must come off the calendar.
- **Amounts:** the exact figure, who pays, who is paid.
- **Attorney to confirm:** a line to answer for every proposed date, every copied deadline and every date left for the attorney, then the hearings and whether every directive is listed.
- **Check:** pages read against the order’s own footer, the rule file and closure list used with their dates, and how the counting was done.

The legal assistant reads the draft against the order and gives it to the handling attorney. The attorney confirms each line or corrects it. Only then does the notice go to the matter team and docketing put dates on the calendar. The notice never goes to the client.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/): the notice is a procedure with an owner, a rule file and a confirmation step, run the same way on every order.
- [Law firms](https://fullypowered.ai/industries/law-firms/), in litigation groups where orders arrive daily and a missed line in a footnote is expensive.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where one long-serving assistant knows how the firm counts and nobody has written it down.

It follows [matter-opening checklist preparation](https://fullypowered.ai/workflows/matter-opening-checklist-preparation/), which records who is on the matter. If the firm’s way of counting lives in one person’s head, [SOP exception capture](https://fullypowered.ai/workflows/sop-exception-capture/) is how to get it written before this workflow template relies on it.

## What has to change for your company

The rule file is yours, and it is the heart of this. A supervising attorney decides which kinds of count staff may propose, which date the firm counts from, what happens when a last day falls on a day the court is closed, and when the file is reviewed. Everything the file leaves out goes to the attorney. Docketing supplies the closure list for each court. You name who confirms when the handling attorney is away, where the confirmation is recorded, and who may circulate the notice afterwards.

We sit with the assistant who writes the notices and the attorney who owns the procedure, write down what is really done, and set it up in the AI product the firm has approved: ChatGPT, Claude, Copilot or Gemini. Your firm keeps control of how the work gets done.

## What has been checked

Fully Powered AI wrote this workflow template from its own built example for an invented firm. It was editorially reviewed on 9 November 2026. It was tried on its invented example in Claude on 9 November 2026, and the record of that run, which replaced an earlier one from the same day, is published with the template. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your firm means running it on past orders whose dates your attorneys already settled, and comparing: every directive found, every proposed date equal to the attorney’s, every uncovered count left alone, nothing sent. Include an order with a directive in a footnote, one counted from service and one with a page missing. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 9 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 9 November 2026. The record is in [TRIAL.md](TRIAL.md).
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
- [SOP exception capture](https://fullypowered.ai/workflows/sop-exception-capture/)
- [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
