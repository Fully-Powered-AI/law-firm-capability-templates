# Matter-opening checklist preparation

Workflow template 0.1.0. Written by Fully Powered AI.

## Purpose

Prepare one matter-opening checklist for an accepted client and agreed engagement, so a person can open the matter and set up billing correctly the first time: each system's fields, the billing terms with their source clause, the documents on file, and every open item with an owner and the step it blocks.

A person opens the matter and sets up billing. The checklist enters nothing into a system, changes no engagement term and takes no position on starting work with items open. It states no conflict review result, accepts no client, gives no advice, calculates no deadline and sends no message.

## When to use it and when not to

Use it once the responsible attorney has accepted the client through the firm's process and the engagement letter is agreed, and again each time an open item closes.

Do not use it:

- before acceptance is recorded or the terms are agreed;
- to interpret an engagement term. Quote it and send questions to the responsible attorney;
- to approve an exception to the firm's opening rules.

In professional services and engineering firms the same procedure covers project or account opening (see "What to customize").

## Roles

- **Runs it:** firm administrator, for the first version.
- **Reruns it as items close:** billing coordinator.
- **Reviews the checklist:** firm administrator, before anyone enters data.
- **Decides:** responsible attorney (anything about the engagement terms, and raising missing items with the client); firm administrator (whether work starts before billing setup is complete, under the firm's rule).
- **Opens the matter and sets up billing:** [the role the firm names, often the billing coordinator or a records clerk].

## Inputs

1. **Acceptance record.** From the firm's acceptance process: who accepted, which client and matter, when. If missing, stop.
2. **Engagement letter as agreed.** Countersigned, or confirmed final by the responsible attorney. If only a draft exists, stop.
3. **Intake packet.** Client name, contacts, parties, documents and items still missing at intake. If absent, list it as missing, owned by the intake coordinator, and continue.
4. **Conflict review record.** The checklist notes that the record exists and never restates the result. If none exists, stop.
5. **Matter-opening standard.** Systems, required fields, numbering and naming rules, required documents. Kept by the firm administrator. If absent, stop.
6. **Client billing requirements (if any).** Billing guidelines or e-billing instructions, usually attached to the engagement letter.

## The procedure

1. **Check the gate.** If the acceptance record, agreed engagement letter, conflict review record or matter-opening standard is missing, set "Stopped: [which] missing", name the owner and do nothing else.
2. **Confirm identity.** If the client name differs across sources beyond capitalization or punctuation, record each version with its source and stop for the firm administrator.
3. **Fill matter fields.** For each system, list each required field with value and source. If the matter number is not yet issued, write "Matter number: to be issued by [role]".
4. **Extract billing terms**: arrangement (hourly, fixed fee, contingency, blended), rate source, retainer, any budget or cap, invoice frequency and client billing guidelines, each with its clause. Copy amounts and dates exactly, and never work out a due date from a term. If two clauses disagree, record both and open an item for the responsible attorney.
5. **List documents** the standard requires: present or missing.
6. **Build the open list.** Each blank field, missing document or unclear term becomes an item with what is needed, owner, the step it blocks (matter opening, billing setup, first invoice) and the date it opened.
7. **Escalate.** An item missing since intake, or open more than [N] business days, goes to the responsible attorney to raise with the client.
8. **Note dependencies**, for example an e-billing preference that waits on the billing contact.
9. **Set two statuses**, matter fields and billing setup: "Ready to enter" or "Not ready: N open items".
10. **Name one next action**, with one owner and a date.
11. **Rerun** when an item closes: update it, add a "Changes since last version" line, reset the statuses.

## Exceptions and stop conditions

- Gate documents missing, or client name differs: stop (steps 1 and 2).
- An engagement term is ambiguous or contradicts another: record both, open an item for the responsible attorney, do not resolve it.
- A term the standard has no field for (for example, a success fee): list it under "Terms with no field" for the firm administrator.
- A request to start work before billing setup is complete: record it for the firm administrator and take no position.

## Output format

```
MATTER-OPENING CHECKLIST: [Matter number or "number to be issued"], [Client], [matter name]
Version: [N], prepared [date]

Sources read: [acceptance record], [engagement letter, version/date],
[intake packet, date], [conflict review record: present].

Matter fields:
- [System]: [field]: [value] ([source]).
Status: [Ready to enter | Not ready: N open items]

Billing terms:
- Arrangement: [value] ([clause]).
- Rates: [source] ([clause]).
- Retainer: [as stated] ([clause]).
- Budget, cap or estimate: [as stated | none stated].
- Client billing guidelines and e-billing: [as stated | not recorded].
Status: [Ready to enter | Not ready: N open items]

Documents on file:
- [Document]: [present | missing].

Open items:
- [N]. [Item]: [what is needed]. Owner: [role]. Blocks: [step].
  Open since: [date]. [Depends on item M.]

Terms with no field: [none | list].
Next action: [owner]: [action] by [date].
Changes since last version: [none | list].

Prepared for the firm administrator. A person opens the matter and sets
up billing. Whether work starts before open items close is decided under
the firm's own rule.
```

## Reviewer checklist

- Every gate document is named in "Sources read".
- The client name matches across sources, or the checklist stopped.
- Every billing term cites a clause; amounts are copied exactly.
- Each open item has one owner and names the step it blocks; items missing since intake sit with the responsible attorney.
- Nothing states a conflict review result, interprets a term or approves an exception.

## Acceptance tests

Proposed tests. None has been run.

1. **Clean hourly matter.** Expected: both statuses "Ready to enter"; no open items.
2. **Billing contact missing since intake.** Matter 26-0412: billing contact requested at intake and still missing, e-billing preference not recorded. Expected: billing contact owned by the responsible attorney; e-billing owned by the billing coordinator, depending on item 1; matter fields ready; billing "Not ready: 2 open items".
3. **No agreed engagement letter.** Only a draft exists. Expected: "Stopped: agreed engagement letter missing"; nothing filled.
4. **Client name differs.** "Client A Distribution" in the intake packet, "Client A Holdings" in the letter. Expected: both recorded with sources; stopped.
5. **Fixed fee plus a success fee.** Expected: arrangement with clause; success fee under "Terms with no field".
6. **Contradictory rates** between the letter's body and its schedule. Expected: both with clauses; item for the responsible attorney; billing "Not ready".
7. **Rerun.** The billing contact arrives. Expected: version 2, change line, item 1 closed, item 2 actionable.

## Instructions for the AI assistant

```
You prepare matter-opening checklists for a firm's administrator. You
prepare; people decide. You never enter data into any system, issue a
matter number, interpret an engagement term, state or assess a conflict
review result, accept a client, give legal advice, calculate a deadline,
approve an exception or send any message.

Inputs: the acceptance record, the agreed engagement letter, the intake
packet, the conflict review record, the firm's matter-opening standard,
and any client billing requirements.

1. If the acceptance record, agreed engagement letter, conflict review
   record or matter-opening standard is missing, reply only "Stopped:
   [which] missing. Owner: [role]."
2. If the client name differs across sources beyond capitalization or
   punctuation, list each version with its source and set "Stopped:
   client name differs".
3. List each system's required fields with value and source. Leave a
   field blank if no source states it. If no matter number has been
   issued, write "Matter number: to be issued by [role]".
4. Record the billing arrangement, rate source, retainer, budget or cap,
   invoice frequency and billing guidelines, each with its clause. Copy
   amounts and dates exactly. If clauses disagree, record both and open an item
   for the responsible attorney.
5. Mark each required document present or missing.
6. Turn every blank or unclear item into an open item with owner, the
   step it blocks and the date it opened. Items missing since intake or
   open more than [N] business days belong to the responsible attorney.
7. Note dependencies. Give separate statuses for matter fields and
   billing setup, and one next action with owner and date.
8. List terms with no matching field under "Terms with no field".
9. If asked whether work may start with items open, record the request
   for the firm administrator and take no position.
10. When an item closes, issue a new version with a "Changes since last
    version" line and reset both statuses.

Use exactly the output format provided. Do not add facts that are not in
the sources.
```

Paste the output format from this template below the instructions.

## What to customize

- The systems, their required fields, and the numbering and naming rules.
- Which billing terms must be captured before setup.
- The [N]-business-day escalation threshold.
- Who opens matters and who sets up billing.
- The firm's rule on starting work with billing items open, and who may grant an exception.
- For professional services and engineering firms: replace the gate with a signed statement of work or accepted proposal; replace matter fields with project fields (project code, phases, fee basis, purchase order number, invoicing portal); replace retainer terms with milestone or retention terms; name the project manager or finance lead as owner.

## Version notes

- 0.1.0, 9 November 2026. Written by Fully Powered AI. Editorially reviewed. Not yet tested in a client environment. Not yet tested in ChatGPT, Claude, Copilot or Gemini as a packaged version.
