# Inquiry handoff

Capability template 0.1.0. Written by Fully Powered AI.

## Purpose

Turn a new inquiry, exactly as it arrived, into one inquiry packet the firm's conflict review and acceptance processes can act on the same day: every party the conflict review needs, every missing item with the person who must supply it, anything the responsible attorney must see, where the packet went and one next action with an owner.

The packet prepares decisions and makes none. The conflicts clerk runs the firm's conflict search. The responsible attorney resolves any potential conflict under the firm's procedure, decides acceptance and assesses every date. The intake coordinator sends every message. Nothing in the packet clears a conflict, accepts a client, advises the prospective client or calculates a deadline.

## When to use it and when not to

Use it when a prospective client contacts the firm by form, phone, email or referral, and again each time a missing item arrives.

Do not use it:

- to answer the prospective client's questions or assess their position;
- to decide whether a conflict exists, or to accept or decline a client;
- for an existing client's new matter, if the firm has a separate procedure ([set locally]);
- when the caller describes a court date or deadline as close. Tell the responsible attorney first, then run it.

## Roles

- **Runs it:** intake coordinator.
- **Reviews before routing:** intake coordinator; the firm administrator spot-checks [one in N] packets.
- **Runs the conflict search and records the result:** conflicts clerk.
- **Decides:** responsible attorney (any potential conflict, under the firm's procedure; acceptance; anything about timing or advice); firm administrator (matter type when unclear).
- **Sends every message to the prospective client:** intake coordinator.
- **Supplies missing items:** the prospective client's contact, asked by the intake coordinator.
- **Owns the checklist, party rule and routing list:** firm administrator.

## Inputs

1. **Inquiry form entry.** From the website or intake inbox. If none, note "No form".
2. **Call notes.** From whoever took the call. If a call happened without notes, list them as missing, owned by that person.
3. **Emails and attachments.** From the intake inbox. If part of an attachment is unreadable, say which part.
4. **Intake checklist.** Required facts per matter type. If missing, stop.
5. **Party rule.** Which related parties go on the conflict list (parents, subsidiaries, signatories, insurers, opposing counsel). If missing, stop.
6. **Routing list.** Who reviews conflicts and who decides acceptance, by practice area, with cover. If missing, route to the firm administrator.
7. **Earlier contact (optional).** Prior inquiries or matters for the same names. If not searched, write "Earlier contact: not checked".

## The procedure

1. **List the sources** with channel, date and supplier.
2. **Identify the matter type.** If no checklist type fits, or two do, write "Matter type: unclear" and route to the firm administrator.
3. **Record each required fact** with its source. Mark caller-only statements "as stated". If sources disagree, record both values with sources and mark "conflicting sources". Never choose.
4. **Build the party list** under the party rule: name as given, role, source. A party referred to but not named (for example "belongs to a larger group") is a missing item.
5. **List missing items**: what is needed, who supplies it, why. Group items by supplier so each supplier gets one request.
6. **Copy dates exactly.** Never calculate a deadline, limitation period or reply date. Any date linked to a court, demand, notice or reply goes under "For the responsible attorney". If the caller's own words place it within [N] days, or the caller does not know when it falls, mark the packet "Urgent". Urgent means the intake coordinator tells the responsible attorney the same day; it says nothing about what is due.
7. **List documents** with date received and any readability problem.
8. **Set the status**: "Complete", "Incomplete: N items missing" or "Stopped: [reason]".
9. **Route** under the routing list. The conflicts clerk receives the party list [only when complete / now, marked incomplete], as the firm decides. Acceptance goes to the responsible attorney only after a conflict review result is recorded.
10. **Name one next action**, with one owner and a date.
11. **Draft one request per supplier** for the missing items, marked for the intake coordinator to review and send.
12. **Rerun** when an item arrives: new version number, a "Changes since last version" line, and any new party names sent to the conflicts clerk.

## Exceptions and stop conditions

- **Advice requested.** Record the question verbatim under "For the responsible attorney". Do not answer.
- **Name match.** If a party matches a name in the earlier-contact records, write "Name match noted for conflicts clerk". Do not assess it.
- **Identity unclear**, such as two company names for the prospective client. Stop and ask the intake coordinator.
- **Sensitive personal details** (health, immigration, criminal history). Record only what the checklist requires; flag for the responsible attorney.
- **Checklist or party rule missing.** Stop and ask the firm administrator.

## Output format

```
INQUIRY PACKET: [Prospective client], [matter as described]
Version [N], prepared [date]
Status: [Complete | Incomplete: N items missing | Stopped: reason] [Urgent]

Prospective client: [name]. Contact: [role], [details as given].
Matter as described: [one or two sentences]. Type: [type | unclear].

Sources:
- [Channel], [date received], from [who supplied it].

Parties for conflict review:
- [Name | missing]: [role]. Source: [source].

Facts recorded:
- [Fact]: [value] ([source]; as stated | confirmed | conflicting sources).

Documents received:
- [Document], [date]. [Readability note.]

Missing, and who supplies it:
- [Item]: [supplier]. Why: [reason].

For the responsible attorney:
- [Date, question or sensitive detail, as stated, with source.]

Routed to: [role], for [conflict review | acceptance | matter type].
Next action: [owner]: [action] by [date].
Changes since last version: [none | list].

Prepared for the intake coordinator to review. Contains no conflict
search, acceptance decision, advice or deadline. Nothing has been sent.

---
DRAFT for the intake coordinator to review and send
To: [supplier]
[One request listing every item this supplier owes, in plain words,
with no comment on the matter.]
```

## Reviewer checklist

- Every party the party rule requires appears, named or marked missing.
- Caller-only statements are marked "as stated".
- Conflicting values sit side by side with sources.
- No date has become a deadline.
- Nothing answers the prospective client or comments on the merits.
- Each supplier gets one drafted request, and it says nothing about the merits or timing.
- Routing matches the routing list; the next action has one owner and a date.

## Acceptance tests

Proposed tests. None has been run.

1. **Complete inquiry.** All facts and parties present. Expected: "Complete"; routed to conflicts clerk; no missing items.
2. **Unnamed related party.** The other side "belongs to a larger group". Expected: parent company missing, supplier named, "Incomplete".
3. **Form and call disagree** on the company name. Expected: both values with sources; "Stopped: identity unclear".
4. **Date mentioned.** A letter dated 28 October, reply due "soon". Expected: date copied as stated for the attorney; no deadline calculated; "Urgent" only if the caller's words meet the [N]-day rule.
5. **Advice requested.** "Do we have a strong case?" Expected: question recorded verbatim; no answer or assessment.
6. **Matter type outside the checklist.** Expected: "Type: unclear"; routed to firm administrator.
7. **Name match.** Party B appears in earlier-contact records. Expected: "Name match noted for conflicts clerk"; no view on conflict.
8. **Rerun.** The parent company name arrives. Expected: version 2, change line, new name sent to the conflicts clerk.

## Instructions for the AI assistant

```
You prepare inquiry packets for a firm's intake coordinator. You prepare;
people decide. Never search for, assess or clear a conflict. Never accept
or decline a client. Never give legal advice or assess the merits. Never
calculate a deadline, limitation period or reply date. Never send a
message: the intake coordinator sends every one.

If the intake checklist or party rule is missing, reply only "Stopped:
[which] missing. Ask the firm administrator."

1. List each source with channel, date and supplier.
2. Match the matter to one checklist type. If none or several fit, write
   "Type: unclear" and route to the firm administrator.
3. Give each required fact with its source. Mark caller-only statements
   "as stated". If sources disagree, show both and mark "conflicting
   sources".
4. Apply the party rule. A party referred to but not named is missing.
5. For each missing item give what, who supplies it and why, grouped by
   supplier.
6. Copy dates exactly. Put any date linked to a court, demand, notice or
   reply under "For the responsible attorney". Mark "Urgent" only if the
   caller's words place it within [N] days or the caller does not know
   when it falls.
7. Record any request for advice verbatim for the attorney; do not answer.
8. If a party matches the earlier-contact records, write "Name match
   noted for conflicts clerk" and nothing more.
9. If the prospective client's identity differs across sources, set
   "Stopped: identity unclear".
10. Route by the routing list. Acceptance goes to the attorney only after
    a conflict review result is recorded.
11. Give one next action with one owner and a date.
12. Draft one request per supplier, headed "DRAFT for the intake
    coordinator to review and send". Say nothing in it about the merits
    or timing.
13. Record sensitive personal details only where the checklist requires
    them, and flag them for the responsible attorney.
14. When a missing item arrives, issue a new version with a "Changes
    since last version" line and list any new party names for the
    conflicts clerk.

Use exactly the output format below. Add no facts beyond the sources.
```

Paste the output format above beneath the instructions.

## What to customize

- Required facts per matter type, and the party rule.
- Whether the conflicts clerk receives an incomplete party list.
- The [N]-day urgency rule.
- Routing by practice area, with cover.
- Which sensitive details are recorded at intake, and the spot-check rate.
- Where the packet is stored, and the tone of the request.
- Outside law firms: rename "conflict review" to the check your firm runs before accepting work, and adjust the party rule.

## Version notes

- 0.1.0, 9 November 2026. Written by Fully Powered AI. Editorially reviewed. Not yet tested in a client environment. Not yet tested in ChatGPT, Claude, Copilot or Gemini as a packaged version.
