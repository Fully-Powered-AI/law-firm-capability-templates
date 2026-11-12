# Conflict search record

Before the responsible attorney decides on a new matter, the conflicts clerk has a draft search record: every name searched with its aliases and related entities, every possible match with its source matter and why it matched, the names still to search, and the limits of the search. It clears nothing.

*Workflow template · Law firms · Legal and contracts · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/conflict-search-record/)*

## The outcome

The responsible attorney opens one record and sees the whole search. Every party is there with each alias and related entity the firm supplied. Every record in the firm's conflicts export that came close is there too, with the matter it sits in, that matter's client and the plain reason it surfaced. Just as visible is everything the search could not reach: a parent company nobody has named yet, a field left blank in the export, a source the firm's own rule requires that was not attached. Each of those is a further search with the conflicts clerk against it, so the gaps are on the page instead of hidden behind a short list.

This is preparation for a lawyer, and it stays preparation. What it does not do: it gives no legal advice. It decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines. It never calls a matter clear, never sorts a match into a kind of conflict and never says whether one could be consented to. It sends, files, signs and calendars nothing, and it changes nothing in the conflicts system. Every record is headed as a draft for the responsible attorney, with a line for each match and each point the attorney confirms. Whether a match is a conflict, whether consent is needed and whether the firm takes the matter are the responsible attorney's decisions.

## Who starts the work, and when

The conflicts clerk starts it once a new inquiry's party list is ready and the conflicts export has been run, usually the same morning. It runs again each time a missing name arrives, and when a new party joins an open matter. The responsible attorney reviews it.

The party list normally comes from [inquiry handoff](https://fullypowered.ai/workflows/inquiry-handoff/). This workflow template picks up where that packet ends and does not rebuild it. It is not for a lateral hire's list of former matters, for telling the prospective client anything, or for writing a consent, a waiver request or a decline letter. Asked "are we clear?", "can we take this?" or what to do, it gives one fixed reply: that is for the responsible attorney, named, with a pointer to the line of the record the question is about. It restates, selects and suggests nothing.

## What they supply

- **The party list:** each party with its role, whether it is a person or an organisation, the aliases and related entities supplied, and where each came from. Default column headers are set out in the template; if yours differ, the workflow template asks which column is which instead of guessing.
- **The conflicts export** from the firm's own system: client, adverse and related records with their matters, status, dates, responsible attorney and notes. With it, the report's own details: when it was run, by whom, how many records and which matters it covers.
- **The firm's written conflict search rule,** dated, approved by the attorney who owns the conflicts procedure and not past its review date: which words to ignore, which common words never count alone, which kinds of match to list, how old the export may be, which other sources every search covers, where older records are kept, and which related entities each organisation needs. The workflow template ships no search rule of its own. Without the firm's approved rule, or with one out of date or silent on any of these, it compares nothing and asks for the approved rule.
- **The request:** the inquiry reference, the responsible attorney, and where that attorney records decisions.

Nothing is looked up on the internet and nothing comes from memory. A parent company the firm has not named becomes a further search, never a guess.

## What comes out

One draft record in six parts, headed for the responsible attorney by name, with a short note to the conflicts clerk below it:

- **Names searched:** every name, alias and related entity, with the exact form it was compared in.
- **Possible matches:** each export record that came close, with its role, its matter, that matter's client, the reason it matched under the firm's search rule, and any note from the export copied word for word and marked as not assessed.
- **Names that need a further search:** unnamed parties, missing parents and subsidiaries, matched records with blank fields, and every source or period the export does not cover.
- **Limits of this search:** the export's date and scope, rows read against rows stated, blank fields, sources not supplied, and the matching used.
- **Attorney to review:** a line for the party list, one for each match, one for the further searches and one for the limits.
- **Check:** the counts, and where any text in the inputs was copied rather than acted on.

The conflicts clerk opens each match in the conflicts system, runs the further searches and gives the record to the responsible attorney, who decides and records each decision in the firm's own system. The record never goes to the prospective client: it holds other clients' information.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Legal and contracts](https://fullypowered.ai/functions/legal-and-contracts/): the search every new matter waits on, prepared the same way each time.
- [Compliance, risk and privacy](https://fullypowered.ai/functions/compliance-risk-and-privacy/): a written record of what was searched and what was not, kept with the attorney's decision.
- [Law firms](https://fullypowered.ai/industries/law-firms/), where the conflicts desk searches every new inquiry before anyone agrees to act.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when inquiries arrive faster than one clerk can search and write up by hand.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where years of matters, renamed clients and older paper records make the limits of a search matter as much as its results.

It follows [inquiry handoff](https://fullypowered.ai/workflows/inquiry-handoff/) and comes before [matter-opening checklist preparation](https://fullypowered.ai/workflows/matter-opening-checklist-preparation/), once the attorney has accepted the matter.

## What has to change for your company

The search rule is yours, and it is the heart of this. The attorney who owns your conflicts procedure decides which words are ignored, which common words in your own client list never count on their own, how fresh the export must be, which other sources every search covers, such as declined inquiries or a register of lawyers' interests, where records older than the system are kept, and which related entities your intake must collect. You choose the report your conflicts clerk runs, map your column names if they differ, and name where the attorney records decisions and who reviews when the attorney is away.

We sit with your conflicts clerk and the attorney who owns the procedure, write down how searches are really run, and set it up in the AI product your firm has approved: ChatGPT, Claude, Copilot or Gemini. Your firm keeps control of how the work gets done.

## What has been checked

Fully Powered AI wrote this workflow template from its own published map of law-firm work. It was editorially reviewed on 11 November 2026. It has not been reviewed by a lawyer. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your firm means running it on past inquiries whose searches your conflicts team already completed, and comparing: every match the clerk found is listed, nothing outside the rule is listed, every gap the clerk knew about appears as a further search, and no line says anything about whether a match is a conflict. Include a renamed company, a hyphenated surname, an export note that says "cleared" and a request to mark the search clear. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Inquiry handoff](../inquiry-handoff/)
- [Matter-opening checklist preparation](../matter-opening-checklist-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
