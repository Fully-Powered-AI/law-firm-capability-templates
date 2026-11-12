# Weekly open-matter check

Every Monday the operations manager sees every open matter: which tasks are overdue, which have no owner, and which matters could not be checked at all. The managing partner gets one summary, and each responsible attorney gets a note that is drafted and ready for the manager to send.

*Workflow template · Law firms · Operations and process improvement · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/weekly-open-matter-check/)*

## The outcome

No matter goes quiet without someone noticing. The whole book is checked every week, the small matters as carefully as the large ones, in the time it takes to check a handful by hand. The operations manager starts Monday with the counts done, the matters that most need attention ranked by a rule the firm chose, and a draft note for each responsible attorney.

The check also says what it could not see. Its first line compares the matters it assessed with an independent list of what should be open, and names every matter it could not assess. A matter that has dropped out of the case system by mistake shows up by name, where a count taken from the case system alone would have missed it.

This is administrative work on the firm's own task list. It gives no legal advice, works out no court deadline and puts no date on any task. The operations manager sends every note, and the attorneys decide who does what and by when.

## Who starts the work, and when

The operations manager starts it, usually on Monday morning once the week's list of open matters has arrived from billing. It can run on any other day the manager wants a fresh look, with that day as the check date.

The responsible attorney on each matter confirms the counts in the note and decides who takes each task. The managing partner reads the summary and says which flags were wrong, so the check gets better each week.

## What they supply

- **The check date.** The Monday being checked. Overdue is measured from it.
- **The roster of open matters.** A dated list kept outside the case system, usually by billing: a matter is open while the firm bills it. This is the independent count.
- **The matters export** from the case system: matter, client, responsible attorney, status.
- **The tasks export** from the case system: task, matter, owner, due date, status.
- **The firm's settings,** once: how old the roster may be, the size of the list, the words the case system uses for open and finished tasks and for an open matter, and the column headers of the three files.

The workflow template works from these exported files. It needs no connection to the case system and no sign-in details.

## What comes out

- **A coverage line, first.** How many matters the roster expected, how many were assessed, and each matter that could not be assessed, by name and responsible attorney.
- **One row for every matter assessed.** Open tasks, overdue, unowned, tasks with no due date, and a plain note such as "no tasks recorded".
- **The attention list.** Up to ten matters, ranked by counts alone, with the rule printed beneath. It is never padded with clean matters.
- **A draft note to each responsible attorney** on the list, with every overdue task, who has it and how many days late, with the working shown, and every task with no owner or no due date.
- **A draft summary for the managing partner,** carrying the same coverage line and naming each matter with no tasks recorded or none left open.

The result ends by confirming that nothing was sent and nothing in the case system was changed.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Law firms](https://fullypowered.ai/industries/law-firms/), where each matter has a responsible attorney and a quiet matter is the one that causes trouble.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where the same check works on engagements or projects, each with a responsible partner or lead.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), which owns the weekly rhythm and the follow-up.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where the check depends on one person's Monday morning and does not happen when that person is away.

## What has to change for your company

Name who keeps the roster and how old it may be before the check waits for a new one. The template states the column headers it expects in each file; replace them with the headers your billing list and your case system's exports really use, and set your status words, so the check does not stop to ask. Confirm the ranking rule and the size of the list. Replace the note wording with your operations manager's own. Decide who receives the notes: the template writes to the responsible attorney, never straight to the person holding the task. Keep holidays and absences with the operations manager, who knows who is away.

## What has been checked

Fully Powered AI wrote this workflow template from its own built example of this check, which used invented records. It was editorially reviewed on 9 November 2026. It was tried on its invented example in two runs, one on a first draft and one on the revised instructions, and the record is published with it. The instructions had small edits after the second run, which the record lists. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on past weeks your operations manager already checked by hand, with cases written in advance: a matter missing from the export, a roster that is two weeks old, a done task with an old due date, a task due on the check date. The manager checks the coverage line against the roster and one matter's counts against the case system before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) sets those cases up, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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
- [Client-status update preparation](https://fullypowered.ai/workflows/client-status-update-preparation/)
- [Weekly receivables summary](https://fullypowered.ai/workflows/weekly-receivables-summary/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
