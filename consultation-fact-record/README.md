# Consultation fact record

After a first consultation, the intake attorney gets a draft fact record: each statement marked by how the client knows it, each date by how exactly it was given, the outcome the client wants set apart, every document mentioned but not supplied, and questions to choose from. It names no legal issue.

*Workflow template · Law firms · Legal and contracts · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/consultation-fact-record/)*

## The outcome

The intake attorney opens one page after the consultation and sees the account sorted: what the client did or saw, what someone else told the client, what the client is assuming, and what the notes do not show either way. Every line points back to its paragraph or timestamp in the notes. Dates stay exactly as precise as the client made them. Where the account disagrees with itself, both versions sit side by side. The outcome the client wants has its own place, and so does every letter, message or photograph the client mentioned and has not yet sent. The attorney's next conversation starts from a ready list of factual questions, and the paralegal's write-up reads the same way after every consultation.

This is preparation, and it stays preparation. It gives no legal advice. It names no legal issue, reads no legal relationship into what the client said, and gives no view on the matter. It decides nothing about legal meaning, merit, validity, privilege, conflicts or deadlines: a time limit the client mentions is quoted and left uncounted, and a name that was not on the inquiry's party list is flagged, never cleared. It sends, files, signs and calendars nothing. The record is a draft for the intake attorney, headed as one, with a line for each point the attorney must confirm. It never goes to the client.

## Who starts the work, and when

The paralegal who sat in on the consultation, or who received the transcript, starts it once the notes are saved in the firm's intake location, usually the same day. The intake attorney who held the consultation verifies the record, decides what to ask next and decides whether any new name goes to the firm's conflict review.

It is not for the first inquiry, before anyone has spoken with the client: [inquiry handoff](https://fullypowered.ai/workflows/inquiry-handoff/) does that. It is not for building a timeline from a set of documents, for reading the documents the client supplied, or for anything written to the client.

## What they supply

- **The consultation notes or transcript**, every page, as typed notes or a transcript with each speaker named.
- **The consultation details:** the prospective client, the matter label, the date, how it was held, who was present, and the intake attorney who verifies.
- **The party list from the inquiry**, so new names can be flagged.
- **The list of documents the client has supplied**, by file name. The record lists them; it does not read them.
- **The firm's own format** for the record, if it has one. Otherwise the default order below is used.

The workflow template works only from these. It brings in no law, no outside facts and nothing remembered from another matter.

## What comes out

One draft record, marked as a draft for the intake attorney:

- **People and organisations named**, each only in the client's own description, with any name not on the inquiry's party list marked as new.
- **What the client said**, one statement per line, each marked first-hand, secondhand (and from whom), the client's assumption, or basis not stated, and each date marked confirmed, approximate or unknown, with approximate words copied as said.
- **Time limits the client mentioned**, quoted and not counted.
- **What the client wants**, in the client's words, apart from the facts, with any question the client asked kept for the attorney to answer.
- **Documents:** mentioned but not supplied, mentioned and supplied, and supplied but never mentioned.
- **Contradictions**, both versions, neither chosen.
- **Gaps in the notes**, and where the note-taker's own comments were left out.
- **Follow-up questions** for the attorney to choose from, each pointing to the lines it comes from.
- **Attorney to confirm**, and a **check** block with the counts.

The paralegal reads the draft against the notes and gives it to the intake attorney. The attorney checks it, signs the verification line and decides what happens next. Nothing goes to the client or into the matter file before that.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Legal and contracts](https://fullypowered.ai/functions/legal-and-contracts/): the record is the step between hearing a client's account and the attorney's own analysis of it, kept free of that analysis.
- [Law firms](https://fullypowered.ai/industries/law-firms/), where the intake attorney sees several prospective clients a week and each account arrives as a page of rushed notes.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when consultations outgrow the time the intake attorney has to write them up by hand.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where one experienced paralegal writes up consultations well and nobody else knows how.

It follows [inquiry handoff](https://fullypowered.ai/workflows/inquiry-handoff/), which brings the inquiry to the firm's conflict review before any consultation. When the firm takes the matter on, [matter-opening checklist preparation](https://fullypowered.ai/workflows/matter-opening-checklist-preparation/) uses the verified record.

## What has to change for your company

The intake attorney decides the shape. Set the order and headings of the record to match the firm's existing intake note, keeping the draft heading, the marks, the attorney-to-confirm lines and the check block. Decide where notes and transcripts are saved, whether consultations are recorded or typed up, and who sends new names to the conflict review once the attorney says so. Name who verifies when the intake attorney is away. Agree how the note-taker marks their own comments, so the record can leave them out.

We sit with the paralegal and the intake attorney, look at how consultations are written up today, and set this up in the AI product the firm has approved: ChatGPT, Claude, Copilot or Gemini. Confirm with your firm's own policy that client information may be used in it. Your firm keeps control of how the work gets done.

## What has been checked

Fully Powered AI wrote this workflow template, drawing on a published intake method credited with it. It was editorially reviewed on 11 November 2026. It has not been reviewed by a lawyer. It was tried on its invented example in Claude on 11 November 2026, and the record of that run, which replaced earlier ones from the same day after an independent review, is published with the template. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your firm means running it on past consultations whose write-ups an attorney already checked, and comparing: every statement present, every mark the same as the attorney's, every approximate date left as said, every mentioned document listed, and no legal issue named. Include notes where the client changes a figure halfway through, a transcript where someone else in the room speaks, a time limit read out from a letter, and a request to say whether the client has a case. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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
- [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
