# Filing package check

Before a filing goes to the attorney for signature, the paralegal gets every item on the firm’s own checklist for that court and judge marked pass or open: caption against the docket, length and format, certificates, exhibits, signature blocks and service. The attorney decides and signs.

*Workflow template · Law firms · Legal and contracts · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/filing-package-check/)*

## The outcome

The attorney picks up a filing package whose housekeeping has already been held up against the firm’s own checklist, item by item. The caption has been compared with the docket, party by party and digit by digit. The exhibits the brief refers to have been matched against the exhibits behind it, in both directions. The proof of service has been compared with the matter’s service list and with the counsel the docket shows. The defendant who dropped out of the caption, the exhibit referred to on page 2 that nobody attached, the bar number with two digits swapped, the co-defendant’s counsel left off the proof of service: each is found while there is still time to fix it, and each is a line for the attorney to confirm.

The check holds a firm line. It gives no legal advice and decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines. A pass means only that the files show what the checklist item asks; whether the filing is sufficient is the attorney’s call. It ships no formatting defaults and uses no court rule from memory: the firm’s checklist is the only measure. It counts no date, writes nothing for the package, edits no file, and sends, files, serves, signs and calendars nothing. Everything it produces is a draft for the named attorney, with a line for each point the attorney must confirm.

## Who starts the work, and when

The paralegal or legal assistant preparing the filing starts it once the package is assembled and before it goes to the responsible attorney for signature, and runs it again after each round of corrections. The responsible attorney decides and signs. In a company’s own legal team, that is the in-house lawyer who signs; where a company has no lawyer of its own, the check is addressed to outside counsel, never to the business as an answer.

It is not for deciding whether a filing is ready, working out when it is due, writing a missing certificate or proof of service, or filing and serving.

## What they supply

- **The filing package**: every file, with readable text, in filing order: the main document, the exhibits, the certificates and the proof of service.
- **The firm’s filing checklist** for that court and judge, approved and dated by an attorney, with an ID, an area and the requirement written out for each item.
- **The docket record** as the court shows it, printed or saved that day: the court, the case number, the judge, every party, the counsel for each party and the hearings set.
- **The matter’s service list**, exported from the matter file as a spreadsheet.
- **The signing attorney’s record** from the firm’s attorney roster.
- The matter, the firm’s client in it, the case number, the document’s title, the attorney who signs, today’s date, which hearing on the docket the document is for when the docket sets more than one, and the word processor’s word count where the checklist sets a word limit.

The workflow template ships no court rules and no formatting defaults. Every requirement comes from the firm’s checklist, used exactly as written. If a column heading in the checklist or the service list does not match the one the template names, it stops and asks which column holds what. It never counts words itself, and what the text cannot show, such as type size, margins or where something sits on the page, is left open for a person to check by eye.

## What comes out

One draft check, headed as a draft for the attorney:

- **Package read:** each file, what it holds and how many pages, counted by its own page numbers.
- **Checklist items:** every item in the checklist’s order, marked pass or open, with the requirement quoted and what the files show located by file, page and line. Each open item says why: a gap, something the text cannot show, an item that is unclear, an input not supplied, or a date that would have to be counted.
- **Exhibits:** each exhibit label, where it is referred to and where it is attached, so one referred to but missing and one attached but referred to nowhere both stand out.
- **Service:** each person on the service list against the proof of service, then anyone in the proof who is not on the list, then any counsel the docket shows who is not on the list.
- **Attorney to confirm:** a line for each open item, then lines for the attorney to confirm the passes, decide sufficiency and authorise filing and service.
- **Check:** the counts, the areas the checklist has no item for, and how pages and words were counted.

The paralegal corrects the files, checks by eye what the text cannot show, and runs it again. Then the package and the check go to the attorney, who answers every line, decides, signs and authorises filing and service. Only then do people file and serve.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Legal and contracts](https://fullypowered.ai/functions/legal-and-contracts/): a filing is something an attorney signs, and this check holds its housekeeping against the firm’s own checklist before the attorney sees it.
- [Law firms](https://fullypowered.ai/industries/law-firms/), in litigation groups where filings go out every week and each judge’s requirements live on a checklist the paralegals keep.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where one senior paralegal’s knowledge of each judge is turned into a written checklist first.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when filings multiply faster than the people who check them.

It sits beside [outgoing work sign-off log](https://fullypowered.ai/workflows/outgoing-work-sign-off-log/), which tracks the attorney’s sign-off on everything leaving the firm without opening the drafts, and [court-order deadline notice preparation](https://fullypowered.ai/workflows/court-order-deadline-notice-preparation/), which turns an entered order into a draft notice for the attorney. [Citation and quotation check](https://fullypowered.ai/workflows/citation-and-quotation-check/) checks the citations inside the brief, which this check leaves alone.

## What has to change for your company

The checklist is yours, and it is the whole measure. An attorney decides what goes on it for each court and judge: the caption rules, the length and format limits, the certificates, how exhibits are labelled, what the signature block holds, how service is recorded. Write each requirement so a person could check it against a file, give it an ID, and give the checklist a date, a review date and an owner. Put the requirements the text can show apart from the ones only a person can see, such as type size, margins and where something sits on the page.

Decide where the docket copy comes from and how fresh it must be, who keeps the service list and the attorney roster, and whether the paralegal corrects the files before or after the attorney sees the check. We sit with the paralegals who assemble your filings and the attorney who owns the checklist, write down how a package is really checked, and set it up in the AI product the firm has approved: ChatGPT, Claude, Copilot or Gemini. Confirm with your own policies, and with counsel on any protective order, that the package may be used there.

## What has been checked

Fully Powered AI wrote this workflow template in its own words, drawing on one published method credited in its sources, and it was editorially reviewed on 11 November 2026. It has not been reviewed by a lawyer. It was tried on its invented example in Claude, in a clean chat given only the instructions and the example’s inputs, on 11 November 2026, and the record of that run, which replaced two earlier ones from the same day, is published with the template. It has not yet been tested in a client environment, and it has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing at your firm means running it on past packages your attorneys already signed, with problems planted in advance: a party dropped from the caption, a transposed case number, a missing exhibit, an exhibit nobody refers to, a wrong bar number, a person left off the proof of service, a checklist item on type size, a request that asks when the filing is due. The attorney checks every line before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Outgoing work sign-off log](../outgoing-work-sign-off-log/)
- [Court-order deadline notice preparation](../court-order-deadline-notice-preparation/)
- [Citation and quotation check](../citation-and-quotation-check/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
