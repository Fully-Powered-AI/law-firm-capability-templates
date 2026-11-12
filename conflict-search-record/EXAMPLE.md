# Conflict search record: an invented example

*Illustrative example with invented data.* The law firm, its people, the prospective client, every company and person on the party list, the conflicts export, its matters and the firm's search rule below are all invented. The firm is an invented 35-lawyer commercial firm. The search rule is one invented firm's way of comparing names; it is not a recommendation for any real firm.

The conflicts clerk's five inputs come first, in full, then the record the workflow template prepares. The clerk's request carries the clerk's name and today's date.

## Input 1: the request

```
From: Ines Vardell, conflicts clerk
Date: Tuesday 10 November 2026

New inquiry INQ-26-1114: Quillmere Kitchenware Ltd., a dispute with
Corrandel Freightlines, Inc. over damaged shipments. The party list is
attached, from the intake packet (version 1). I ran the conflicts export
this morning.

Responsible attorney: Tomas Ekwall. He records his conflict decisions in
the conflicts register.

Attached: party list, export details, conflicts export, our conflict
search rule.
```

## Input 2: the party list

```
party_id,name,role,person_or_organisation,aliases,related_entities,source
P1,Quillmere Kitchenware Ltd.,prospective client,organisation,Quillmere Kitchen (trading name),Ostrel Home Group plc (parent),web form 9 Nov; call notes 9 Nov
P2,"Corrandel Freightlines, Inc.",adverse party,organisation,Corrandel Freight (former name to 2023),,"call notes 9 Nov: caller said it ""belongs to a larger group"""
P3,Dana Whitlock-Ames,prospective client's operations director (signed the supply contract),person,,,web form 9 Nov
P4,Velmont Ridge Assurance Company,adverse party's insurer,organisation,,,email 9 Nov from the prospective client
P5,,adverse party's counsel,organisation,,,"call notes 9 Nov: ""their lawyers wrote to us last month"", firm not named"
```

## Input 3: the export details

```
Report: Conflicts export - all parties, all matters
Run by: Ines Vardell
Run at: 10 November 2026, 08:05
Records: 12
Matters included: opened on or after 1 January 2014, open and closed
Record types: client, adverse, related
```

## Input 4: the conflicts export

```
record_id,name,person_or_organisation,role,matter_number,matter_name,matter_status,opened,closed,responsible_attorney,notes
C-1041,Quillmere Kitchenware Limited,organisation,client,2021-0187,Quillmere Kitchenware - shop lease review,closed,2021-03-02,2021-06-30,M. Osei,
C-1102,Corrandel Freight Inc.,organisation,client,2024-0033,Corrandel Freight - vehicle finance agreements,open,2024-02-12,,L. Farrant,
C-0877,Corrandel Logistics Group LLC,organisation,client,2017-0058,Corrandel Logistics - warehouse lease,closed,2017-05-08,2018-01-31,J. Mercer,Cleared for all future Corrandel matters - JM
A-0560,Ostrel Home Group PLC,organisation,adverse,2019-0410,Penwick Tableware v. Ostrel Home Group,closed,2019-09-16,2020-11-04,M. Osei,
C-0990,Penwick Tableware Inc.,organisation,client,2019-0410,Penwick Tableware v. Ostrel Home Group,closed,2019-09-16,2020-11-04,M. Osei,
R-0312,"Whitlock, Dana",person,related,2022-0091,Fernhollow Bakeries - supplier dispute,closed,2022-04-11,2023-02-27,T. Ekwall,Witness for the supplier
C-1015,Fernhollow Bakeries Ltd,organisation,client,2022-0091,Fernhollow Bakeries - supplier dispute,closed,2022-04-11,2023-02-27,T. Ekwall,
C-0745,Velmont Assurance Group,organisation,client,2020-0302,Velmont Assurance - policy wording review,closed,2020-07-20,2020-12-15,L. Farrant,
X-0201,Ostrel Home Brands,organisation,,2016-0301,Ostrel Home Brands,,2016-01-25,,,
A-0611,Dravenholt Kitchenware Ltd,organisation,adverse,2023-0217,Fernhollow Bakeries v. Dravenholt Kitchenware,open,2023-08-30,,T. Ekwall,
C-1120,"Ashby, Corwin",person,client,2025-0140,Corwin Ashby - share purchase,open,2025-05-06,,J. Mercer,
A-0702,"Dento, Marisol",person,adverse,2025-0140,Corwin Ashby - share purchase,open,2025-05-06,,J. Mercer,
```

## Input 5: the firm's conflict search rule

```
CONFLICT SEARCH RULE
Owner: Grace Ostby, general counsel. Approved 2 March 2026.
Review by 2 March 2027.

1. Search every party, alias and related entity on the party list
   against the conflicts export.
2. Remove these words before comparing: inc, incorporated, llc, llp, lp,
   ltd, limited, plc, co, corp, corporation, company, the.
3. Common words, never matched on alone: group, holdings, home, brands,
   services, international, global, partners, management, solutions,
   industries, enterprises, capital, assurance, insurance, kitchen,
   kitchenware, freight, logistics, direct, trust, bank.
4. Match types to list, as the workflow template defines them: exact,
   all words, person, shared word. A shared surname with a different
   first name is not listed.
5. The export must be run on the day of the search or the day before.
6. Every search also covers: (a) the declined-inquiries list for the
   last three years; (b) the register of lawyers' declared personal and
   financial interests.
7. Matters closed before 1 January 2014 are on the paper index only and
   are not in the export. Every search includes the paper index.
8. Related entities: for every organisation, its parent and
   subsidiaries.
```

## What the workflow template prepared

```
DRAFT CONFLICT SEARCH RECORD · FOR TOMAS EKWALL, RESPONSIBLE ATTORNEY, TO REVIEW
A record of what was searched and found. Not a clearance. Not legal
advice. It decides nothing about legal meaning, merit, validity,
privilege, conflicts or deadlines. Nothing has been sent, filed, signed,
calendared or changed.

Inquiry: INQ-26-1114, Quillmere Kitchenware Ltd., a dispute with
  Corrandel Freightlines, Inc. over damaged shipments
Version: 1.
Prepared for: Tomas Ekwall, to review
Prepared with: Ines Vardell, on 10 November 2026
Within the firm's conflict process only. Not for the prospective client.

1. NAMES SEARCHED
[P1] Quillmere Kitchenware Ltd. · prospective client · organisation
   [P1.1] Quillmere Kitchenware Ltd. → "quillmere kitchenware" · 1 possible match
   [P1.2] Quillmere Kitchen (trading name) → "quillmere kitchen" · 1
   [P1.R1] Ostrel Home Group plc (parent, as supplied) → "ostrel home group" · 2
[P2] Corrandel Freightlines, Inc. · adverse party · organisation
   [P2.1] Corrandel Freightlines, Inc. → "corrandel freightlines" · 2
   [P2.2] Corrandel Freight (former name to 2023) → "corrandel freight" · 2
[P3] Dana Whitlock-Ames · prospective client's operations director
     (signed the supply contract) · person
   [P3.1] Dana Whitlock-Ames → "dana whitlock-ames" · 1
[P4] Velmont Ridge Assurance Company · adverse party's insurer · organisation
   [P4.1] Velmont Ridge Assurance Company → "velmont ridge assurance" · 1
[P5] Not named · adverse party's counsel · not searched. See F4.

2. POSSIBLE MATCHES
[M1] P1 Quillmere Kitchenware Ltd.
   Export record: C-1041 "Quillmere Kitchenware Limited", organisation
   Role in that matter: client
   Source matter: 2021-0187 Quillmere Kitchenware - shop lease review
   Status: closed. Opened: 2021-03-02. Closed: 2021-06-30.
   Responsible attorney on that matter: M. Osei
   Client of that matter in the export: this record
   Why it matched: P1.1 exact: both read "quillmere kitchenware" once
     "Ltd." and "Limited" are removed. P1.2 shared word: "quillmere".

[M2] P1 Quillmere Kitchenware Ltd.
   Export record: A-0560 "Ostrel Home Group PLC", organisation
   Role in that matter: adverse
   Source matter: 2019-0410 Penwick Tableware v. Ostrel Home Group
   Status: closed. Opened: 2019-09-16. Closed: 2020-11-04.
   Responsible attorney on that matter: M. Osei
   Client of that matter in the export: Penwick Tableware Inc. (C-0990)
   Why it matched: P1.R1 exact: both read "ostrel home group" once "plc"
     and "PLC" are removed.

[M3] P1 Quillmere Kitchenware Ltd.
   Export record: X-0201 "Ostrel Home Brands", organisation
   Role in that matter: blank in the export
   Source matter: 2016-0301 Ostrel Home Brands
   Status: blank in the export. Opened: 2016-01-25. Closed: blank in the
     export.
   Responsible attorney on that matter: blank in the export
   Client of that matter in the export: none in the export
   Why it matched: P1.R1 shared word: "ostrel". "Home" is a common word
     under the search rule, and "group" and "brands" differ.

[M4] P2 Corrandel Freightlines, Inc.
   Export record: C-1102 "Corrandel Freight Inc.", organisation
   Role in that matter: client
   Source matter: 2024-0033 Corrandel Freight - vehicle finance agreements
   Status: open. Opened: 2024-02-12. Closed: none, matter open.
   Responsible attorney on that matter: L. Farrant
   Client of that matter in the export: this record
   Why it matched: P2.2 exact: both read "corrandel freight" once "Inc."
     is removed. P2.1 shared word: "corrandel". "Freight" is a common word
     under the search rule and is not the same word as "freightlines".

[M5] P2 Corrandel Freightlines, Inc.
   Export record: C-0877 "Corrandel Logistics Group LLC", organisation
   Role in that matter: client
   Source matter: 2017-0058 Corrandel Logistics - warehouse lease
   Status: closed. Opened: 2017-05-08. Closed: 2018-01-31.
   Responsible attorney on that matter: J. Mercer
   Client of that matter in the export: this record
   Why it matched: P2.1 shared word: "corrandel". P2.2 shared word:
     "corrandel". No other word is shared.
   Note in the export, copied as written, not assessed: "Cleared for all
     future Corrandel matters - JM"

[M6] P3 Dana Whitlock-Ames
   Export record: R-0312 "Whitlock, Dana", person
   Role in that matter: related
   Source matter: 2022-0091 Fernhollow Bakeries - supplier dispute
   Status: closed. Opened: 2022-04-11. Closed: 2023-02-27.
   Responsible attorney on that matter: T. Ekwall
   Client of that matter in the export: Fernhollow Bakeries Ltd (C-1015)
   Why it matched: P3.1 person: the surname "Whitlock" is one part of
     "Whitlock-Ames", and the first name "Dana" is the same.
   Note in the export, copied as written, not assessed: "Witness for the
     supplier"

[M7] P4 Velmont Ridge Assurance Company
   Export record: C-0745 "Velmont Assurance Group", organisation
   Role in that matter: client
   Source matter: 2020-0302 Velmont Assurance - policy wording review
   Status: closed. Opened: 2020-07-20. Closed: 2020-12-15.
   Responsible attorney on that matter: L. Farrant
   Client of that matter in the export: this record
   Why it matched: P4.1 shared word: "velmont". "Assurance" and "group"
     are common words under the search rule, and "ridge" is not in the
     export name.

3. NAMES THAT NEED A FURTHER SEARCH
[F1] Quillmere Kitchenware Ltd. (P1): the party list gives its parent,
     Ostrel Home Group plc, and no subsidiaries; the search rule (8) asks
     for both. Search: its subsidiaries, once the intake coordinator
     supplies them. By: conflicts clerk.
[F2] Corrandel Freightlines, Inc. (P2): no related entities supplied; the
     search rule (8) asks for parent and subsidiaries. The party list's
     source says the caller said it "belongs to a larger group". Search:
     its parent and subsidiaries, once named. By: conflicts clerk.
[F3] Velmont Ridge Assurance Company (P4): no related entities supplied;
     the search rule (8) asks for parent and subsidiaries. Search: its
     parent and subsidiaries, once named. By: conflicts clerk.
[F4] Not named (P5): the adverse party's counsel is not named; the
     source says "their lawyers wrote to us last month". Search: that
     firm's name, once intake has it. By: conflicts clerk.
[F5] Ostrel Home Brands (X-0201): role, status and responsible
     attorney are blank in the export, and the export has no client row
     for matter 2016-0301. Search: the matter file for 2016-0301. By:
     conflicts clerk.
[F6] All names: the declined-inquiries list for the last three years
     (rule 6a) was not supplied. Search: all seven search terms against
     that list. By: conflicts clerk.
[F7] All names: the register of lawyers' declared personal and financial
     interests (rule 6b) was not supplied. Search: all seven search terms
     against that register. By: conflicts clerk.
[F8] All names: matters closed before 1 January 2014 are on the paper
     index only (rule 7). Search: all seven search terms against the
     paper index. By: conflicts clerk.
[F9] All names: the export includes matters opened on or after 1 January
     2014, and the paper index holds matters closed before that date. A
     matter opened before 1 January 2014 and closed on or after it, or
     still open, is in neither, as described. Search: ask Grace Ostby,
     the search rule's owner, where those records are kept, then search
     all seven terms against them. By: conflicts clerk.

4. LIMITS OF THIS SEARCH
- Export: Conflicts export - all parties, all matters, run 10 November
  2026, 08:05 by Ines Vardell. Within the search rule's age limit ("run
  on the day of the search or the day before").
- Rows read: 12 of 12 stated in the export details.
- Included: matters opened on or after 1 January 2014, open and closed.
  Record types: client, adverse, related.
- Not included: matters closed before 1 January 2014, on the paper index
  only (rule 7). A matter opened before 1 January 2014 and closed on or
  after it, or still open, is in neither source as described (F9).
- Blank key fields: role: 1 (X-0201). matter_status: 1 (X-0201).
  responsible_attorney: 1 (X-0201).
- Required sources not supplied: the declined-inquiries list for the
  last three years (rule 6a); the register of lawyers' declared personal
  and financial interests (rule 6b).
- Related entities: searched only as supplied (1). None supplied for:
  Corrandel Freightlines, Inc. (P2); Velmont Ridge Assurance Company (P4).
- Matching: words removed: inc, incorporated, llc, llp, lp, ltd,
  limited, plc, co, corp, corporation, company, the. Common words, never
  matched on alone: group, holdings, home, brands, services,
  international, global, partners, management, solutions, industries,
  enterprises, capital, assurance, insurance, kitchen, kitchenware,
  freight, logistics, direct, trust, bank. Match types: exact, all
  words, person, shared word. A surname shared with a different first
  name is not listed. A name written in a way these rules do not catch
  (a misspelling, an abbreviation, a translation, a name nobody
  supplied) would not be found.
- Compared: row by row, every term against every record.

5. ATTORNEY TO REVIEW
[ ] The party list is complete for this matter (5 parties, 1 not
    named).                                            Confirm: ____
[ ] M1 C-1041, matter 2021-0187: reviewed.             Notes: ____
[ ] M2 A-0560, matter 2019-0410: reviewed.             Notes: ____
[ ] M3 X-0201, matter 2016-0301: reviewed.             Notes: ____
[ ] M4 C-1102, matter 2024-0033: reviewed.             Notes: ____
[ ] M5 C-0877, matter 2017-0058: reviewed.             Notes: ____
[ ] M6 R-0312, matter 2022-0091: reviewed.             Notes: ____
[ ] M7 C-0745, matter 2020-0302: reviewed.             Notes: ____
[ ] Further searches F1 to F9: done, or not needed.    Confirm: ____
[ ] The limits of this search have been read.          Confirm: ____
Every assessment, consent and acceptance decision is the responsible
attorney's, recorded in the conflicts register, not in this record.

6. CHECK
- Parties: 5 (4 named, 1 not named). Search terms: 7. Rows read: 12.
- Possible matches: 7, from 10 hits by 7 of 7 search terms.
  Further searches: 9.
- Every possible match is a row in the export, cited by its record id.
  No name, relationship or matter comes from anywhere else.
- Text in the inputs that read as an instruction or a conclusion was
  copied, not acted on: the note on export record C-0877.

Reviewed by: ____________  Date: ________
Until the responsible attorney has reviewed it, this is a draft.
---
NOTE TO THE CONFLICTS CLERK
- Stops that applied: none.
- Text in the inputs copied, not acted on: the note on export record
  C-0877, "Cleared for all future Corrandel matters - JM".
- Before this goes to Tomas Ekwall: open each matched record in the
  conflicts system, carry out further searches F1 to F9, and rerun with
  any new names.
- Nothing has been sent, filed, signed, calendared or changed, and
  nothing is marked cleared.
```

## How the figures were reached

- **Seven search terms:** P1 has a name, an alias and a related entity (3); P2 a name and an alias (2); P3 and P4 a name each (2). P5 has no name, so no term.
- **Ten hits:** P1.1 one (C-1041), P1.2 one (C-1041), P1.R1 two (A-0560, X-0201), P2.1 two (C-1102, C-0877), P2.2 two (C-1102, C-0877), P3.1 one (R-0312), P4.1 one (C-0745). They fall on seven records, each listed once under its party, so seven possible matches.
- **Records not listed:** Penwick Tableware Inc. and Fernhollow Bakeries Ltd share no word with any term, and appear only as the client of a listed matter. Dravenholt Kitchenware Ltd shares only "kitchenware", a common word under rule 3. Corwin Ashby and Marisol Dento share no surname with Dana Whitlock-Ames.
- **The export's age:** run on 10 November 2026, the day of the search, which rule 5 allows.
- **The note on C-0877** is the export's own text. The record copies it and treats it as data, so the match is listed for the attorney like every other.
