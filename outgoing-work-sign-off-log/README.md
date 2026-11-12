# Outgoing work sign-off log

Every item that needs a responsible attorney's sign-off before it leaves the firm sits in one log, in the order it has to go out: waiting, approved or returned, with the attorney's own note. Anything close to its date with no decision is flagged first. The log tracks status and never touches the legal substance.

*Workflow template · Law firms · Operations and process improvement · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflow templates/outgoing-work-sign-off-log/)*

## The outcome

Nothing leaves the firm unsigned because someone lost track. The operations manager has one list of everything staff and junior lawyers have prepared for a client, a court or the other side, sorted by the day it has to go. Each line shows whether the responsible attorney has approved it, sent it back or not yet looked, and carries the attorney's note exactly as they wrote it. The items running out of time with no decision sit at the top, so the attorney hears about them while there is still a day to act.

The log doubles as the firm's own record of who signed off what, and when. Every change arrives as a history line naming the person it came from, and an item that went out with no approval on file is called out by name rather than quietly closed.

This is status work and nothing more. The workflow template never opens a draft, says nothing about what is in it and approves nothing. An item counts as approved when the responsible attorney says so in their own message, and not before.

## Who starts the work, and when

The operations manager, or the assistant who supports a practice group, runs it each working morning, and again later on a day when a lot is going out. They bring the log and the messages that came in since the last update: new items put up for sign-off, the attorneys' approvals and returns, and word of anything sent or withdrawn.

Each responsible attorney approves or returns their items in their own message. The operations manager checks the proposed update, saves the log and takes the flagged items to each attorney.

## What they supply

- **Today's date.** Every flag is measured from it.
- **The log as it stands,** exported as a spreadsheet file. The template names the column headers it expects; a firm whose log is headed differently lists its own headers once in the settings, and the update stops and asks when it meets one it was not told about.
- **The messages since the last update,** each with who sent it and when: new items with their matter, who they go to and the date they must go out, approvals and returns, resubmissions, and notes of items sent or withdrawn.
- **The firm's settings,** once: how many working days ahead counts as close, the days the office is closed, and which attorney may decide for which when someone is away.

It works from the file and the messages alone. It needs no connection to the firm's systems and never needs the drafts themselves.

## What comes out

- **The flagged items first,** each with its reason: sent with no approval on file, past its date, due soon with no decision, sent back close to its date, a decision passed on by someone other than the attorney, an item with no attorney or no date.
- **The open log in send-by order,** one heading per date, with the status and the attorney's note on every line.
- **What closed in this update,** and a short list per attorney of what to raise today.
- **The messages it did not record,** each with the reason, such as an approval for an item that is not in the log.
- **The history lines to add and the updated log file,** ready for the operations manager to check and save.

It ends by confirming that nothing was saved, sent or approved and that no draft was read.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Law firms](https://fullypowered.ai/industries/law-firms/), where work prepared by staff and junior lawyers goes out under a responsible attorney's name.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where a partner or responsible professional signs off what goes to a client.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), which keeps the daily rhythm and chases the open items.
- [Quality management](https://fullypowered.ai/functions/quality-management/), which wants a dependable record that every outgoing item passed its sign-off.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where the sign-off list lives in one assistant's inbox and stops when they are away.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when new hires produce more drafts than a partner can keep track of by memory.

## What has to change for your company

Replace the default column headers with the ones your firm's log really uses, so the update does not stop to ask. Set how many working days ahead counts as close and list the days your office is closed. Write down who may decide for whom when an attorney is away; as written, only the named attorney, or a covering attorney in the settings, can approve or return an item. Keep your policy on what needs sign-off in your own procedures; the log records what is put up for it. Decide where the history lines are kept and how long closed items stay in the file. Firms outside law change the word "attorney" to the role that signs off.

## What has been checked

Fully Powered AI wrote this workflow template, taking the idea of a law-school clinic's review queue from two published versions under the Apache-2.0 licence and turning it into a status log for a firm. It was editorially reviewed on 10 November 2026. The update shown in the example was worked through by hand from the template's rules. The template was then tried once on its invented example on 10 November 2026; the record is published with it, and lists the small edits made afterward that have not been run again. It has not been tested in a law firm, and it has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your firm means running it on a past week your operations manager remembers well, with cases written in advance: an approval passed on by a paralegal, an item sent before it was approved, a return two days before the date, an item due on a Monday checked on the Thursday before. The operations manager checks every status against the attorneys' own messages before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) sets those cases up, and the [Weekly open-matter check](https://fullypowered.ai/workflows/weekly-open-matter-check/) is the companion routine for the tasks on each matter.

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

- [Weekly open-matter check](../weekly-open-matter-check/)
- [Court-order deadline notice preparation](../court-order-deadline-notice-preparation/)
- [Client-status update preparation](https://fullypowered.ai/workflow templates/client-status-update-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
