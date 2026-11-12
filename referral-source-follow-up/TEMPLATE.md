# Referral source follow-up

Workflow template, version 0.1.0.

## Purpose

After a partner's conversation with a referral source or a prospective client, prepare two things from the conversation notes: the list of every promise made in that conversation, by either side, and one follow-up message in the partner's voice that keeps or restates the firm's promises using only materials approved for that audience. Everything that could not safely go into the message, such as client and matter details, things said in confidence, unconfirmed introductions, figures the firm's advertising rules control and questions that would need advice, is held back and listed for the partner. The assistant prepares; the partner checks confidentiality and the advertising rules, chooses the next step and sends the message. The assistant never sends anything, never updates the relationship record and never answers a question on the law.

## When to use it and when not to

Use it within a day or two of a lunch, call, meeting or event conversation with someone who sends the firm work or may become a client: another lawyer, an accountant, a banker, a financial adviser, a former client, or a business owner who has met the partner.

Do not use it:

- for a new inquiry that describes a matter and asks the firm to act. That goes through the firm's intake first (Inquiry handoff prepares it); this workflow template then drafts only the courtesy follow-up;
- for a first approach to someone the partner has not spoken to. That is cold outreach, prepared by Cold outreach sequence drafting;
- to design how the firm asks for and rewards referrals. That is Referral programme design;
- to answer a question about the contact's or their client's legal position, to quote fees or to describe the terms of an engagement. Those are the partner's, and are recorded for them, never drafted;
- to send messages in bulk after an event. Each conversation gets its own run.

## Roles

- **Runs it:** the partner, or a business development or relationship coordinator working from the partner's notes.
- **Decides:** the partner. They confirm what was promised, check confidentiality and the firm's advertising rules, choose the next step, edit the draft and send it.
- **Approves materials:** whoever the firm names, usually a marketing partner or the marketing team. Only their approved list counts.
- **Keeps the relationship record:** the coordinator or the partner, who enters the proposed log line after the message is sent.
- **The AI assistant:** prepares the promise list, the draft and the checks. It contacts nobody.

## Inputs

Everything is pasted or attached by a person. No mailbox, calendar or relationship system is connected, and the assistant never asks for a password or a login code.

1. **The conversation notes.** The partner's own notes or a transcript, with the date, the channel (lunch, call, meeting, event) and who attended from each side. Any line the partner marks "confidential", "off the record", "not public" or "don't mention" keeps that mark. If there are no notes, stop: the promise list cannot be built from memory.
2. **The contact record,** one row from the firm's contact list, with these default column headers: `Name, Organisation, Role, Relationship, Preferred name, Preferred channel, Do not contact, Last contact`. `Relationship` is "Referral source" or "Prospective client". If a header does not match, stop and ask which column holds which field. If no row is supplied, write "contact record not supplied", use the name in the notes and default to email.
3. **The relationship history,** the earlier entries for this contact, with these default column headers: `Date, Type, Firm person, Summary, Open promise`. If a header does not match, stop and ask. If no history is supplied, write "history not supplied; earlier promises not checked".
4. **The approved materials list,** with these default column headers: `Title, Audience, Approved by, Approved until, Link or file`. `Audience` names the relationship types the item may go to, separated by semicolons. If a header does not match, stop and ask. If no list is supplied, the draft offers no material and every promised material is left out for the partner.
5. **The settings:**
   - the partner's name, role and sign-off;
   - today's date;
   - [your follow-up window] (default: 2 working days after the conversation; working days are Monday to Friday unless the firm says otherwise);
   - [your word limit] for the body of the message (default: 180 words);
   - [your advertising checklist] (default: the seven categories in step 7);
   - [your required label], any wording the firm's rules require on a message of this kind (default: none);
   - the partner's chosen next step, if they have chosen one.

## The procedure

1. **Check the inputs.** Confirm one conversation, one date and one contact. If the contact record says "Do not contact: yes", stop and write only "Stopped: the contact record says do not contact. The partner decides." If the notes name a different contact from the record, stop and ask which is right.
2. **Set the dates.** Follow-up due by = the conversation date plus the follow-up window, counted in working days. If today is later, write "OVERDUE by [n] working days" in the header. Where the notes give a loose day ("by end of next week", "Friday"), turn it into a date counted from the conversation date and keep the words in brackets. "End of next week" is the Friday of the week after the week of the conversation, "end of this week" is the Friday of the conversation's week, and a bare weekday is the next such day after the conversation. Where the notes give no date, write "no date stated". Never invent a date.
3. **Find the promises.** A promise is a line in the notes where a named person, on either side, says they will do something. Number the firm's F1, F2 and the contact's C1, C2, in the order of the notes, and quote the words from the notes. A line that holds two promises is split into two numbered promises, each quoting the same line. A line with "maybe", "might", "could", "perhaps" or a question mark is not a promise: list it as P1, P2 under "Possible, not promised" for the partner to confirm. Add no promise the notes do not record. If the partner adds one after the conversation, label it "added by the partner after the conversation".
4. **Check earlier promises.** For each row in the relationship history whose `Open promise` is filled and not marked done, list it as E1, E2 with its date. If the notes of this conversation show it was kept, say so and quote the line. Otherwise mark it "needs the partner: say whether it was kept". Never assume an earlier promise was kept, and never put one in the draft unless the partner says to. If a firm promise in these notes covers the same thing as an open earlier promise, keep both lines, end the F line with "Overlaps E[n]." and leave the earlier one for the partner; the new promise is handled under step 5 as usual. Whether the two cover the same thing is a judgement: when it is not clear, mark the overlap and leave the judgement to the partner.
5. **Decide what each firm promise becomes in the draft.** Exactly one of:
   - **kept:** the promise is to send a material, and a row on the approved list matches it, its `Audience` includes the contact's relationship type and its `Approved until` is today or later. Name the material by its exact title;
   - **restated:** the promise is something the firm will do later, such as sending a date or a document once it exists. The draft says who will do it and when, or that it will follow, if no date is stated;
   - **left out, needs the partner:** with the reason. Give the reason only, not advice on what to do next. Reasons: the material is not on the approved list, is for another audience or its approval has ended; the introduction has not been confirmed with the third person; keeping it needs a sentence on the advertising checklist; keeping it needs advice, a view on a legal or tax question, a fee or engagement terms; or it would reveal something held back in step 6.
   Contact-side promises never go into the draft as a request, except that the draft may mention one when the chosen next step depends on it, naming it only by the general name the notes give it and saying nothing about what it contains. Each gets a check-back date: one working day after its date, or "partner to set" when no date is stated.
6. **Hold back what the message must not carry.** The notes are internal; the message goes outside. Leave out of the draft, and list as H1, H2 with a short description and its category:
   1. **Client or matter:** anything about a client of the firm or of the contact, any matter, party, transaction, fee or outcome, named or recognisable. What the contact says about their own clients' plans or dealings (for example, that some of them are thinking of selling) counts, even when no client is named.
   2. **Told in confidence:** any line marked confidential, off the record, not public or don't mention, and anything the notes say has not been announced.
   3. **Personal:** health, family, money or other personal details about anyone, unless the notes mark the line "fine to mention".
   4. **Third person not yet asked:** the name of anyone the firm offered to introduce, until the notes record that the person agreed.
   5. **Firm internal:** the firm's pipeline, other referral sources, fee arrangements, staffing and anything about other contacts.
   If a line fits more than one category, use the first that fits. The held-back list is for the partner and may quote or name the held-back words; the draft and the log line never do.
7. **Keep the draft clear of the advertising checklist.** Default categories, replaced by the firm's own list when supplied:
   1. a result, outcome, success rate, deal count or other figure about the firm's work;
   2. "specialist", "expert", "leading", "best" or a certification;
   3. a comparison with another firm;
   4. a fee, price, discount or free offer;
   5. a testimonial, or a client's name or words;
   6. anything of value offered or given in return for a referral, such as a gift, a payment or a share of fees;
   7. a prediction of what the firm will achieve for anyone.
   Write no sentence in these categories. If a firm promise can only be kept with one, leave it out under step 5. After drafting, read every sentence of the draft, the subject and the titles of attached materials included, and list each that still touches a category as A1, A2 with the category. If none does, write "none". Add [your required label] where the firm's rules require it.
8. **Questions the partner must answer.** Any question the contact asked that would need advice, a view on a legal or tax position, a fee or engagement terms is recorded word for word from the notes as Q1, Q2. A question the partner declined to answer in the conversation (for example, "rather not answer off the cuff") is still recorded as a Q item and is not a promise. A factual question about the firm's work, such as a deal count, is not recorded as a Q item; it appears only as a promise under step 3 if the partner said they would answer it. The draft does not answer it, refer to it or promise an answer unless the notes record the partner promising one, in which case that promise is left out for the partner under step 5.
9. **Prospective client conversations.** When `Relationship` is "Prospective client", the draft refers to the conversation only by its general subject as the notes name it, never by facts about the person's situation. If the notes record other parties, a dispute, a deadline or a request for the firm to act, write "INTAKE FIRST: the notes describe a possible matter; the firm's intake and conflict review come before any follow-up about it", hold the matter details back under category 1, and set the status to NOT READY TO SEND until the partner confirms intake has started.
10. **Offer the next step.** List up to three options, each taken from something the notes record as discussed or suggested, with the words from the notes. Never invent an option. If the partner has chosen one, mark it "Chosen" and use it in the draft. If not, the draft carries "[NEXT STEP: partner to choose]" and the status is NOT READY TO SEND.
11. **Write the draft,** in the partner's voice, on the contact's preferred channel. Email gets a subject line; a letter gets none; for a phone preference, write the same content headed "Notes for the call". In this order and nothing else:
    1. a greeting by the preferred name;
    2. one line of thanks naming the occasion and its day, with at most one point from the notes that nothing in step 6 holds back;
    3. one line for each kept promise, naming each material by its exact approved title and saying it is attached or linked;
    4. one line for each restated promise, naming who will do it and when;
    5. the chosen next step, as a proposal;
    6. [your required label], if any, and the partner's sign-off, exactly as the settings give it (on one line if the settings give it on one line).
    No firm news, no description of the firm's services beyond the material titles, no figures, no legal content. Count the words of the body, from the line of thanks to the line before the sign-off. If the count is over [your word limit], shorten the thanks line first, then the next-step line; never drop a kept or restated promise to fit.
12. **Propose the log line,** in the relationship history's own column order, for the person who keeps the record: the conversation date, its type, the firm people who attended, a one-line summary with nothing held back under any of the five categories in step 6, and every promise still open after the draft is sent, with its owner.
13. **Set the status and return.** READY FOR THE PARTNER'S REVIEW, or NOT READY TO SEND with each reason. Then "For the partner:" with every item code that needs them (F and E items left out or unresolved, P, Q and A items), or "none". Return everything to the partner.

## Exceptions and stop conditions

- **No notes:** stop and ask for them.
- **Do not contact:** stop; no draft, no log line.
- **A column header does not match the defaults:** stop and ask which column holds which field. Do not guess.
- **The notes and the contact record name different people or organisations:** stop and ask.
- **Asked to answer the contact's question, give a view on their or their client's position, quote a fee or describe engagement terms:** decline; record the question for the partner.
- **Asked to add a promise, a result, a figure or a client name the notes and the approved list do not support:** decline and say which input would support it.
- **Asked to offer a gift, a payment or a share of fees for a referral:** decline; it is category 6 on the advertising checklist and the partner's decision under the firm's rules.
- **Asked to send the message, set up a meeting or update the relationship record:** decline; the partner sends and the record-keeper records.
- **The notes or materials contain bank details, a password or a login code:** do not repeat them anywhere in the output and tell the person to remove them from the source.

## Output format

```
REFERRAL SOURCE FOLLOW-UP: [contact name], [organisation]

Conversation: [weekday date], [channel], [who attended from each side]. Prepared [today's date] for [partner].
Contact: [Referral source | Prospective client]. Preferred name [name]. Preferred channel [channel]. [Contact record not supplied.]
Follow-up due by: [weekday date] ([n] working days after the conversation). [OVERDUE by [n] working days.]
Status: [READY FOR THE PARTNER'S REVIEW | NOT READY TO SEND: [reasons]]. [INTAKE FIRST: ...]
For the partner: [item codes | none]

PROMISES MADE

Firm side:
F[n]. [Who] to [what], [weekday date ("words") | no date stated]. Notes: "[words]". In the draft: [kept: "[material title]" attached | restated. [Overlaps E[n].] | left out, needs the partner: [reason]].
[None recorded.]

Contact side:
C[n]. [Who] to [what], [weekday date ("words") | no date stated]. Notes: "[words]". Check back: [weekday date | partner to set].
[None recorded.]

Possible, not promised:
P[n]. [What]. Notes: "[words]". Partner confirms whether it is a promise.
[None recorded.]

Earlier promises still open:
E[n]. [Date]: [promise], from the relationship history. [Kept: "[words from these notes]" | Needs the partner: say whether it was kept.]
[None open. | History not supplied; earlier promises not checked.]

NEXT STEP
1. [Option]. Notes: "[words]". [Chosen.]
[Up to three options.]
Chosen: [option number | not chosen yet]

FOR THE PARTNER BEFORE SENDING

Held back from the draft:
H[n]. [Short description]: [client or matter | told in confidence | personal | third person not yet asked | firm internal].
[Nothing held back.]

Advertising checklist, sentences in the draft that touch it:
A[n]. "[sentence]": [category].
[None.]

Questions recorded, not answered:
Q[n]. "[question as noted]".
[None.]

DRAFT for [partner] to review, edit and send
Channel: [email | letter | notes for the call]
To: [preferred name], [organisation]
Subject: [subject, email only]

[Greeting],

[Body]

[Required label, if any]
[Sign-off]

Body words: [n] of [word limit]

PROPOSED LOG LINE, for the person who keeps the relationship record
[Column headers of the relationship history, separated by " | " like the entry]
[Date] | [Type] | [Firm people] | [Summary] | [Open promises with owners | none]

Prepared for [partner]'s review. Nothing has been sent, recorded or promised on the firm's behalf.
```

## Reviewer checklist

1. Every promise in the notes is on the list, on the right side, with the words quoted; nothing on the list is missing from the notes. (Partner)
2. Every "maybe" line sits under Possible, not as a promise. (Partner)
3. Every kept material is on the approved list, for this audience, in date. (Coordinator)
4. Nothing in the draft or the log line comes from a held-back category. (Partner)
5. No sentence in the draft touches the advertising checklist, or each that does is listed and the partner has cleared it. (Partner)
6. No question is answered and no fee or engagement term appears. (Partner)
7. No third person is named in the draft unless the notes record that the person said yes. (Partner)
8. The due date, every converted date and the word count are right. (Coordinator)
9. Earlier open promises are listed and none is assumed kept. (Coordinator)

## Acceptance tests

Proposed tests. None has been run.

1. **Ordinary referral lunch.** Two firm promises to send approved materials, one contact promise with "by end of next week". Expected: both kept with exact titles; the contact's date converted with the words in brackets; check-back the next working day.
2. **Material out of date.** A promised one-pager whose approval ended last week. Expected: left out, needs the partner, reason "approval ended [date]"; not mentioned in the draft.
3. **Material for another audience.** A promised briefing approved for clients only, sent to a referral source. Expected: left out, reason "approved for another audience".
4. **Unconfirmed introduction.** "Could introduce him to a contact at a bank, check with her first." Expected: left out; the bank contact's name appears nowhere in the draft or the log line.
5. **A figure the rules control.** "Said I'd get him the number of deals we did this year." Expected: left out under the advertising checklist; no figure in the draft.
6. **Off the record.** A line marked "not public" about the contact's firm. Expected: held back as told in confidence; absent from the draft and the log line.
7. **A legal question.** The contact asks how a tax change affects a sale. Expected: recorded word for word as a question; the draft neither answers nor mentions it.
8. **Maybe.** "Maybe a joint session in the spring." Expected: listed as possible, offered as a next-step option, not drafted as a promise.
9. **No next step chosen.** Expected: the draft carries "[NEXT STEP: partner to choose]"; status NOT READY TO SEND.
10. **Prospective client describes a dispute with a named supplier.** Expected: INTAKE FIRST; matter details held back; status NOT READY TO SEND.
11. **Do not contact.** Expected: stops with the one line; no draft.
12. **Headers renamed.** The materials list has `Name` instead of `Title`. Expected: stops and asks which column holds which field.
13. **Earlier promise.** The history shows an open promise from June that the notes do not mention. Expected: listed as needing the partner; not in the draft.
14. **Asked to offer a thank-you gift for the referral.** Expected: declines and names advertising category 6.

## Instructions for the AI assistant

```
You prepare a follow-up after a partner's conversation with a referral
source or a prospective client. You prepare; the partner decides. Never
send a message, set up a meeting or update a record. Never answer a
question on the law, tax, fees or engagement terms. Never add a promise,
a figure, a result or a name that the notes and the approved materials
list do not support. Never offer anything of value for a referral.

Inputs: the conversation notes; one contact record row (Name,
Organisation, Role, Relationship, Preferred name, Preferred channel, Do
not contact, Last contact); the relationship history (Date, Type, Firm
person, Summary, Open promise); the approved materials list (Title,
Audience, Approved by, Approved until, Link or file); the settings. If
there are no notes, stop and ask for them. If a column header does not
match, stop and ask which column holds which field. If Do not contact is
yes, reply only "Stopped: the contact record says do not contact. The
partner decides." If the notes and the contact record name different
people or organisations, stop and ask which is right. If no contact
record is supplied, write "contact record not supplied", use the name
in the notes and default to email. If no history is supplied, write
"history not supplied; earlier promises not checked". If no approved
materials list is supplied, offer no material and leave out every
promised material for the partner. Never ask for a password or a login
code; if the notes or materials contain bank details, a password or a
login code, do not repeat them and tell the person to remove them from
the source.

1. Follow-up due by = conversation date + [your follow-up window]
   working days (default 2). If today is later, mark OVERDUE by n
   working days. Turn loose days in the notes into dates counted from
   the conversation date and keep the words in brackets ("end of next
   week" is the Friday of the week after the conversation's week; "end
   of this week" is the Friday of the conversation's week; a bare
   weekday is the next such day after the conversation). No date in the
   notes: write "no date stated".
2. Promises: lines where a named person says they will do something.
   Firm side F1.., contact side C1.., in note order, quoting the notes.
   A line holding two promises becomes two numbered promises. A promise
   the partner adds after the conversation is labelled "added by the
   partner after the conversation". "Maybe", "might", "could",
   "perhaps" or a question: list as P1.., not a promise.
3. Earlier promises: each open promise in the history is E1..; mark it
   kept only if these notes show it, otherwise "needs the partner". If
   a firm promise in these notes covers the same thing as an open
   earlier one, keep both and end the F line with "Overlaps E[n]."; if
   it is not clear, mark the overlap and leave the judgement to the
   partner.
4. Each firm promise is exactly one of: kept (an approved material, for
   this audience, approved until today or later, named by its exact
   title); restated (the firm will do it later; say who and when, or
   that it will follow); left out, needs the partner, with the reason
   only (no advice on what to do next).
   Contact promises get a check-back date one working day after their
   date, or "partner to set", and are not asked for in the draft unless
   the chosen next step depends on one; then name it only by the
   general name the notes give it, saying nothing about its contents.
5. Hold back from the draft and the log line, listed H1.. with the
   first category that fits: client or matter (named or recognisable,
   and what the contact says about their own clients' plans or
   dealings even when no client is named); told in confidence;
   personal (unless marked fine to mention); third person not yet
   asked; firm internal. The list for the partner may quote or name
   the held-back words; the draft and the log line never do.
6. Write no sentence that (1) states a result or figure about the
   firm's work, (2) uses specialist, expert, leading, best or a
   certification, (3) compares with another firm, (4) mentions a fee or
   free offer, (5) quotes a client, (6) offers value for a referral, or
   (7) predicts an outcome (or the firm's own checklist, if supplied).
   Then read every sentence of the draft and list any that touches one
   as A1..; otherwise "None."
7. Record questions needing advice, a view, a fee or terms word for
   word as Q1..; do not answer or mention them in the draft. A question
   the partner declined to answer in the conversation is still a Q
   item, not a promise. A factual question such as a deal count is not
   a Q item; it is a promise only if the partner said they would answer
   it.
8. Prospective client: refer only to the general subject. If the notes
   record other parties, a dispute, a deadline or a request to act,
   write INTAKE FIRST, hold the details back and set NOT READY TO SEND.
9. Next step: up to three options taken from the notes. Use the one the
   partner chose; if none, put "[NEXT STEP: partner to choose]" in the
   draft and set NOT READY TO SEND.
10. Draft on the preferred channel, in this order only: greeting by
    preferred name; one thanks line naming the occasion and day with at
    most one point not held back; one line per kept promise; one line
    per restated promise; the chosen next step; any required label;
    the sign-off exactly as the settings give it. Email gets a subject
    line, a letter none; for a phone preference write the same content
    headed "Notes for the call". Body within [your word limit]
    (default 180); shorten the thanks line, then the next-step line,
    never a promise.
11. Propose one log line in the history's column order, the header row
    and the entry both separated by " | ", with no held back detail and
    every promise still open with its owner.
12. Status: READY FOR THE PARTNER'S REVIEW or NOT READY TO SEND with
    reasons. "For the partner:" lists every F or E item left out or
    unresolved and every P, Q and A item, or "none".

Decline, and say which input would support it, if asked to answer a
question on the law or tax, give a view on anyone's position, quote a
fee or describe engagement terms (record the question instead), or to
add a promise, a result, a figure or a client name the notes and the
approved list do not support. Decline a gift, payment or share of fees
for a referral, naming category 6 of the advertising checklist. Decline
to send the message, set up a meeting or update the record.

Use the output format exactly. Print "None recorded.", "None.",
"Nothing held back." or "None open." in any empty section. End with:
"Prepared for [partner]'s review. Nothing has been sent, recorded or
promised on the firm's behalf."
```

## What to customize

- [your follow-up window], your working days and [your word limit].
- [your advertising checklist]: replace the seven default categories with the categories your firm's own rules and policies require, and set [your required label] if your rules require one.
- The confidentiality categories, if your firm holds back more, such as anything about a panel or a pitch.
- Your contact list, relationship history and approved materials columns, if they differ from the defaults.
- Who approves materials, and how often the approved list is refreshed.
- The partner's sign-off and tone: formal or first-name.
- Outside law firms: keep the same rules for any firm whose work arrives through introducers, such as accounting, wealth management or consulting, and replace the advertising checklist with your own profession's.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI from its own published map of law-firm work. Editorially reviewed. Tried on its invented example on 10 November 2026 in Claude; the record is published with it. After a pre-review the instructions, output format and example were revised in small ways, and the trial record was rewritten from a second run on the revised version. A later review's minor points (numbered advertising categories in the instruction block, two more date conversions, one sentence each on overlap, declined answers and naming a contact's promised list, and an aligned log-line rule) were applied as wording clarifications and not re-run; that run was made by the model that made the revisions, so it is not an independent check. Not yet tested in a client environment.
