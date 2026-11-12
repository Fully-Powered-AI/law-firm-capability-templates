# Research plan for counsel

Before an associate or paralegal starts on a partner's research question, they hold a one-to-two-page plan: the question split into sub-questions, the stated facts against each, the firm's own notes to read first, where to search and with what terms, and the gaps. Leads, not authorities: nothing is named from memory.

*Workflow template · Law firms · Legal and contracts · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/research-plan-for-counsel/)*

## The outcome

The researcher starts from a map of the work instead of a blank page. The partner's question is broken into its parts, in the partner's own words, so the scope can be confirmed before hours go into it. Every fact supplied is quoted with where it came from, and every document mentioned but not yet in hand is listed. The firm's own notes and earlier memos come first, with the ones due for review marked. The kinds of source to search and a set of search terms follow, each term traced back to the inputs it came from. Anything from research already done is copied exactly, with what is missing from each reference shown.

The plan is headed "leads, not authorities", and it means it. It names no case, statute or rule from memory, ever. If someone asks it for "the leading case", it says no. An authority appears only when it is already in the inputs, copied exactly where it stands, listed with the research supplied and marked "to be verified by the lawyer". It gives no legal advice; decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines; and sends, files, signs and calendars nothing. Asked for a verdict, a deadline, an amount, a case or what to do, it says that is for the named lawyer and points to the part of the plan concerned, and nothing more. The researching lawyer chooses the searches, finds every authority and verifies each one.

## Who starts the work, and when

An associate starts it when a partner or the responsible attorney hands over a research question, before the research begins or just after a first look. A paralegal can start it too, for a named lawyer; the paralegal's own name is not enough. The plan is always prepared for that lawyer and headed as a draft for them to confirm. If the person asking is not a lawyer, the plan is addressed only to the outside counsel they name, opens by saying it is not an answer, and shows the question, jurisdiction and court as that person's words until outside counsel states them.

It is not for answering the question, writing the research memo or advising a client.

## What they supply

- The request: the partner's question in the partner's words, the matter, the practice area, the lawyer the plan is for, and when the research is wanted.
- The facts as they stand: the partner's message, the intake note or other matter notes.
- The jurisdiction and court level, as the partner stated them. The plan never infers them.
- An export of the firm's practice-notes index, with fixed column headers. If a header does not match, the plan stops and asks.
- Today's date, so a practice note due for review can be marked. If it is missing, the plan asks for it before it starts.
- Optionally, research already done (notes, authorities found, a search log) and the firm's list of approved research sources.

## What comes out

One plan, marked as a draft for the named lawyer:

- **The question and its sub-questions**, in counsel's words, with any point to settle with the partner first.
- **The facts**, each quoted and located, set against the sub-questions by shared words, and a list of what is not stated.
- **Read first:** the firm's own notes that share words with the question, those past the firm's review age marked for their owner.
- **Kinds of source and search terms** for each sub-question, every word traced to the inputs. Which courts bind and what weight a source carries are left to the lawyer.
- **From the research supplied:** each item copied exactly, marked "to be verified by the lawyer", with what its reference lacks. Any case, statute or rule named elsewhere in the inputs, or added later in the conversation, is listed the same way and marked as supplied outside the research notes, and what it says a case held stays the supplier's words.
- **Gaps**, a **lawyer-to-confirm list** and a **check** that no authority appears beyond the inputs.

The person who ran it reads the plan against the inputs and gives it to the researching lawyer, who confirms it with the partner and does the research.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Legal and contracts](https://fullypowered.ai/functions/legal-and-contracts/): the preparation before research, done the same careful way every time, with the lawyer doing the lawyering.
- [Law firms](https://fullypowered.ai/industries/law-firms/), where partners hand questions to associates daily and a confident wrong citation is the most expensive kind of mistake.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where the firm's notes and precedents are its best asset and too often sit unread.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when new associates arrive faster than partners can walk each one through where to start.

When the work is summarising documents already gathered for an executive, [research summary brief](https://fullypowered.ai/workflows/research-summary-brief/) is the right workflow template. Once the research turns into work that needs a partner's sign-off, [outgoing work sign-off log](https://fullypowered.ai/workflows/outgoing-work-sign-off-log/) tracks it. Dates in an order belong to [court-order deadline notice preparation](https://fullypowered.ai/workflows/court-order-deadline-notice-preparation/).

## What has to change for your company

Your practice-notes index is the heart of it: an export with the standard column headers, a knowledge owner for each note, and a review date the plan can read. Decide how old a note may be before it is marked for review, how many sub-questions a request may hold before it goes back to the partner, and which research sources a lawyer has approved for each kind of source. Decide who may run it, where confirmed plans are kept and who passes them on.

We sit with the associates who do the research and the partner who owns the practice notes, write down how your firm really starts a research question, and set it up in the AI product the firm has approved: ChatGPT, Claude, Copilot or Gemini, with web search switched off for this workflow. Your firm keeps control of how the work gets done.

## What has been checked

Fully Powered AI wrote this workflow template, drawing on a clinic research starter Anthropic publishes under the Apache 2.0 licence, and left out that method's list of likely statutes: this plan proposes none. It was editorially reviewed on 11 November 2026. It has not been reviewed by a lawyer. A separate review of the legal boundary then found that the earlier version let a few sentences through that read as the plan's own view, and that its replies to pressure questions said more than they should; the instructions were tightened the same day. It was tried on its invented example in Claude on 11 November 2026, with five pressure tests, on the tightened instructions, and the record of that run, which says what the earlier run got wrong, is published with it. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your firm means running it on past questions whose research is done and comparing: every fact located, every useful note listed, every search term traceable, every reference copied exactly, no authority beyond the inputs. Include a request for "the leading case", an incomplete citation and a question with no jurisdiction. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Research summary brief](https://fullypowered.ai/workflows/research-summary-brief/)
- [Outgoing work sign-off log](../outgoing-work-sign-off-log/)
- [Court-order deadline notice preparation](../court-order-deadline-notice-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
