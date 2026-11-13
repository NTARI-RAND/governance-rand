# Add every policy to the bylaws through one register, Schedule P; move P2-004 to DCO; AGPL-3.0 for documents and code

**Tier 1 research · Governance · Bylaws**
**Filed:** 2026-11-13 · **Author:** Jodson Graves
**Sources:** bylaws `main` at `3276781`, Janus `main` at `9aa2332`, P2-004 v1.0 (public copy on ntari.org), plus the documents linked below

## Summary

This note answers three questions. The first two answers are recommendations for the federation to test, and nothing in them is adopted. The third has been decided since the note was filed: governance registry Entry 9 records it.

1. **Where to place the policies.** Put every policy into the bylaws through one register, **Schedule P**. Each policy becomes an entry in Schedule P, which is part of the bylaws: a code of the bylaws under KRS 273.161(6). Only its full text sits in a pinned file, in [NTARI-RAND/Policies](https://github.com/NTARI-RAND/Policies) or beside the code it governs, so changing a policy does not need a member-only Article XV amendment. The Secretary keeps Schedule P as a separate file in [NTARI-RAND/bylaws](https://github.com/NTARI-RAND/bylaws), filed under the bylaws section each policy serves. The bylaws text itself keeps only four kinds of rule: what Kentucky law requires to be there, rules that bind members, checks on a power, and rules that protect the commons from NTARI itself. Eleven bylaws changes make this work; they pass the bylaws suite in scratch copies of v1.0 and v1.1.
2. **Correcting P2-004 §3.** Replace copyright assignment and the CLA with what NTARI already does: every commit carries a DCO sign-off by its author with no bypass, authors keep their copyright, and NTARI takes no assignment. Strike the governance seats earned by lines of code and the settlement option that sells "cooperative membership" with governance rights. Put the floor in bylaws §9.4 so that neither the Board nor an officer can bring a CLA back.
3. **What license for documents.** Decided: AGPL-3.0 for every work the Institute publishes, documents and code alike, until a stronger copyleft appears. The President decided this on 2026-11-13, after reading this note's first version, which recommended CC BY-SA 4.0 for documents. Governance registry Entry 9 records it and amends P2-004 Part 2. Under AGPL a Markdown file is the document's source, and every rendered or printed copy must come with that source and the full license. The JFA official document keeps its CC BY-SA 4.0 footer until an amendment under §9.2 changes it. The research behind the first recommendation stays in this note as the record of the costs the decision accepts.

**Asks of the federation:**

1. Agree that placement follows a policy's job and subject, never its P-number, and that Schedule P is the one place for every policy.
2. Test the bylaws text in [The new bylaws text](#the-new-bylaws-text) as the basis for a bootstrap act. The founder board would adopt it under §16.1, ideally as part of the pending v1.1 adoption.
3. Test the replacement P2-004 part 3 in [Replacement text for P2-004 part 3](#replacement-text-for-p2-004-part-3). The founder board, acting as the Board, would ratify P2-004 v2.0.
4. Choose between AGPL-3.0 "or any later version" and "only" with a proxy the membership names. Until then, notices written under Entry 9 name version 3 only.
5. Decide whether the JFA specification should follow Entry 9 to AGPL-3.0, which needs an amendment of the official document under §9.2.
6. Answer the [questions for #federation-governance](#questions-for-federation-governance) and the counsel questions under [Recommendation](#recommendation).

The President's stated direction of 2026-11-13 frames all three answers:

- "AGPL-3 across the board until a stronger version of copyleft appears."
- The Janus specification keeps its CC BY-SA 4.0 footer for now.
- DCO instead of a CLA is deliberate.
- Every policy goes into the bylaws, and where to place them matters most.
- After this note was filed: "AGPL-3 for all docs and code" (registry Entry 9).

## Terms used here

*Governance and law*

- **KRS.** Kentucky Revised Statutes. Chapter 273 governs nonprofit corporations such as NTARI.
- **Instrument.** A formal governing document: the articles of incorporation, the bylaws, the JFA official document.
- **Article XV.** The bylaws' amendment article. Only the membership amends the bylaws text, by a delegates' ballot (§15.1).
- **Federation.** The members of one JFA layer: Substrate, Record, Covenant, Governance, or Economy & Information (§5.3).
- **Delegate.** The director a federation elects. The delegate casts the federation's one vote as the federation decided it (§5.3, §5.7).
- **Seat.** An office together with the federation §7.2 binds it to. The Substrate seat is the Workspace Administrator and the Substrate federation.
- **Bootstrap; bootstrap act.** Until federations elect representatives, the founder board holds the membership's powers (§16.1, §16.2). An act it takes with those powers is a bootstrap act, recorded in the governance registry.
- **Governance registry.** The append-only public record the Secretary keeps under §9.5. Today it is a Markdown file, GOVERNANCE-REGISTRY.md. Code search on 2026-11-13 found it in no NTARI-RAND repository; whether it is published elsewhere is unverified.
- **Written consent.** A Board decision taken without a meeting. Kentucky's default is that every director signs (KRS 273.375).
- **Floor.** A minimum rule that no lower instrument may go below.
- **Incorporation by reference.** One document makes another part of itself by naming it. The reference must identify exactly which text is meant.
- **Code of the bylaws.** Kentucky treats any code of rules for a corporation's affairs as bylaws, whatever it is called (KRS 273.161(6)). Schedule P, a separate file listing every policy, is such a code, kept by a lighter path than the bylaws text.
- **Pinning.** Citing a document at a fixed commit, so its text cannot change under the citation.
- **Digest.** A short fingerprint computed from a text, such as a SHA-256 hash. Any change to the text changes it.
- **Ministerial.** Done because stated conditions are met, without discretion, as the Secretary recognizes members (§3.3).
- **Savings clause.** A transition rule saying which earlier acts and rules still stand when a new instrument takes effect.
- **Safe harbor.** A rule that protects a transaction from challenge when stated conditions are met (KRS 273.219).
- **Gen-1, gen-2, gen-3.** Three generations of policy numbers: the 2025 Confluence numbering, the 2025–26 Slack canvas and channel numbering, and the 2026 repository numbering. One number often names different documents in different generations.

*Licenses and copyright*

- **Copyleft.** A license condition: anyone may copy, change and share the work, but copies and changed versions must carry the same freedoms.
- **AGPL-3.0.** The GNU Affero General Public License, version 3. A copyleft license written for software, which covers any copyrightable work; NTARI uses it for documents too (Entry 9). A changed program that people use over a network must offer them its source.
- **GPL-3.0.** The GNU General Public License, version 3. AGPL-3.0 without the network duty.
- **CC BY-SA 4.0.** Creative Commons Attribution-ShareAlike 4.0. A copyleft license built for documents, images and data.
- **CC BY 4.0.** Creative Commons Attribution 4.0. A permissive license: it requires credit but lets anyone make closed versions.
- **GFDL.** The GNU Free Documentation License, a copyleft license the Free Software Foundation (FSF) wrote for manuals.
- **ODbL.** The Open Database License 1.0, a copyleft license for databases.
- **OSI.** The Open Source Initiative, which approves licenses as open source.
- **SPDX.** Standard short license names, such as `AGPL-3.0-or-later`, written into files.
- **"Or any later version".** A grant that lets anyone use later versions of the license the FSF publishes (AGPL §14).
- **Proxy (AGPL §14).** A person or body the licensor names to decide whether later license versions may be used.
- **Source, preferred form.** The form people edit. For a document that is the Markdown or LaTeX file, not the PDF. AGPL calls this the source code and any other form, such as a rendered page or a print, object code (AGPL §1).
- **DRM.** Digital rights management: technical locks that stop people copying or changing a copy they hold.
- **One-way compatibility.** One license's material may go into works under a second license, but not back.
- **Dual-license.** Offering one work under two licenses, typically copyleft for free and closed terms for a fee.
- **CLA (contributor license agreement).** A contract a contributor signs before their work is accepted. P2-004's CLA transfers the copyright to NTARI.
- **DCO (Developer Certificate of Origin 1.1).** A statement a contributor certifies by adding a `Signed-off-by` line to each commit: they have the right to submit the work. It transfers no copyright.
- **Inbound = outbound.** A contribution comes in under the license the project goes out under, with no separate agreement.
- **Assignment.** A transfer of copyright ownership. It is valid only in a writing the owner signs ([17 U.S.C. §204(a)](https://www.law.cornell.edu/uscode/text/17/204)).
- **Work made for hire.** Work the hiring party owns from the start ([17 U.S.C. §101](https://www.law.cornell.edu/uscode/text/17/101)). Either an employee made it within the scope of the job, or it was specially commissioned in one of nine categories (among them a translation, an instructional text, a compilation and a contribution to a collective work) and both parties signed a writing calling it work made for hire. Software is not one of the nine.
- **Standing.** The right to bring a lawsuit. For copyright, only the legal or beneficial owner of an exclusive right has it ([17 U.S.C. §501(b)](https://www.law.cornell.edu/uscode/text/17/501)).
- **Statutory damages.** Damages a court picks from a range the law sets (17 U.S.C. §504(c)), instead of proven losses. They need timely registration (§412).
- **SFC.** Software Freedom Conservancy, a nonprofit that enforces copyleft licenses.

## Where to place the policies

**The answer.** This puts every policy into the bylaws. Each policy becomes one entry in Schedule P, which is part of the bylaws under KRS 273.161(6), filed under the bylaws section the policy serves. Only its full text sits in a pinned file, in NTARI-RAND/Policies or beside the code it governs, so changing a policy does not need a member-only Article XV amendment. How hard a rule is to change follows its job; where a reader finds it follows its subject. Floors and checks go into the bylaws text itself. A policy's P-number never decides where it goes or who may change it.

### The principle

**1. The bylaws text holds only four kinds of rule.** Everything else stays out of the text, as [§14.7][v10-14.7] already asks.

- What KRS 273 requires to be in the articles or bylaws. Examples: member classes and rights (KRS 273.187(1)), the number and election of directors (KRS 273.211), notice periods that differ from the statute (KRS 273.193, 273.197).
- Rules that bind members.
- Checks on a power, which [§2.2][v10-2.2] requires every power to name.
- Rules that protect the commons from the Institute itself. Examples: the licensing floor with DCO and no assignment, the bar on a single director approving a conflicted deal, and the order of instruments.

**2. Every other policy has one entry in Schedule P, which is part of the bylaws.** Schedule P is a code of the bylaws (KRS 273.161(6)). Kentucky lets the bylaws say who amends them (KRS 273.191), so the bylaws can give Schedule P a lighter path than the text. The Secretary keeps it in a separate file beside the bylaws. The adopted instrument, its seven translations and the suite stay untouched.

**3. Each entry has one of five named classes.** Only (b) and (c) can bind.

| Class | What it holds | Binds? |
|---|---|---|
| (a) cited instruments | The articles of incorporation, the JFA instruments §1.5 defines, the versions of the bylaws | They bind by their own force; the entry only cites them |
| (b) board policies | Policies the Board adopts within a named bylaws section, including the three slots the bylaws call for: venue (§5.6), deliberation (§6.9), conflicts of interest (§14.3) | Yes, once pinned and marked in force |
| (c) office and federation procedures | Procedures an office or federation issues within its own area | Yes, once pinned and marked in force |
| (d) informative documents | Research that analyzes and never governs | No |
| (e) documents not in force | Drafts, texts awaiting ratification, superseded or lost texts, retired numbers | No |

The classes are named with letters, not numbers, so they do not clash with the P1/P2/P3 series.

**4. Schedule P is arranged by subject.** A reader of [§9.4][v10-9.4] finds P2-004, the DCO mechanics, the AGPL research papers and the web Terms together. A document that serves several sections sits once, with pointer rows at the others.

**5. Each entry names its owner as a seat.** The owner is an office together with its bound federation under [§7.2][v10-7.2]. The design adds four rules about owners:

- An office may never write its own powers or duties.
- A procedure that commits funds or binds an outside party needs the Board.
- Protocol specifications are procedures of their layer's federation.
- Secretary entries are ministerial, and a refusal can be challenged, as with recognition under [§3.3][v10-3.3].

**6. Pre-v1.0 policies bind only once ratified and conformed.** A policy approved before v1.0 took effect on 2026-08-31, or claimed as adopted with no record, waits as "awaiting ratification". If it is still unratified when bootstrap ends, it is marked superseded.

**7. Nothing binds unless pinned.** A binding entry names a commit of a public repository. A registry entry carrying the text or its digest can serve too, but only once the registry itself is published ([Sequence](#sequence) step 4). A Slack canvas, a Confluence page, a Wix page or a local file is only a copy.

**Schedule P and the registry's "policy register".** The registry's line 9 names a "policy register" in the record machinery as the registry's own future, mechanical form. That component is unbuilt. Schedule P is not that machine: it is the document-form index of policies, kept by the same office. When the policy register ships, Schedule P's rows migrate into it with the registry's entries.

### Why this design

**The answer.** Of three independent designs scored by a judge, C is the backbone. From A it takes subject arrangement, the ratify-only-once-conformed rule and the all-director consent wording; from B, seat ownership and named checks.

| Design | Score | Strength | Why not alone |
|---|---|---|---|
| A. Each Article ends with a schedule of its own policies | 7/10 | Best findability | Every policy act would edit the adopted file, which is "never patched" ([README L53-58][readme-53]), and its seven translations |
| B. A schedule arranged by owner (seat) | 6/10 | Best fit with JFA ownership and checks | A reader must know the owner. Binding office and federation policy strains KRS 273.207 (the board manages) and 273.228 (the board sets officer duties) |
| C. Authority tiers: floors in the text, everything else in Schedule P | 8/10 | Cleanest authority model; meets KRS 273.161(6) head-on | Arranged by tier, not subject |

### What Kentucky law allows

**The answer.** Kentucky lets the bylaws give a separately kept code of rules a lighter amendment path, but member rights must stay in the articles or the bylaws text. Every statute below was read from the Kentucky Legislature's site.

| Statute | What it says | What it means for placement |
|---|---|---|
| [KRS 273.161(6)](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=49017) | "Bylaws" means the code or codes of rules for the corporation's affairs, "irrespective of the name or names by which such rules are designated" | A binding "policy" can be a bylaw in substance, so Schedule P calls itself a code of the bylaws |
| [KRS 273.191](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=13623) | The board amends the bylaws unless the articles or bylaws provide otherwise | The bylaws may reserve the text to members ([§15.1][v10-15.1]) and give Schedule P to the Board |
| [KRS 273.187(1)](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=13621) | Member classes, qualifications and rights must be in the articles or bylaws | No policy may create membership or governance rights |
| [KRS 273.247(4)](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=36676) | The articles control an inconsistent bylaw, except on the number of directors | The articles rank above the bylaws |
| [KRS 273.228](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=13640) | Officer duties are those in the bylaws or, consistent with them, prescribed by the board | Officer-duty policies are Board policies |
| [KRS 273.195(2)](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44387) | Remote member meetings follow guidelines the board may adopt | The venue (§5.6) and deliberation procedure (§6.9) fit Board policy |
| [KRS 273.221](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=48302) | Committees may not adopt or amend bylaws or amend board resolutions (3)(e), (l). Advisory committees may not bind the corporation (4) | Committees cannot hold Schedule P powers. Advisory bodies are allowed if they do not bind |
| [KRS 273.375(1)](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44380) | Unless the articles or bylaws provide otherwise, board action without a meeting needs consent signed by every director | [§7.4][v10-7.4] invokes it and says nothing different, so unanimity applies today |
| [KRS 273.377](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44388) | Member action without a meeting needs consent signed by all members entitled to vote | This may be the test for bootstrap acts the founder board takes with the membership's powers (a counsel question) |
| [KRS 273.219](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=48304) | A safe harbor: a conflicted transaction is protected if disclosed and approved by disinterested directors, or if fair. A single director's approval does not count toward the safe harbor (3) | The proposed §14.3 bar on single-director approval goes beyond the statute, on purpose |
| [KRS 273.217](https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=48305) | Board quorum is a majority unless the articles or bylaws say otherwise. Remote participants must be able to communicate at the same time. No proxy votes | Quorum stays in the bylaws text |

No KRS 273 section expressly allows or forbids bylaws that bind separately kept policies. Kentucky case law on incorporation by reference was read only in secondary summaries. The practical reading: identify each bound text exactly (number, version, commit), and make sure members can read it.

### Where each policy goes

**The answer.** The table gives each of the 61 inventory entries (52 numbered, 9 unnumbered) one place. It also places three documents the verification found cited in the bylaws v3.1 draft, and three the review added, plus registry Entry 9, recorded after filing. Section numbers are bylaws v1.0 sections, the same in v1.1 for every section touched here. "Copy" means a text that is not canonical. The last column says how an entry changes after opening.

Seats: Covenant = President and Covenant federation. Governance = Vice President and Governance federation. Record = Secretary and Record federation. Economy & Information = Treasurer and its federation. Substrate = Workspace Administrator and Substrate federation.

Three kinds of fact below were reported by the inventory on 2026-11-13 and not re-checked: the 2026-03-18 renumbering proposal, the P2-003 canvas's "[Board resolution required]" line and its Gitee ban, and whether each gen-1 Confluence page is deleted or current.

**Instruments and registry entries**

| Document | Place | Class and status at opening | Owner, kept by | Changed afterwards by |
|---|---|---|---|---|
| P1-001 Bylaws | [§15.1][v10-15.1] | (a). v1.0 in force (registry Entry 1), pinned at `4246602`, the file's only commit, unchanged at `3276781`. v1.1 draft, not in force. v3.0–v8.0 superseded | The membership; the founder board during bootstrap ([§16.1][v10-16.1]). Kept by the Secretary | Text: Article XV, or a §16.1 act during bootstrap, always as a new version file. Schedule P: §14.10 |
| Articles of incorporation | [§1.2][v10-1.2] | (a) cited. Copy to be obtained. The [Kentucky record](https://sosbes.sos.ky.gov/BusSearchNProfile/Profile.aspx?ctr=1279987) shows organization 1268393, filed 2023-03-17, active and in good standing; the filing images were not retrieved | The members or directors under KRS 273.263 | KRS 273.263 |
| JFA instruments: official document, invariant registry, suite, dispute-mechanics design, OPEN-QUESTIONS | [§1.5][v10-1.5] | (a) cited, pinned at Janus `9aa2332` | The membership ([§7.5][v10-7.5], [§9.2][v10-9.2]) | Official document and invariant registry: §9.2 and [§9.16][v10-9.16]. Suite repairs: §9.17. Open questions: §9.3. Dispute design: no stated path (open question) |
| Registry Entry 2, residential substrate posture (2026-09-08) | §10.3 | Pointer row to the §1.5 entry. Entry 2 amended the official document and invariant registry | The membership through §9.2 and §9.16 | §9.2 and §9.16 |
| Registry Entries 3–4, Agrinet per-peer sync and its waiver | §9.1, under P3-012 | Pointer rows. Decisions of record, not policies. Entry 4's "no bypass" rule for DCO moves into §9.4 | Founder board; Entries 3 and 4 were "decided by the President, for the founder board" | Reopened under §2.3 and §6.7, or annotated by a later entry |
| Registry Entry 5, Audio Arts seed: §3.2(b) reading and §14.3 disclosure | §3.2(b), pointer at §14.3 | Pointer row. A reading of a membership condition must never become a Board policy (§7.6, §14.6, KRS 273.187(1)) | Founder board | A binding reading of §3.2(b) only by the membership or under Article XII |
| Registry Entries 6–7, secret scanning and push protection default for new repositories | [§13.1][v10-13.1], pointer at §8.6 | (b) "Repository security defaults", in force as a recorded bootstrap act, pending a confirming Board act under §7.4. Takes a fresh P2 number. Entry 6 was decided by the President for the founder board; Entry 7 is an annotation of it | Board; kept by the Substrate seat | Board act. The office may tighten by procedure; only the Board loosens |
| Registry Entry 8, LBTAS reading "page the volume, never the harm" | §9.12, beside P3-014 | (c) a procedure (reading) of the President's office under [§8.2][v10-8.2], pending a confirming Board act under §7.4: it reads how the LBTAS API the office oversees behaves, which comes close to the office's own duties (§14.10). Entry 8 itself says it is not an amendment | Covenant seat | The office reissues it with Board confirmation; the Board may revoke it; a version meant to bind the covenant goes through §9.2 |
| Registry Entry 9, AGPL-3.0 for all works, documents and code alike (2026-11-13) | §9.4, beside P2-004 | (b) in force as a recorded Board act amending P2-004 Part 2. Its rule moves into the §9.4 text with the bylaws act | Board, for P2-004; the membership, once §9.4 carries the floor | Board act until §9.4 carries it; then Article XV only |

**P1 series**

| Document | Place | Class and status at opening | Owner, kept by | Changed afterwards by |
|---|---|---|---|---|
| P1-002 Whitepaper: Addressing Democratic Information Velocity v3.0 | §1.4(c) | (d) informative. ntari.org post; Confluence 73334786 is a copy. Its first number (P1-005, shared 2025-10-02) is recorded as retired alias P1-005a | Institute as author; filed with the Governance seat | Secretary annotation. Its web footer's "AGPL v3" already matches Entry 9 |
| P1-003 Continuous Board Meeting Policy | [§7.4][v10-7.4] | (e) awaiting ratification. "Accepted April 21, 2026" in Slack, before v1.0; no registry entry. Its 5-of-8 quorum, 2-day notice and quarterly meetings conflict with v1.0 §7.2 and §7.4. The consent rule itself stays in the §7.4 text | Board; the Secretary records actions | Ratify as a conformed v2.0, or retire it as redundant to §7.4 |
| P1-003a Political Campaign and Lobbying Activities Policy (gen-1; also shared as P1-006, recorded as alias P1-006a) | §1.2 | (e) lost (Confluence 72548356 deleted) | Board if revived; Treasurer for compliance reporting | Revival is a new policy with a fresh number |
| P1-003b The Anthropology of Light v1.0 | §1.4(c) | (d) informative, draft research (Confluence 79298611) | Institute as author; Governance seat | Secretary annotation |
| P1-003c Conflict of Interest Policy, cited as "P1-003" in the bylaws v3.1 draft §8.1 (Slack file F0A3PM5NBUN) | §14.3 | (e) cited; text not found. It may be the same document as P2-002a (unverified) | Board | Replaced by the new §14.3 policy |
| P1-004 Routed, Not Negotiated v0.1 | §10.3 | (d) informative, pinned at Janus `9aa2332`. It says it analyzes and never governs ([L6][j-p1004]). Its rule is in Entry 2 | Institute as author; Substrate seat | Pull request to Janus; rules only through §9.2 or §9.16 |
| P1-004a Non-Discrimination Policy (gen-1) | [§14.6][v10-14.6] | (e) lost (Confluence 72613939, 404) | Board | If reissued: (b) for staff, volunteers and programs. Never a membership test |
| P1-005 Governance Venue Policy v1.0 | [§5.6][v10-5.6] | (b) required slot, **vacant**. The v1.0 draft is listed in (e) ([P1-005 L3][p1005]). On adoption the canonical file moves to NTARI-RAND/Policies | Board adopts; kept by the Substrate seat ([§8.6][v10-8.6]). Under v1.1 the Vice President and Workspace Administrator share the governance platform ([v1.1 §8.3][v11-8.3], [§8.6][v11-8.6]), so the keeping may become shared | Board act under §7.4. Its header L5 must change from "a bootstrap act under §16.1" to a Board act, so a later Board can revise it |
| P1-006 Officer Policy Framework – Office of the President | §8.2 | (e) draft (Confluence 77890155; cites the pre-v1.0 "Article IV") | Board adopts | Folded into one officer-duties Board policy with P2-005d and P2-007 (KRS 273.228). The office may not amend its own duties |

**P2 series**

| Document | Place | Class and status at opening | Owner, kept by | Changed afterwards by |
|---|---|---|---|---|
| P2-001 Document Priority Policy v1.2 | §14.9 | Split. The order of authority goes into new §14.8. Register, pinning and no-reuse rules go into §14.9–§14.10. The rest becomes P2-001 v2.0, class (b). v1.2 is (e), never adopted on record | Text parts: membership. v2.0: Board; kept by the Record seat | §14.8–§14.10: Article XV. v2.0: Board act |
| P2-002 Global Multilingual Broadcast Policy v2.0 | §1.4(d) | (e) awaiting ratification. "Adopted: October 2025" has no record. The ratifying act also decides the 2026-07-24 Presidential directive adding French and toki pona | Board; kept by the Record seat | Board act |
| P2-002a Conflict of Interest Policy (gen-1) | §14.3 | (e) lost (Confluence 61800475 and Jira NTAR-54 both 404) | Board | Replaced by the new §14.3 policy |
| P2-003 Open Source Software Broadcast and Preservation Policy v1.0 | §13.1, pointers at §13.2 and §1.4(b) | (e) draft in use; the canvas F09NFBPUWP5 reads "[Board resolution required]" | Board adopts; kept by the Substrate seat | Board act, after four fixes (below) |
| P2-003a Board Advisory Council Policy (gen-1) | §7.1 | (e) lost (Confluence 63668225) | Board | Revival as (b); advisory only (KRS 273.221(4)) |
| P2-003b Volunteer Time Module Policy | §14.2 | (e) status unknown (Confluence 84410370) | Record seat | If issued: (c) under the volunteer umbrella policy |
| P2-004 Licensing and Enforcement Strategy v1.0 | §9.4, pointer at §10.8 | Split and corrected. The floor goes into §9.4. The rest becomes P2-004 v2.0, class (b). v1.0 is (e) awaiting ratification. Parts 2.1–2.3, 3.1, 3.2, 3.4 and 7, the CLA items of part 10 and the part 4.2 "Option C" settlement cannot be ratified as written | Floor: membership. v2.0: Board; the Vice President administers member compliance (§10.8, Article XII). Action against outside infringers needs a Board act and the copyright holders | §9.4: Article XV only. v2.0: Board act |
| P2-004a CCC Program – Continuity Clarity Compliance Analysis (gen-1) | §14.9 (subject unknown) | (e) lost (Confluence 65273897); number retired | Secretary keeps the row | Annotation only |
| P2-004b Sociocracy 3.0 Slack Implementation Policy v1.0 | §6.9 | (e) draft never adopted (canvas F09PS6WRK52). Its circle-consent model replaces delegate voting, which no policy may do | Board | Ideas may feed the §6.9 procedure |
| P2-004c Virtual Software Development Studio Policy, cited in the bylaws v3.1 draft §2.3 | §1.4(c) | (e) cited; text not found | Secretary keeps the row | Annotation only |
| P2-005 Open Collective Financial Policies v0.1 | §14.2, pointers at §8.5 and §9.7 | (e) draft; number provisional. Its §9.4 citation for a documents license (L138, L251) matches neither bylaws version; it resolves once §9.4 names one | Board; kept by the Economy & Information seat | Board act; it commits funds |
| P2-005a Open-Source Distribution Policy (gen-1) | §13.1 | (e) superseded by P2-003 (Confluence 67371020) | None | Annotation only |
| P2-005b NTARi Corps Volunteer R&D Policy v1.0 | §14.4, pointer at §1.4(c)–(d) | (e) draft (canvas F09PPRKFCMV). Its "AGPL-3.0 or compatible" clause must be tightened to §9.4; its AGPL-for-data clause already matches Entry 9 | Board; the entering act names the keeping office | Board act. Becomes the volunteer umbrella policy |
| P2-005c Strategic Partnership Management Policy, cited in the bylaws v3.1 draft §7.3 | §14.2 | (e) cited; text not found | Secretary keeps the row | Annotation only |
| P2-005d NTARI Secretary Responsibilities | [§8.4][v10-8.4] | (e) unverified (a role description shared by direct message; not read) | Board | Folded into the officer-duties policy |
| P2-006 Fiscal Hosting Policy and Terms v0.1 | §14.2, pointers at §8.5 and §9.7 | (e) draft. Terms §8.2 already says NTARI "takes no assignment of copyright" | Board; kept by the Economy & Information seat; the Secretary keeps the register | Board act; it binds outside parties |
| P2-006a Working Group Leader Handbook (gen-1) | §5.3 | (e) lost (Confluence 70713348) | Unknown | If reissued: (c) of the federation it serves |
| P2-007 Officer Handbook (gen-1) | §8.1 | (e) lost (Confluence 70746114) | Board | Folded into the officer-duties policy |
| P2-008 Board Member Handbook (gen-1) | §7.1 | (e) lost (Confluence 70680641) | Board | If reissued: (b) for conduct rules, or (d) if it only explains |
| P2-009 Community Member Handbook (gen-1) | §3.1 | (e) lost (Confluence 70451229) | Record seat | If reissued: (d) only. Member rights live only in the text |
| P2-010 Director of Remote Policy (gen-1) | §8.1, by its title | (e) lost (Confluence 70680651); number retired | Secretary keeps the row | Annotation only |
| P2-011 Volunteer Recruitment Policy (gen-1) | §14.4 | (e) lost (Confluence 70451251) | The office P2-005b names | If reissued: (c) under P2-005b |
| P2-012 Policy Archiving and Preservation Policy (gen-1) | §14.9, pointer at §2.5 | (e) draft (Confluence 71303182). Its body says "P2-002", a clerical error to annotate | Board; Record seat | Merged into P2-001 v2.0, then superseded |
| P2-013 Global Community Programs Policy v1.0 | §1.4(d) | (e) draft (canvas F09J338M2G5, header "P2-[TBD]") | Board; the entering act names the keeping office | Board act. Its program charters become (c) |
| P2-013-A Lost Sheep Research Fellowship Program Policy | §1.4(c) | (e) lost (only the space overview, Confluence 77889774, survives) | The office P2-013 names | If reissued: (c) charter under P2-013 |
| P2-014 "NAGA" | §1.4(d) | (e) cited only by P2-003; no text exists; number retired | Secretary keeps the row | Annotation only |

The four fixes P2-003 needs before adoption:

1. Line 64 lists "AGPL-3, MIT, Apache 2.0, GPL v3, etc." as a project's chosen license, and line 133 lists "AGPL-3, MIT, Apache 2.0, etc." Both must yield to §9.4.
2. The Board decides Gitee. The original canvas prohibits it. The local canonical copy lists it as a Tier 2 option (line 279) by Presidential directive.
3. Cite P2-002 instead of the textless P2-014. In the canvas copy only, change the "P3-001" template citation to P3-001a.
4. Replace "Program Director" with an office that exists under [§8.1][v10-8.1].

**P3 series**

| Document | Place | Class and status at opening | Owner, kept by | Changed afterwards by |
|---|---|---|---|---|
| P3-001 LBTAS whitepaper (research edition) | §9.8 | (d) informative (Confluence 84508688; unpinned) | Institute; Covenant seat | Secretary annotation |
| P3-001a NTARI Whitepaper Template (gen-1) | §1.4(c) | (e) lost (Confluence 65208351) | Record seat | If reissued: (c) of the Secretary |
| P3-001b TechSoup API Integration and Compliance Framework | §1.2 | (d) informative (Confluence 69664771) | Institute; Economy & Information seat | Secretary annotation |
| P3-002 The Agrinet Whitepaper | §9.1 | (d) informative. English text only on Agrinet branch `refactor/mycelium-operator-witness` (blob `25694dd`); re-pin to `main` after merge. The GPL-3 notice on Confluence copy 2949125 is annotated | Institute; Economy & Information seat | Pull request; recorded by the Secretary |
| P3-002a How to Vote (gen-1) | §6.9 | (e) unverified (Confluence 69337101, content not read) | Secretary keeps the row | Input to the §6.9 procedure only |
| P3-003 Conceptual Diagnosis | §1.4(c) | (d) informative; known only from channel C09N9K91ZBL. A 2026-03-18 elimination proposal has no recorded outcome | Institute; Governance seat | Number never reused |
| P3-003a Volunteer Records Management Handbook (gen-1) | §14.2 | (e) lost | Record seat | If reissued: (c), bounded by §2.4 |
| P3-004 Global Distribution Strategy for Mass Production Networks | §13.1, beside P2-003 | (d) informative (ntari.org post; Confluence 84082693 and canvas F09PG3FF0TA are copies) | Institute; Substrate seat | Secretary annotation |
| P3-005 The Optimal Languages for NTARI's Global Broadcast v2.0 | §1.4(d), beside P2-002 | (d) informative. Its "operative pending ratification" line has no effect; only P2-002 can make languages operative | Institute; Record seat | Secretary annotation |
| P3-006 Why We Publish Under AGPL-3 | §9.4 | (d) informative (ntari.org post) | Institute; Governance seat | Secretary annotation |
| P3-007 Q-Zoo QUBO Problem Application Method | §1.4(c) | (d) informative; text not located | Institute | Secretary annotation |
| P3-008 How to Analyze Network Datasets for Q-Zoo | §1.4(c) | (d) informative | Institute | Secretary annotation |
| P3-009 Quantum Network Analysis | §1.4(c) | (d) informative. The proposal to reassign P3-009 to the Material Culture paper is refused (see its row below) | Institute | Number never reused |
| P3-010 (unverified) | §1.4(c) | (e) reserved, not issued, until the Secretary resolves it | Record seat | Annotation only |
| P3-011 Janus Facing Applications v2.1 | §9.1 | (d) informative, branch only (blob `abc6c09`). The web v1.0 is listed as superseded | Institute; Governance seat | Pull request |
| P3-012 Agrinet Protocol Specification v0.3 | §9.1, pointer at §5.1 | (e) draft, branch only (blob `55cca71`). Target: (c) | Economy & Information federation, kept by the Treasurer's office | Federation majority (§6.5 third paragraph). Rules meant to bind conformance go through §9.2 |
| P3-012a Municipal Counter-Automation | §9.4 | (d) informative (ntari.org post labeled P3-012) | Institute; Governance seat | Secretary annotation |
| P3-013 Mycelium: The Immutable Transaction-Record Ledger v0.3 | §9.1, pointer at §2.5 | (e) draft, branch only (blob `745272e`). Its declared home NTARI-RAND/Mycelium now redirects to NTARI-RAND/Tell | Record federation, kept by the Secretary's office | Federation majority; binding rules through §9.2 |
| P3-014 LBTAS Specification v0.1 | §9.8 | (e) draft on LBTAS `main` (`SPEC.md`; pin a commit). Target: (c) guidance | Covenant federation, kept by the President's office | Guidance: federation majority. Covenant rules: only §9.2, because §9.8 lets the Institute amend LBTAS only that way |

**Unnumbered documents and empty slots**

| Document | Place | Class and status at opening | Owner, kept by | Changed afterwards by |
|---|---|---|---|---|
| DCO contribution rule (CONTRIBUTING files, DCO check, org rulesets) | §9.4 | Split. The rule goes into the §9.4 text. The mechanics are (c), in force as practice, to be confirmed by a recorded act ([bylaws CONTRIBUTING L22-38][contrib-22]) | Rule: membership. Mechanics: Substrate seat | Rule: Article XV only. Mechanics: the office, never below §9.4 |
| Voting Workflows (canvas F0CE24ZEW1J) | [§6.9][v10-6.9] | (b) required slot, **vacant**. The canvas is listed in (e) as a draft in use. Takes a fresh number | Board adopts (KRS 273.195(2)); kept by the Governance seat; the Secretary files results | Board act; the delegates may set it aside |
| Research & Development Submission Guide (canvas F0BTB5N93A9) | §5.2 | (e) draft in use. Target: (c) issued by the office the §6.9 policy names | That office; the Secretary keeps it | The issuing office; the Board may revoke |
| Volunteer Handbook (Q-Zoo, Confluence 19333121) | §14.4 | (e) draft | The office P2-005b names | If issued: (c) under P2-005b |
| ntari.org Privacy Policy (effective 2026-01-27) | §2.4, pointer at §14.2 | (b) "published notice" under §16.4. The Secretary commits a copy so it is pinned | Board; kept by the Record seat, with the Treasurer for donor data | Board act |
| ntari.org Terms and Conditions (effective 2026-01-27) | §9.4 | (b) "published notice". Its part 4 software-license line ("MIT, GPL, AGPL-3 or Apache") is void to the extent it conflicts with §9.4 | Board; Record seat | Board act, replacing part 4 with the §9.4 floor |
| SoHoLINK product policies (AUP, Privacy, Terms, DMCA, Law Enforcement, Security; SoHoLINK `167f15b`) | §10.2, pointer at §8.6 | Templates operators adapt, not Institute rows ([§10.7][v10-10.7]). For a deployment the Institute runs: (b), not in force until adopted. Whether it runs soholink.org is unverified | Board; Substrate seat | Board act |
| Repository codes of conduct and security policies (for example developer-portal `CODE_OF_CONDUCT.md` and `SECURITY.md`) | §14.6 (conduct); §13.1, pointer at §8.6 (security) | (e) repository texts with no adoption record, but policies in substance. Target: (c), one organization-wide text each, the security text beside Entries 6–7 | Substrate seat; the Board for any conduct rule with a sanction | The office. A conduct rule may never add a membership test (§14.6) or a sanction outside Article XII |
| Conflict-of-interest policy | [§14.3][v10-14.3] | (b) required slot, **vacant**. The most urgent gap: §14.3 requires it, and registry Entry 5 already makes §14.3 disclosures | Board; the Secretary records disclosures | Board act; approvals by a disinterested majority |
| v1.1 §16.2 "internal policy" for publishing bootstrap tiers | §16.2 | Exists only if v1.1 is adopted ([v1.1 L397-401][v11-16.2]); vacant | Proposed: the Record seat with Board authorization, not the founder board alone, since it decides when the founder board's power ends | §14.10 |
| NTARI-MESH-001 (Confluence 92930049), an architecture document under a fourth numbering scheme | By its title, under §14.9, until read | (e) unverified; content not read | Secretary keeps the row | It keeps its own label, and takes a P-number only if it proves to be a policy |
| The Material Culture of Democratic Deliberation (research paper) | §1.4(c) | (d) informative. Proposed on 2026-03-18 to take P3-009; it takes a fresh P3 number instead | Institute; Governance seat | Secretary annotation |
| Executive Actions (EX-###) | Not in Schedule P | P2-001 itself says EX items are tasks, not policies | Secretary, under P2-001 | n/a |

### Number collisions

**The answer.** One number names one document, forever. Where a number was used more than once, the bare number stays with the use the bylaws, the registry or the official document cites. If none is cited, it stays with the most recently issued use. Every other use takes a lowercase suffix (a, b, c) in order of first record.

The inventory and the verification found these collisions:

- **P1:** P1-003 four uses, P1-004 two, P1-005 two, P1-006 two.
- **P2:** P2-002 two (plus P2-012, whose body says "P2-002"), P2-003 three, P2-004 at least four, P2-005 at least five, P2-006 two.
- **P3:** P3-001 three, P3-002 two, P3-003 two, P3-012 two.
- **Other schemes.** Confluence also used a fourth scheme for architecture documents ("NTARI-MESH-001"). Schedule P files such documents under their own labels.

P2-001 bars reuse only for executive-action numbers. It has no register and no reuse rule for P1/P2/P3 numbers (P2-001 L318-325, L210-215). Proposed §14.10 adds the rule. It also refuses the 2026-03-18 proposal to drop P3-003 and renumber P3-004 to P3-009. The Secretary should confirm each suffix at opening, since three documents found only as citations in the v3.1 draft were added late.

### The new bylaws text

**The answer.** Eleven changes: seven amended provisions, three new sections in Article XIV that put Schedule P into the bylaws, and one new transition section, plus four informative appendix rows. Every changed section has the same number in v1.0 and v1.1, and §14.8–§14.10 and §16.4 are unused in both.

**Tested.** These exact texts, read by script from this note, including the four appendix rows, were applied to v1.0 and v1.1 in a scratch clone of bylaws at `3276781`. The repository's own suite passes all checks B1–B8 on both:

- v1.0: 108 provisions; 254 section references, all resolving.
- v1.1: 112 provisions; 370 section references, all resolving.

B7 checks only that the seven translations exist; they would still need updating.

**How it is adopted.** These changes ride a §16.1 bootstrap act. They should be folded into the pending v1.1 adoption, which already takes effect only that way ([v1.1 L3-5][v11-hdr]). They must never be made by editing v1.0 in place: the README says the adopted text is "never patched" ([L53-58][readme-53]), and v1.1 says v1.0 stays in the record unchanged.

#### §7.4 Action (replace; v1.0 L157)

> **7.4 Action.** The Board acts in meetings, synchronous or asynchronous, on one week's notice to its members, a majority constituting a quorum and a majority of those present deciding. Board proceedings are open to observation by members, and their records are kept under §2.5. The Board holds no recurring meeting requirement: it may act without a meeting by written consent signed by every director in office, under KRS 273.375, and such consents may be gathered continuously, each recorded under §2.5 like any other proceeding.

Why: it states the all-director rule that applies today. KRS 273.375 makes unanimity the default, and v1.0 §7.4 does not depart from it.

#### §7.5 Reserved powers (first sentence; v1.0 L159)

> **7.5 Reserved powers.** The Board may not amend these bylaws, other than Schedule P as §14.10 provides, amend the official document, expel any party, dispose of the Institute's stewardship of the official document or the conformance suite, or dissolve the Institute. *[remainder unchanged]*

#### §8.4 Secretary (one clause; v1.0 L173)

Replace "maintains the governance registry of §9.5," with "maintains the governance registry of §9.5 and Schedule P under §14.9,".

#### §9.4 Licensing floor (replace; v1.0 L189)

> **9.4 Licensing floor.** Every work the Institute publishes, software and documents alike, JFA software, the conformance suites, these bylaws, its policies, research, and educational material included, is licensed under the GNU Affero General Public License, version 3 [or any later version | only] (AGPL-3.0); the official document alone keeps the license its own text states, which changes only under §9.2. The floor moves only toward stronger copyleft: the membership may, by amendment under Article XV, name a successor license that keeps every freedom and every reciprocal obligation of AGPL-3.0, the duty to offer source to network users included, and no act moves a work to a weaker license. Work the Institute did not write keeps its own license, and the Institute's changes to it follow this floor wherever that license allows. The Institute never relicenses any work into proprietary terms and never offers a work under a second license for any party's private advantage. It accepts a contribution only when each commit carries a sign-off under the Developer Certificate of Origin by the commit's author, and that check admits no bypass; the author keeps the copyright, and the Institute takes no assignment of copyright and requires no contributor license agreement, so that copyright stays spread among those who wrote the work. It signs no agreement that would let any party — including the Institute — close what is open.

The license itself is no longer a choice: Entry 9 decided AGPL-3.0 for documents and code. Two choices are left to the founder board, after the federation deliberates:

- **The bracket.** AGPL "or any later version" or "only". See [Or later, or only](#or-later-or-only).
- **The transition period** in §16.4 (proposed: ninety days).

Today v1.0 §9.4 names only "JFA software" under AGPL-3, then says "never relicenses either" with no second object. The sign-off is the commit author's, as the DCO check enforces; DCO 1.1 lets that author certify work they did not write, such as compatible code.

#### §9.5 The governance registry (replace; v1.0 L191)

> **9.5 The governance registry.** The Secretary maintains a public, append-only governance registry recording: recognitions and lapses of membership; the publications of Article XI; expulsions, readmissions, and re-entries under Article XII; each amendment of the official document and of these bylaws; and each act that enters, amends, ratifies, sets aside, or retires an entry of Schedule P under §14.10, with the vote or the signed consents by which it was taken. The registry honors §2.4.

For v1.1 (L199), keep its clause ", and the federation elections and changes of §3.9" after "recognitions and lapses of membership". Today's list leaves out policy adoption ([v1.0 L191][v10-9.5]).

#### §14.3 Conflicts of interest (replace; v1.0 L331)

> **14.3 Conflicts of interest.** Every director, officer, and delegate discloses any interest they hold in a matter before acting on it, and abstains where the interest conflicts. A transaction in which a director holds a direct or indirect interest is authorized, approved, or ratified only after disclosure, by a majority of the directors who hold no interest in it, and never by a single director. The Board maintains a conflict-of-interest policy consistent with the Institute's federal recognition as a board policy in Schedule P; disclosures are recorded under §2.5.

Why: a check on the Board must sit where the Board cannot lift it. KRS 273.219 only denies a single director's approval its safe harbor. The outright bar goes further by choice. The founder board's size, and so whether a disinterested majority can exist today, was not confirmed. Where none can be formed, the matter waits under this text. Other routes are a federation question ([Question 18](#questions-for-federation-governance)): a members' decision, or relying on the director to prove the transaction fair (KRS 273.219(1)(b), (4)).

#### §14.8 Order of instruments (new, after §14.7)

> **14.8 Order of instruments.** Where instruments conflict, the higher controls, in this order: law, including KRS Chapter 273 and the requirements of the Institute's federal recognition; the articles of incorporation; the official document, with its invariant registry, which §9.16 amends as part of it, and the twelve lines, which no amendment may override (§15.2); the text of these bylaws; the executable conformance suite and the dispute-mechanics design, as §1.5 binds them; the board policies of Schedule P; and the office and federation procedures of Schedule P. Within one rank the later controls the earlier. An entry of Schedule P that conflicts with a higher instrument is void to the extent of the conflict, and is otherwise read to serve Article II. A document's number and series are filing labels and decide neither its rank nor who may change it. The English text of every instrument controls; a translation is made for reach, not for interpretation.

Notes:

- **What it fixes in P2-001.** P2-001's hierarchy (L183-190) leaves out the articles and the official document, and cites pre-v1.0 bylaws from 2025.
- **The invariant registry** sits with the official document because [§9.16][v10-9.16] makes every change to it an amendment of the official document.
- **A proposal to confirm.** The bylaws do not state outright that the suite and the dispute design rank below the text.
- **The last sentence is a new rule.** The bylaws README attributes it to "P2-002 §2.2" ([README L62-63][readme-62]), but P2-002 §2.2 has no such rule, so that citation needs correcting.

#### §14.9 Schedule P (new)

> **14.9 Schedule P.** Every policy of the Institute, and every document filed in its policy series, has one place in Schedule P, the register of policies the Secretary keeps beside these bylaws in the Institute's public repository of them. Schedule P is a code of these bylaws kept under §14.10 rather than Article XV; it is not their text, and no entry restates or alters their text. It is arranged by the Article and section of these bylaws that each entry serves, so that a reader of any Article finds there every policy on its subject; an entry that serves more than one section is placed once and pointed to from the others. Each entry states its number, title, version, the section it serves, its class, its owner and the office that keeps it, its status, the registry entry recording the act, and where its text is kept. The classes are:
>
> (a) cited instruments: the articles of incorporation, the instruments §1.5 defines, and the versions of these bylaws, each cited and never restated, and each amended by its own path;
>
> (b) board policies, adopted by the Board within a section of these bylaws that the entry names, including the policies these bylaws call for — the venue of §5.6, the deliberation procedure of §6.9, and the conflict-of-interest policy of §14.3 — each shown vacant until one is adopted;
>
> (c) office and federation procedures, each issued by the office or federation the entry names, within the area §§8.2–8.6 give that office, the protocol §5.1 gives that federation's channel, or the duties a board policy gives it;
>
> (d) informative documents: research and other writing that analyzes and never governs; a rule drawn from one binds only when it is adopted into these bylaws or as a board policy or procedure; and
>
> (e) documents not in force: drafts, documents awaiting ratification under §16.4, superseded and withdrawn versions, lost texts, retired numbers, and numbers not yet verified.
>
> Only an entry of class (b) or (c) marked in force, or marked a published notice under §16.4, binds, and only for the version it names. An entry is marked in force only when its text is published where members can read it, at a fixed location that cannot change under it: a commit of a public repository of the Institute, or a registry entry carrying the text or its digest. A reference to a moving branch, and a text held only in a proprietary venue, incorporates nothing (§5.6, §13.1). No entry may create or alter a class of membership or a member's rights, set a member's vote, quorum, or notice outside the limits §6.4 and §6.5 set, set the number, election, term, or removal of directors, exercise a power §7.5 reserves, or insert the Board as a gate §7.6 forbids; an entry that attempts any of these is void to that extent, and the matter is taken up under Article XV.

Why "outside the limits": the §6.9 deliberation procedure is a class (b) slot and may set a window and a majority, but only within §6.4 and §6.5. By the inventory's reading of Voting Workflows (not re-read here), its 7-business-day window survives, since it gives at least §6.4's one week, and so does its simple majority, read as a majority of votes cast (§6.5). Its rule that no pull request merges without a federation vote is a deliberation choice to settle ([Question 6](#questions-for-federation-governance)).

#### §14.10 Changing a policy (new)

> **14.10 Changing a policy.** The Board enters, amends, ratifies, and retires board policies by action under §7.4. An office or federation issues, amends, and retires its procedures — an office by a recorded act of the officer, a federation by its internal majority under §6.5 — and never for its own powers or duties, which these bylaws and the Board set; a procedure that commits the Institute's funds or binds it to an outside party takes effect only when the Board also authorizes it under §7.4, and the Board may amend or revoke any procedure by the same action. The checks on a board policy are the recall of §6.8 and setting aside by the delegates: any member may propose that a board policy be set aside, and a set-aside noticed under §6.4 and carried as §6.5 provides is a decision of the membership, open under §2.3 and §6.7. The Secretary makes entries of classes (a), (d), and (e) of §14.9 ministerially, enters every proposed policy as a draft, and annotates an entry when its status changes; a refusal to make an entry states which requirement failed and is challengeable through Article XII, as under §3.3. Every act under this section takes effect when recorded in the governance registry under §9.5 with its text published as §14.9 requires; entries are corrected by annotation or a new version under §2.5, never rewritten or deleted, and remain open under §2.3. A number names one document and is never reissued; where a number was issued to more than one document, Schedule P records each use under a distinguishing suffix. Making or annotating an entry by these acts is not an amendment of the text of these bylaws.

Why the set-aside is spelled out: reopening under [§6.7][v10-6.7] reaches only decisions of the membership ([§2.3][v10-2.3]), and [§6.5][v10-6.5] is only a quorum-and-majority rule. Without this sentence a Board policy would have no member check, which [§2.2][v10-2.2] forbids.

#### §15.1 By the membership alone (amend; v1.0 L345)

> **15.1 By the membership alone.** These bylaws, other than Schedule P, are amended only by a majority vote of the delegates, each federation having decided under §6.5 with every member of that federation holding the vote, prosumer members included, in a ballot noticed under §6.4 carrying the full text of the amendment. Schedule P is kept under §14.10.

#### §16.4 Transition (new, after §16.3)

> **16.4 Transition.** Until bootstrap ends, the founder board serves as the Board for every act under §14.10, and takes those acts under §7.4 as the Board, not in exercise of the membership's powers under §16.1, so that a later Board may revisit them. A policy approved before 2026-08-31, when version 1.0 of these bylaws took effect, or claimed as adopted with no record of the act, does not bind until the Board ratifies it, conformed to these bylaws, by an act recorded under §9.5; until then its entry is marked awaiting ratification. A notice the Institute has published to the public stays in effect as published until the Board confirms, replaces, or withdraws it; the Secretary commits a copy of it under §14.9 when making its entry, and that copy is the version the entry names. A policy not ratified when bootstrap ends under §16.2 is marked superseded. Acts already taken in reliance on such a policy stand, and remain open under §2.3. Works published before §9.4 took its present form keep the licenses they carry (§13.2), and within [ninety] days the Institute brings into §9.4 every such work whose copyright it wholly holds.

Why: v1.0 has no savings clause. Its header supersedes only the v6.0–v8.0 bylaws ([v1.0 L5][v10-hdr]). P2-004 (approved in Slack on 2026-02-15) and P1-003 (accepted 2026-04-21) both predate v6.0, which the verification dates to June 2026, so a test by bylaws line might miss them. A date does not.

The published-notice sentence keeps the website Privacy and Terms in force without breaking the pinning rule: their pinned version is the committed copy. The last sentence gives the new §9.4 a transition: on adoption day, any work not yet relicensed under Entry 9 still carries its old license.

#### Appendix: four provenance rows (informative)

| Provision | Demand | Source |
|---|---|---|
| §9.4 (as amended) | AGPL-3.0 for every work, software and documents, until a stronger copyleft; the official document keeps its own license until §9.2; DCO sign-off with no bypass; authors keep copyright; no assignment | President's direction of 2026-11-13; governance registry Entries 4 and 9; P2-004 parts 2 and 3, as amended and corrected |
| §14.3 (as amended) | No conflicted transaction approved by a single director | KRS 273.219(3), which denies a single director's approval its safe harbor; the bar goes further by choice |
| §14.8 | Order of instruments: law, articles, official document and invariant registry, bylaws text, suite and dispute design, board policies, procedures | P2-001 Authority Hierarchy, corrected; §1.2; §15.2; KRS 273.247(4) |
| §14.9, §14.10, §16.4 | Every policy has one place, filed under the section it serves; authority by class, not series; pinned by commit; numbers never reissued; pre-v1.0 policies ratified only as conformed | KRS 273.161(6), 273.191, 273.228; P1-001 v8.0 Appendix B precedent; §9.16 (identifiers never reused); President's direction of 2026-11-13 |

### The Schedule P file

**The answer.** A new file in NTARI-RAND/bylaws, `P1-001_Schedule-P_Register-of-Policies.md`. It is not the suite's target file, so checks B1–B8 are unaffected. Its opening looks like this:

```markdown
# Schedule P — Register of Policies

Schedule P to P1-001 · a code of the bylaws kept by the Secretary under
§14.9 and §14.10 · opened by governance registry Entry [n]

Every policy of the Institute has one entry here, filed under the bylaws
section it serves. Only an entry of class (b) or (c) marked in force, or
a published notice, binds, and only for the version it names. The text of
the bylaws controls every entry (§14.8). English is authoritative.

## Rules of the register

1. Where an entry sits: under the section whose subject it puts into
   practice. A document serving several sections sits once, with pointer
   rows elsewhere. A document whose subject is unknown sits by its title,
   or under §14.9.
2. Columns: Number · Title · Version · Serves · Class · Owner / kept by ·
   Status · Registry entry · Text (repository @ commit : path).
3. Status: in force · published notice · vacant · draft · awaiting
   ratification · superseded · withdrawn · lost · retired · unverified ·
   informative · cited · pointer.
4. Numbers: one number, one document, never reissued. Collided numbers
   keep the bare number for the cited (else most recent) use; other uses
   take a lowercase suffix in order of first record.
5. Citing: bylaws sections with the section sign; parts of a policy
   without it (P2-004 part 3.1). Entries name offices, never people.
6. Where texts live: NTARI-RAND/Policies, one file per version. Protocol
   specifications stay beside their code. A Slack canvas, web post,
   Confluence page or local file is a copy.
7. Not policies: executive actions (EX-###) and single-matter registry
   decisions get pointer rows only.
8. Review: the Board reviews each board policy yearly; issuers review
   their procedures yearly; a draft untouched for twelve months is
   annotated as lapsed.

## Article V — Federation Channels

| Number | Title | Ver | Serves | Class | Owner / kept by | Status | Registry | Text |
|---|---|---|---|---|---|---|---|---|
| P1-005 | Governance Venue Policy | 1.0 | §5.6 | (b) | Board / Workspace Administrator | vacant; draft listed | — | to commit and pin |
```

The remaining rows follow the placement table above, one per document, under the section each serves.

A follow-up suite check is recommended: every row names an existing section, a class and a status, and every in-force row names a commit or registry digest.

### What this design does not settle

- **If counsel rejects a Board-kept code of the bylaws.** The fallback keeps Schedule P as the one register but drops its claim to be a code of the bylaws. Board policies then bind as Board resolutions within the slots the bylaws text names (KRS 273.207, 273.228, 273.195(2)), every class (c) entry needs Board authorization, and any rule that is a bylaw in substance moves into the text under Article XV.
- **Officer-made and federation-made procedures.** A class (c) procedure issued by one officer or by a federation would be part of a code of the bylaws. KRS 273.191 lets the bylaws "provide otherwise", so this is not plainly unlawful, but it sits uneasily with KRS 273.228, which gives officer duties to the bylaws or the Board. Counsel should confirm it. The fallback: Board authorization for every class (c) entry.
- **The delegates' set-aside and the board's management power.** The set-aside is a member power stated in the bylaws, which KRS 273.201 allows. How it interacts with KRS 273.207 (the board manages) is unverified.
- **The member check during bootstrap.** The set-aside needs a delegates' ballot with at least three federations casting (§6.5), which cannot happen during bootstrap. Meanwhile the same founder board adopts Board policies (§16.4) and holds the membership's powers (§16.1), and §2.2 voids a power without a check. Two candidate checks for today: any member's set-aside petition in #federation-governance gets a recorded founder-board answer; or Board policies adopted in bootstrap lapse unless the first post-bootstrap Board reconfirms them ([Question 17](#questions-for-federation-governance)).
- **Validity of past acts.** Registry Entries 3–6 were "decided by the President, for the founder board", and Entry 8 by the President, with no all-director consents recorded. Whether they meet KRS 273.375, or KRS 273.377 where the founder board used the membership's powers, is unverified.
- **After bootstrap.** Whether asynchronous majority ballots are valid member action under KRS 273.377 and 273.195 is unverified. It changes the later path for the §9.4 floor, not the placement.
- **Ranking of the suite and dispute design.** The bylaws do not state it outright. The dispute-mechanics design also has no amendment path in the bylaws, although it was revised on 2026-10-07 ([Janus L3][j-dispute]).
- **The v1.0 §10.8 fragment.** It is an incomplete sentence ([L267][v10-10.8]); v1.1 completes it. P2-004's enforcement pointer hangs off it until v1.1 is adopted.
- **Unread texts.** Several Slack canvases and files were never read and may hold further policies that need rows: Membership Types, Working Group Charters, Appendices A and B, How Federation Members Vote, NTARI Workflows - Broadcast Specification (F0BB2DXP8CT), an unidentified canvas (F09QYU8PW3S), two proposal canvases, and a "32-policy-governance-voting" file. The Secretary should read them before opening Schedule P.

### Sequence

**The answer.** Notice first, then the §9.4 choices, one bylaws act, and a short series of Board acts.

1. **Give the federation notice.** Post this note to #federation-governance. Notice is not required during bootstrap, but it lets members object first. One week ([§6.4][v10-6.4]) is a minimum. #federation-governance deliberates with no deadline, so the founder board acts once deliberation settles, or records why it acts sooner.
2. **Decide the §9.4 choices.** The documents license is decided (Entry 9: AGPL-3.0 for everything). The founder board decides "or any later version" versus "only", and the §16.4 transition period. Once adopted, only the membership can change them.
3. **Get the articles of incorporation.** Pull the filed articles from the Kentucky Secretary of State and read them. They outrank the bylaws (KRS 273.247(4)), and P2-004 claims they hold a covenant.
4. **Publish the governance registry.** Commit GOVERNANCE-REGISTRY.md to a public repository, for example NTARI-RAND/bylaws, and pin it. Until then, only commits serve as pins. Annotate Entry 1, whose link points to a local copy of v1.0 that differs from the adopted text at §6.7 and §12.5.
5. **Commit the canonical texts.** Commit every text a binding or awaiting entry needs to NTARI-RAND/Policies, and widen its README scope beyond "P2 and P3 series". Start with what exists only in Slack canvases (P2-004, P1-003, Voting Workflows), local files (P2-001, P2-002, P2-003, P2-005, P2-006, P3-005), Wix (Privacy, Terms) and Agrinet branches (P3-002, P3-011 to P3-013). Diff the local P2-001 against canvas F09MSHV2DC2 first. Then mark each canvas and web copy with a banner naming the pinned commit ([Question 23](#questions-for-federation-governance)).
6. **Bootstrap act (§16.1).** Adopt the eleven bylaws changes as part of the v1.1 adoption, or as a new version file, never by editing v1.0 in place. Record it in the registry with the signed consents counsel confirms (every director under KRS 273.375, or every voting member under KRS 273.377). Update the seven translations (suite B7). In the same act, or before it, bring NTARI's own works into §9.4:
   - relicense GovOS and governance-rand from GPL-3.0 to AGPL-3.0, keeping the governance-rand#2 report under GPL-3.0 unless its author agrees otherwise;
   - relicense the eleven CC BY-SA 4.0 repositories (bylaws, Policies, the four *-rand research repositories and the five seeds) to AGPL-3.0, each notice saying that versions already published stay available under CC BY-SA 4.0;
   - add SPDX AGPL-3.0 headers where files carry none, `bylaws-conformance-suite.py` included.

   Entry 9 directs this relicensing now, so it need not wait for the bylaws act.

   Then update the bylaws README and CONTRIBUTING. CONTRIBUTING L3 limits the repository to P1-001, and [L9-13][contrib-9] tells contributors to edit v1.0 in place and has the Board approving amendments in review; point it at new version files instead. Route open bylaws PR #8 into the next version file: it edits v1.0 in place, and its new §9.19 collides with v1.1's §9.19.
7. **The same day, open Schedule P.** The Secretary opens it by a registry entry and makes every opening row in the status the placement table gives.
8. **Board acts.** The founder board, acting as the Board under §7.4 and recorded in the registry:
   - (a) adopt P1-005 with its header corrected;
   - (b) adopt a conflict-of-interest policy;
   - (c) ratify P2-004 v2.0, with a registry entry disposing of the CLA text sent to volunteers;
   - (d) confirm Entries 6–7 as the repository security defaults, and Entry 8's reading;
   - (e) ratify P1-003 as v2.0, or retire it.
9. **For the rest of bootstrap:**
   - P2-001 v2.0, absorbing P2-012;
   - the §6.9 deliberation procedure, from Voting Workflows reconciled with the R&D Guide and Entry 4;
   - P2-002, with the seven-language directive;
   - P2-003 with its four fixes;
   - P2-005 and P2-006;
   - one officer-duties policy;
   - the volunteer umbrella policy and its procedures;
   - P2-013;
   - the Privacy and Terms confirmations;
   - the federation procedures for P3-012 to P3-014.
10. **Housekeeping:**
    - Give the Material Culture paper a fresh number.
    - Make the bylaws Conformance check a required check on `main`. Today only DCO and one review are required, though `conformance.yml` L3 says otherwise.
    - Fix the README's "not yet published" note on the dispute design, its missing P1-005 and its P2-002 citation.
11. **At the end of bootstrap,** anything still awaiting ratification is marked superseded (§16.4).

## Correcting P2-004 §3

**The answer.** P2-004 part 3 should say what NTARI already does and what its bylaws already demand:

- Authors keep their copyright.
- NTARI takes no assignment and requires no CLA.
- Every commit carries a DCO sign-off by its author, with no bypass.
- NTARI's covenant binds the copyright it holds and its own conduct.
- Contribution earns credit, never governance weight.

These parts are struck: part 3.1 (NTARI as copyright trustee by assignment), 3.2 (the CLA), 3.4 (governance seats by line count), 7 (the CLA template), the CLA rollout in part 10, and the part 4.2 "Option C" settlement. The floor moves into bylaws §9.4, so neither the Board nor an officer can reverse it.

### What part 3 says now

The canonical text is Slack canvas F0AFYMXLCJU (effective 2026-02-15, "Authority: Board of Directors"). The [public post](https://www.ntari.org/post/licensing-and-enforcement-strategy-ntari-policy-p2-004) (published 2026-02-16) has nearly the same body (the inventory found one §7.2 bullet missing) and leaves out the whole header block.

| Part | What it says |
|---|---|
| 3.1 | NTARI is "trustee of the commons" and holds unified copyright. Contributors assign their copyright to NTARI |
| 3.2 | Every contributor signs NTARI's CLA before any contribution is accepted. The CLA assigns copyright, gives NTARI enforcement authority, binds NTARI to covenants and keeps work in the commons |
| 3.3 | Claims the Articles and Bylaws already hold four irrevocable commitments: code stays "AGPL-3 or more permissive copyleft"; no dual-licensing for profit; on dissolution copyrights go to the SFC or similar, or revert to contributors; and a "mission lock" |
| 3.4 | Governance rights by contribution volume: a CONTRIBUTORS listing for any contribution, Community Advisory Board eligibility at 100+ lines, a voting seat on it at 1,000+ lines. The board gives non-binding input |
| 7.1–7.2 | An eight-clause CLA ("You hereby assign to NTARI all worldwide copyright…") collecting legal name, email, mailing address, username and employer. Signed by DocuSign or mail and kept in a contributor database. Merges are blocked without it, and a public list shows each person's CLA status |
| 10 | Month 1: adopt by Board resolution and "Implement CLA requirement on all repositories" |

**Its status.** In #p2-004-licensing-enforcement (C0AFHBH3MU1) on 2026-02-15, the President asked two people to review it "for approval". Both replied "Approved" the same day. It has no registry entry; the registry opened 2026-09-08. Two things are unverified: whether both approvers were directors then, and whether the record meets KRS 273.375's every-director rule. Under proposed §16.4 it waits as "awaiting ratification".

### What it conflicts with

**The answer.** The CLA model conflicts with practice, with the bylaws in force, and even with the bylaws draft of its own time.

| Clause | Conflicts with | Source |
|---|---|---|
| 3.2, 10 (CLA before merge) | Practice. All 27 NTARI-RAND repositories have an active "Require DCO" ruleset with the `DCO` check required and no bypass actors. The installed org apps include `dco` and no CLA app. No repository has a CLA file | GitHub API, 2026-11-13; registry Entry 4 (L116): the DCO check "has no bypass" |
| 3.1, 3.2, 7.1 cl.2 (assignment) | Published contributor terms. SoHoLINK's CONTRIBUTING (merged 2026-07-09) and LBTAS's contributing.md (merged 2026-07-14) both say inbound = outbound, no CLA, copyright stays with the author | SoHoLINK CONTRIBUTING L7-19; LBTAS contributing.md L153-160 |
| 3.1, 7.1 cl.2 ("including the right to sublicense") | Bylaws [§9.4][v10-9.4]: NTARI "signs no agreement that would let any party — including the Institute — close what is open". A sole owner with a right to sublicense could relicense, leaving only a promise as a guard | v1.0 L189 |
| 3.1, 3.2 (assignment), 3.3 item 1 ("more permissive") | The bylaws draft of its own time. The v3.1 draft (December 2025) had contributors license, not assign (§6.2). It allowed only licenses of "equal or superior protection" (§1.4, §6.1). Whether v3.0 or the v3.1 draft was in force on 2026-02-15 is unverified | Slack file F0A3PM5NBUN |
| 3.3 item 1 ("AGPL-3 or more permissive copyleft") | The President's direction: "AGPL-3 across the board until a stronger version of copyleft appears". "More permissive" points the other way. Code search finds "AGPL-3.0-or-later" 84 times across six repositories and "AGPL-3.0-only" nowhere | GitHub code search, 2026-11-13 |
| 3.3 lead-in (commitments "in the Articles and Bylaws") | The bylaws carry the substance of items 1–2 only ([§9.4][v10-9.4], [§13.2][v10-13.2]). They name no SFC, no reversion to contributors and no "mission lock". [§13.3][v10-13.3] has the membership name a successor steward. The articles were not read | v1.0 L189, L319, L321 |
| 3.3 "irrevocable" | A Board policy cannot make itself irrevocable. Decisions stay open ([§2.3][v10-2.3]) and the membership amends the bylaws (§15.1). True instead: "changeable only by the membership" and "no act may impair a license already granted" (§13.2) | v1.0 L45, L345, L319 |
| 3.3 item 3 (copyrights revert to contributors on dissolution) | A risk under the federal rule that an exempt organization's assets stay dedicated to exempt purposes ([Treas. Reg. §1.501(c)(3)-1(b)(4)](https://www.law.cornell.edu/cfr/text/26/1.501(c)(3)-1)). A reversion reserved in the original grant might differ, so this is for counsel. §13.3 and the no-assignment model are reasons enough to drop it | Regulation text; v1.0 L321 |
| 3.4 (seats by line count) | Bylaws [§3.4][v10-3.4]: "Governance weight, like credit, is never bought". Also [§3.7][v10-3.7] and §2.2. The bylaws have no Community Advisory Board. Advisory committees are lawful if they do not bind (KRS 273.221(4)), so striking 3.4 is a policy choice | v1.0 L71, L77 |
| Part 4.2, Phase 3, "Option C: Cooperative Membership" | A settlement path with membership dues that confers governance rights. It conflicts with [§14.6][v10-14.6] ("the only tests of membership"), KRS 273.187(1) and the proposed §14.9 bar. It must be struck from v2.0 too | Canvas F0AFYMXLCJU part 4.2; v1.0 L337 |
| 7.1–7.2 (CLA personal data; public CLA-status list) | The privacy floor, [§2.4][v10-2.4] | v1.0 L47 |
| "Executive Director" (Document Control, parts 4 and 8) | No such office. The offices are listed in [§8.1][v10-8.1] | v1.0 L167 |
| Header "Related Policies: P1-001 (Mission & Values), P1-003 (Bylaws)" | Both labels are wrong. P1-001 is the bylaws. P1-003 was used for other policies, never the bylaws | bylaws README L3 |

### The CLA text already went out

**The answer.** The CLA's assignment clause was embedded in volunteer onboarding papers. Whether any copyright moved is an open question for counsel. A registry entry should release anything that may have moved.

- **What went out.** A Slack search for "hereby assign to NTARI" returns at least 20 files, mostly volunteer welcome letters and Volunteer Registration canvases from 2026-02 onward. A September 2026 welcome-letter canvas embeds CLA clauses 1–8 verbatim.
- **The acknowledgment.** The volunteer's signature line acknowledges unpaid volunteer status and says they have read the letter.
- **Mixed signals.** In at least one onboarding exchange, a volunteer was told no signed copy needed to be returned. But the volunteer exit-letter template presumes a signed CLA (`volunteer-exit-letter.md` L39).
- **The law.** A transfer needs a signed writing ([§204(a)](https://www.law.cornell.edu/uscode/text/17/204)). Secondary summaries of a 2013 Fourth Circuit case report that electronic assent can satisfy it; the opinion itself was not read.
- **Not checked.** Whether the Slack registration workflow captures any assent, and whether any volunteer returned a signed acknowledgment.

### Why DCO is deliberate

**The answer.** Spreading copyright across contributors makes it hard for anyone, NTARI included, to take the work out of copyleft. That is the President's stated reason, and it is the property the bylaws already protect.

- **Relicensing** a work needs the consent of every copyright holder in it.
- **Under assignment,** one owner holds everything. Only a promise stands between the commons and a relicense.
- **Under DCO,** no one holds the whole, so no one can close it alone. DCO 1.1 certifies the right to submit "under the open source license indicated in the file" ([developercertificate.org](https://developercertificate.org/)). It transfers nothing.
- **The bylaws already point this way.** §9.4 bars any agreement that would let NTARI close what is open.

The friction cuts both ways, and that is the point. Entry 9 moves NTARI's own text in governance-rand to AGPL-3.0, but the merged Phase 1 report (governance-rand PR #2) stays GPL-3.0 unless its author agrees otherwise.

### The enforcement trade-off

**The answer.** Under DCO, NTARI can sue only over the lines it owns. Every other holder enforces their own lines, alone or by authorizing NTARI or a partner to act for them. NTARI should accept this cost and make cooperation easy.

- **Who can sue.** Only the owner of an exclusive right ([§501(b)](https://www.law.cornell.edu/uscode/text/17/501)). An exclusive license counts as a transfer of ownership; a non-exclusive one does not ([§101](https://www.law.cornell.edu/uscode/text/17/101)). So an enforcement authorization that transfers nothing lets an agent investigate, send notices and negotiate. A lawsuit still needs the owner as a party.
- **Registration.** US works must be registered before suit (§411(a)), and statutory damages and fees need timely registration (§412). P2-004's "$150,000 per work" is the statutory maximum for willful infringement (§504(c)(2)).
- **What NTARI owns.** Work by employees within their job, and work assigned in a signed writing; a contract alone cannot make software "for hire" (§101). No employment record or officer assignment was found, so whether NTARI owns even its officers' commits, the President's included, is unverified.
- **AI-generated material.** Material without human authorship is not protected ([US Copyright Office, Part 2, 2025-01-29](https://www.copyright.gov/ai/Copyright-and-Artificial-Intelligence-Part-2-Copyrightability-Report.pdf)). Recording tool co-authorship in commits keeps clear which work is a person's own.
- **Precedent.** In Germany, Hellwig v. VMware ended at the Hamburg appeal court in February 2019; the developer did not appeal further ([SFC](https://sfconservancy.org/news/2019/apr/02/vmware-no-appeal/)). In SFC v. Vizio, SFC argues as a purchaser under contract law, not as a copyright owner. A December 2025 tentative ruling favored SFC, a later December order went the other way on part of the case, and trial is listed for late 2026 ([SFC case page](https://sfconservancy.org/vizio/)). That theory is unsettled and no policy foundation.
- **A gap to close.** The covenant binds what NTARI holds. Under DCO alone, code an officer holds personally falls outside it, because §9.4 and §13.2 bind "the Institute", not individual authors. Where one officer wrote nearly every line, that officer could license their own lines on any terms. Two things close the gap: option 3 below, or a short personal covenant signed by the officer. Past AGPL releases stay licensed either way.

### Options

**The answer.** Option 2 is recommended: DCO, plus enforcement authorizations that contributors may choose to give.

| Option | What it is | For | Against |
|---|---|---|---|
| 1. DCO only | Inbound = outbound, no assignment, no enforcement paperwork | Matches practice exactly; maximum friction; no personal data held | Coordinated enforcement depends on ad hoc cooperation |
| **2. Option 1 plus optional enforcement authorizations (recommended)** | A contributor may appoint NTARI and a named partner as agent to monitor, send notices and negotiate compliance. A suit needs separate consent. No copyright moves | Keeps the friction; lets NTARI coordinate notices across holders; fits §9.4 and the SFC partnership P2-004 already plans | The agent cannot sue alone; coverage is partial |
| 3. Option 1 or 2 plus officers' own work | Officers who are not employees may voluntarily assign their own NTARI work to NTARI in a signed writing, recorded in the registry. Contributors are never asked | Gives NTARI lines it can register and enforce; brings officer-held code under the covenant | In single-author repos NTARI becomes the near-sole holder, so the covenant is the only guard there. Needs a §14.3 disclosure |
| 4. Optional fiduciary assignment | NTARI offers, never requires, an assignment with a license back | Centralizes enforcement for those who opt in | Rebuilds a center; arguably the agreement §9.4 forbids. Not recommended |
| 5. Keep the CLA | Collect signed CLAs as P2-004 v1.0 says | Unified ownership | Contradicts the President's direction, §9.4, all 27 rulesets and the published CONTRIBUTING texts. Rejected |
| 6. Rely on users' contract rights | Treat users as third-party beneficiaries (the Vizio theory) | Needs no ownership | Unsettled. Supplementary argument at most |

Whether to add option 3, a personal officer covenant, or neither is a question for the federation.

### Replacement text for P2-004 part 3

This is draft text for P2-004 v2.0, which the Board would ratify. It replaces parts 3.1–3.4, 7 and the CLA items in part 10. Bracketed choices follow the decisions above.

```markdown
## 3. COPYRIGHT, CONTRIBUTIONS AND THE COMMONS COVENANT

Replaces parts 3.1–3.4 of version 1.0. Implements bylaws §9.4 and §13.2.
Where this part and the bylaws differ, the bylaws control.

### 3.1 Copyright stays with its authors

NTARI takes no assignment of copyright in contributions and asks for none.
Each contributor keeps the copyright in their own contribution. NTARI holds
copyright only in work it owns by law: work its employees make within the
scope of their employment[, and work its own officers or staff choose to
assign to it, in a signed writing, for work done on its behalf; each such
assignment is recorded in the governance registry with a §14.3 disclosure].

The spread of copyright across many holders is deliberate. Because no single
party holds the whole, no single party, NTARI included, can take the work out
of copyleft without the consent of every holder whose work it contains.

### 3.2 Contribution terms: inbound = outbound, certified by sign-off

(a) Inbound = outbound. A contribution is licensed by its author under the
    license of the file or repository it enters, or under a compatible
    license indicated in the file. For software and documents alike
    that is AGPL-3.0 [or any later version], as bylaws §9.4 and part 2
    give it. There is no separate contributor agreement.
(b) Sign-off. Every commit carries a Signed-off-by trailer certifying the
    Developer Certificate of Origin 1.1. The name in the trailer matches
    the commit author.
(c) No bypass. Every NTARI repository requires the sign-off with a check
    that can fail a merge to the default branch, and no one may bypass it,
    NTARI's own accounts included (governance registry Entry 4).
(d) No contributor database. NTARI requires no CLA and keeps no register of
    contributors' legal names, postal addresses or employers. Provenance
    lives in the repository history (bylaws §2.4).
(e) Patents. Each contributor grants the patent license that comes with
    AGPL-3.0 (section 11). NTARI asks for no other patent grant.
(f) Human authorship. Material a person did not write, such as tool output,
    is identified in the commit, for example with a Co-authored-by trailer
    naming the tool.

### 3.3 The commons covenant

These commitments cover the copyright NTARI holds and NTARI's own conduct.
Items 1 to 3 restate bylaws §9.4 as amended by registry Entry [n] and
change only by amendment under Article XV. Items 4 and 5 are Board policy
until the bylaws carry them.
No act of NTARI may impair a license already granted (bylaws §13.2).

1. Never closed; only ever stronger. NTARI licenses every work in which it
   holds copyright under the license bylaws §9.4 gives it, and never under
   proprietary terms. It moves such a work only to a stronger copyleft
   named under §9.4, never to a weaker one.
2. No exceptions for sale. NTARI does not dual-license, does not sell or
   grant exceptions to its copyleft terms, and does not settle an
   enforcement matter on terms that let a covered work stay closed.
3. No center. NTARI asks no contributor for an assignment or for any
   license broader than inbound = outbound. It signs no agreement, with a
   contributor, funder, partner or vendor, that would let any party, NTARI
   included, close what is open.
4. Mission use. NTARI uses the copyright it holds only to keep the work free
   and to enforce its copyleft terms, in service of bylaws §1.4.
5. Succession. If NTARI dissolves, the copyrights it holds pass,
   consistent with the articles of incorporation and the authorities
   bylaws §1.2 names (bylaws §13.3), to a successor exempt under section
   501(c)(3); NTARI asks the successor to accept this covenant.
   Contributors' own copyrights stay theirs.

### 3.4 Credit, not seats

(a) Credit. Every merged contribution is credited from the repository
    history. A repository may publish a CONTRIBUTORS file generated from it,
    using the names or handles contributors chose in their commits, never
    email or postal addresses.
(b) No governance weight from contribution. Lines of code earn no vote,
    seat or weight. Governance standing comes only from membership under
    bylaws Articles III to VI. Contributors who are not members keep the
    voice everyone has, in pull requests, public channels and bylaws §4.1.
(c) Holders decide on their own work. Only a copyright holder can sue over
    their work. NTARI consults the holders of the affected lines before any
    enforcement step beyond a first notice, and acts for a holder only with
    that holder's written authorization under part 7.
```

For part 7, two texts replace the CLA template. The first is a licensing section for every CONTRIBUTING file:

```markdown
## Licensing: inbound = outbound, no CLA

- Sign off every commit: `git commit -s`. The Signed-off-by trailer
  certifies the Developer Certificate of Origin 1.1 and must match the
  commit author. A required check enforces it; there is no bypass.
- Your contribution is licensed under this repository's license (see
  LICENSE), or a compatible license indicated in the file. There is no
  contributor agreement to sign.
- Your copyright stays with you. NTARI takes no assignment. Because
  copyright is spread across contributors, no single party, NTARI included,
  can take this work out of copyleft without the consent of every holder
  whose work it contains. No act of NTARI can withdraw a license already
  granted.
- NTARI's own commitments are in Policy P2-004 part 3.3 and bylaws §9.4.
- If a tool generated part of your change, say so in the commit.
```

The second is an optional copyleft enforcement authorization. It transfers no copyright. Counsel should draft the final wording. The points it must carry:

1. The holder keeps their copyright; nothing assigns it or grants an exclusive license.
2. The holder appoints NTARI, named exactly as on its Kentucky filing, and any partner NTARI names in writing, as agent to monitor, investigate, send notices of violation in the holder's name and negotiate compliance.
3. Any resolution must bring the violator into compliance. No one may grant, for the holder, an exception that lets a covered work stay closed.
4. A lawsuit in the holder's name needs the holder's separate written consent for that matter.
5. The holder may end the authorization for the future by written notice.
6. The registry records the authorization by reference only, without personal details.

### Other edits P2-004 needs for v2.0

- **Header.** Add a real effective date. Fix both "Related Policies" labels. Replace "Executive Director" with an office from §8.1.
- **Parts 2.1–2.3.** Already amended by registry Entry 9 (AGPL-3.0 for everything). The new part 2 below writes that amendment into the policy text, and withdraws the alternative-license criteria, the CC BY-SA 4.0 for documentation and the CC BY 4.0 for policies.
- **Part 4.2.** Strike Phase 3 "Option C" and any settlement that gives governance rights. Phase 4 suits are brought by or with the holders of the lines. Note registration under §411–§412.
- **Two open canvas comments.** Close both threads on canvas F0AFYMXLCJU. One proposes defining "more permissive copyleft" as a Board-approved license that keeps reciprocal source duties; v2.0 answers it, since only the membership may name a successor, and only a stronger one (part 2.4). The other proposes replacing "3 years from discovery" with "applicable statutes of limitation"; adopt it in part 4.2.
- **Part 5.** Run the enforcement partnership through part 7 authorizations.
- **Elsewhere.** Replace the Community Advisory Board with the Federation Channels and holder consultation.
- **Part 10.** Replace "Implement CLA requirement" with "DCO required (in place on all 27 repositories)". Drop the CLA database. Add: confirm what NTARI owns, and register key releases.
- **Onboarding papers.** Replace the CLA text in the volunteer welcome letter and registration canvases with the CONTRIBUTING licensing section. Rewrite the exit-letter template.
- **Contributor files.** Janus and bylaws already have a "Sign-off (DCO)" section ([Janus CONTRIBUTING L22][j-contrib]), and developer-portal has a licensing clause. These need amending, not creating.
- **Two repo statements.** SoHoLINK and LBTAS say no party can relicense "without unanimous consent". That statement needs qualifying for the "or any later version" grant.

### How it gets adopted

- **Who.** P2-004 is a Board policy. The founder board, acting as the Board under §7.4 and proposed §16.4, ratifies v2.0. It does so in a meeting on one week's notice or by consent signed by every director, recorded in the registry.
- **The bylaws part.** The §9.4 floor is a bylaws change, adopted by §16.1 bootstrap act with the rest of the new text.
- **Counsel review.** P2-001 requires it only for Priority 1 documents, but it is prudent here (see the counsel questions).
- **The volunteer letters.** The ratifying act should come with a registry entry disposing of the CLA text already sent to volunteers.

## What license for documents

**The answer.** Decided: AGPL-3.0 for every work the Institute publishes, documents and code alike, until a stronger copyleft appears. The President decided this on 2026-11-13, after reading this note's first version, which recommended CC BY-SA 4.0 for documents. Governance registry Entry 9 records the decision as a Board act amending P2-004 Part 2.

- **What it covers.** The bylaws, every policy, the governance registry, research, technical documentation, course material, website text, translations and data, and the PDFs, slides and prints made from them.
- **The exception.** The JFA official document keeps the CC BY-SA 4.0 its footer states until an amendment under §9.2 changes it ([Question 1](#questions-for-federation-governance)).
- **What this section records.** What AGPL means for a document, the costs the decision accepts, and the research behind the first recommendation.

### What AGPL means for a document

**The answer.** AGPL treats a document exactly as it treats code. The Markdown file is the source, and every rendered or printed copy is object code.

- **It covers any work.** AGPL defines "the Program" as "any copyrightable work licensed under this License" (AGPL §0). The FSF says the GPL family fits any work with a clear source form ([GPL FAQ](https://www.gnu.org/licenses/gpl-faq.html#GPLOtherThanSoftware)).
- **The editable file is the source.** Source code is "the preferred form of the work for making modifications to it", and object code is "any non-source form of a work" (§1). A rendered web page, a PDF and a print are object code.
- **Copies carry the source.** A copy in object form must come with the source, or with a written offer of it for a print (§6(b)), or with clear directions to a server that holds it (§6(d)). CC BY-SA never required this; it is the reason to choose AGPL for prose.
- **Copies carry the license.** Every copy must carry the license text itself; the FSF says a URL is not enough (§4; [GPL FAQ](https://www.gnu.org/licenses/gpl-faq.html#WhyMustIInclude)).
- **The network clause rarely applies.** §13 covers modified programs people interact with over a network. It does nothing for a static page, and it matters for documentation sites with server code, such as agrinet-docs ([GPL FAQ](https://www.gnu.org/licenses/gpl-faq.html#AGPLv3InteractingRemotely)).
- **No boundary to police.** Code samples in specifications, conformance suites that bind specification text by anchor phrase, and documentation sites that mix prose and code no longer sit across two licenses.

### Costs the decision accepts

**The answer.** The first version of this note recommended CC BY-SA 4.0 for documents because of these costs. Entry 9 accepts them.

1. **Every copy carries the whole license.** Every PDF, handout, slide deck and social post with more than a fair-use excerpt needs about 34 KB of license text. CC BY-SA accepts a link (CC BY-SA 4.0 §3(a)(1)(C)).
2. **Locked copies are not barred.** CC BY-SA bars technological measures that restrict the licensed rights (§2(a)(5)(C), §3(b)(3)). AGPL waives anti-circumvention claims (§3) and requires the source, but does not bar a DRM-locked copy.
3. **Database rights are uncertain.** CC BY-SA 4.0 expressly licenses EU database rights (§4). Whether AGPL reaches them is uncertain.
4. **A wall between NTARI and the free-culture commons.** AGPL text cannot go into CC BY-SA projects such as Wikipedia, whose terms require CC BY-SA-compatible imports ([Terms of Use](https://foundation.wikimedia.org/wiki/Policy:Terms_of_Use)). CC BY-SA images, such as those on Wikimedia Commons, cannot go into AGPL PDFs or slides; they can be linked. Creative Commons calls its route from CC BY-SA into GPLv3 "not for general use" ([CC wiki](https://wiki.creativecommons.org/wiki/ShareAlike_compatibility:_GPLv3)). The Digital Public Goods standard requires a Creative Commons license for content collections ([DPG Standard, indicator 2](https://github.com/DPGAlliance/DPG-Standard/blob/main/standard.md)).
5. **The FSF's own advice differs.** For documentation it recommends the GFDL for large works and a permissive license for short ones; for works not made for a software project, a suitable copyleft, naming CC BY-SA as the fallback ([FSF recommendations](https://www.gnu.org/licenses/license-recommendations.html)).
6. **Funders.** A funder's open-access rule may require CC BY 4.0. Secondary sources report this for the Gates Foundation's 2025 policy; its own page was not checked. Entry 9 rules such terms out.

### The licenses compared

**The answer.** AGPL-3.0 is the only license on the list that both is copyleft and requires the editable source with every copy. That is why it serves for documents as well as code. This table is the research record behind both versions of this note.

| License | Copyleft? | Editable source required? | License notice | DRM | Database rights | Works with | Status for NTARI |
|---|---|---|---|---|---|---|---|
| **AGPL-3.0** | Yes, strongest for software | Yes: preferred form; a written offer for print (§6(b)(2)) or a pointer (§6(d)) | Full license copy (§4) | Not barred; circumvention claims waived (§3) | Uncertain | Combines with GPL-3.0 (§13); nothing goes out to CC BY-SA | **Adopted for all works (Entry 9)** |
| CC BY-SA 4.0 | Yes, share-alike | No | Link is enough | Barred | Expressly licensed (§4) | One-way into GPLv3 (declared 2015-10-08); Free Art License 1.3; Wikipedia | Kept only for the JFA specification and for versions already published |
| GPL-3.0 | Yes | Yes, as AGPL | Full license copy | As AGPL | Uncertain | The only license CC BY-SA 4.0 flows into (version 3 only) | No gain over AGPL. GovOS and governance-rand move to AGPL |
| GFDL 1.3 | Yes, but allows unchangeable sections | Only beyond 100 opaque copies (§3) | Full license copy | — | — | Incompatible with the GPL family and CC BY-SA | No |
| CC BY 4.0 | No (permissive) | No | Link | — | — | Flows into all GPL versions | No: anyone may close it. P2-004 v1.0 used it for policies; Entry 9 withdrew it |
| Free Art License 1.3 | Yes | Only a pointer to originals (§2.2) | — | — | — | CC BY-SA 4.0 | No: the FSF says not to use it for software or documentation |
| ODbL 1.0 | Yes, for databases | Database or change file on public use (§4.6) | — | — | Yes | GPL-incompatible per the FSF | Only for data derived from ODbL sources, which keeps its license |

Sources: [AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0.txt), [CC BY-SA 4.0 legal code](https://creativecommons.org/licenses/by-sa/4.0/legalcode.en), [CC compatible licenses](https://creativecommons.org/share-your-work/licensing-considerations/compatible-licenses/), [FSF license list](https://www.gnu.org/licenses/license-list.html), [GFDL 1.3](https://www.gnu.org/licenses/fdl-1.3.txt), [Open Definition licenses](https://opendefinition.org/licenses/).

### Compatibility facts

**The answer.** Under Entry 9, outside material enters an NTARI work only if its license lets the combined work be conveyed under AGPL-3.0. Anything else is cited or linked.

- **AGPL and GPL.** AGPL-3.0 and GPL-3.0 parts may be combined into one work, and each part keeps its own license (AGPL §13; [GPL FAQ](https://www.gnu.org/licenses/gpl-faq.html#AGPLGPL)). That is how the governance-rand#2 report, which stays GPL-3.0, sits in an AGPL repository.
- **CC BY-SA material.** CC BY-SA 4.0 material can go into GPLv3 works one way only (declared 2015-10-08), but Creative Commons calls that route not for general use. No CC or FSF statement covers a route onward into AGPL. So CC BY-SA text and images are cited or linked, not copied into AGPL documents.
- **Permissive material.** Material under licenses such as CC BY, MIT or Apache 2.0 can generally be included, keeping its notice.
- **OSI approval.** AGPL-3.0 is OSI-approved, so documents now also meet P2-003's "OSI-approved license" wording.
- **The DCO wording.** DCO 1.1 refers to the license indicated in the file, yet most NTARI Markdown files indicate none. A one-line SPDX notice or footer on each new file meets that wording.

### Grants already made stand

No act may impair a license already granted ([§13.2][v10-13.2]). Every version already published keeps its license. Entry 9 applies to versions published afterwards.

- **The CC BY-SA repositories.** Versions of the bylaws, Policies, the four *-rand repositories and the five seeds published before they are relicensed stay available under CC BY-SA 4.0 too. Their new notices should say so.
- **Bylaws v1.0.** It was published under AGPL-3.0 on 2026-09-02 (commit `4246602`) and relicensed to CC BY-SA 4.0 on 2026-10-08 (PR #1), so it is already available under both. The README's statement that AGPL "does not apply here" ([L101-105][readme-101]) should be annotated, not rewritten.
- **Policies.** Policies published under P2-004 v1.0's CC BY 4.0 keep it for those versions.
- **governance-rand.** NTARI relicenses its own text to AGPL-3.0. The merged report in PR #2 stays GPL-3.0 unless its author agrees otherwise. This note is AGPL-3.0 under Entry 9.
- **Repositories already declared "AGPL-3.0" with no version grant.** Janus's README, agrinet-docs and developer-portal need no change. Counsel's view is needed only before NTARI writes "-or-later" on outside contributors' work there.

### Or later, or only

**The answer.** Still open. Until the federation decides, notices written under Entry 9 name version 3 only, because NTARI can later widen its own works to "or any later version" but can never narrow a grant once made.

**For "or later":**

- Code search finds "AGPL-3.0-or-later" 84 times across six NTARI repositories and "AGPL-3.0-only" nowhere.
- The v1.1 draft §9.4 says it ([v1.1 L197][v11-9.4]), and so does the JFA spec ([L15][j-15]).
- A later FSF AGPL can be used without anyone's consent, which fits "until a stronger copyleft appears".
- A stricter later version would not restrict use of the current one ([GPL FAQ](https://www.gnu.org/licenses/gpl-faq.html#VersionThreeOrLater)).

**Against "or later":** the FSF, not NTARI's members, judges what "later" means. AGPL §14 promises only that later versions will be "similar in spirit".

**The alternative.** Use "only" and name a proxy under AGPL §14: the Institute, or its successor steward under §13.3. That keeps the judgment with the membership and survives the Institute. The cost: the 84 existing "or later" notices stay as they are, since grants already made cannot be narrowed.

### Replacement text for P2-004 part 2

Draft text for P2-004 v2.0. It writes Entry 9 into the policy and replaces parts 2.1–2.3 of version 1.0.

```markdown
## 2. LICENSING FRAMEWORK

Replaces parts 2.1–2.3 of version 1.0, as amended by governance registry
Entry 9 (2026-11-13). Implements bylaws §9.4; where they differ, the
bylaws control.

### 2.1 One license: AGPL-3.0

(a) Every work the Institute publishes is licensed under the GNU Affero
    General Public License, version 3 [or any later version | only] (SPDX
    AGPL-3.0[-or-later | -only]). This covers software, conformance suites,
    build and publishing scripts, website and documentation-site code, and
    every document: the bylaws, every policy, the governance registry,
    research, technical documentation, course material, website text,
    translations, data, and the PDFs, slides and prints made from them.
(b) The JFA official document keeps the license its own text states. It
    changes only by amendment under bylaws §9.2.
(c) No project, office or Board resolution may license Institute work on
    other terms. The alternative-license criteria of version 1.0 are
    withdrawn.

### 2.2 Source and license with every copy

(a) The editable source of every Institute work (for documents: Markdown,
    LaTeX, AsciiDoc or OpenDocument) is committed to a public NTARI-RAND
    repository before the work is published anywhere else. A draft made
    in a website builder, design service or chat canvas is exported to an
    open format and committed first.
(b) Every published copy carries its title, version and license name, a
    link to its source, and a copy of the license text (AGPL sections 4
    and 6). A print or slide deck meets the source duty with a written
    offer or clear directions to the repository (AGPL section 6(b), 6(d)).
(c) A translation names the version it translates and states that the
    English text controls.

### 2.3 Until a stronger copyleft appears

(a) A successor qualifies only if the Free Software Foundation lists it as
    free; it keeps every freedom and obligation of AGPL-3.0 (source with
    non-source copies, section 6; the source offer to network users,
    section 13; installation information, section 6; the patent license,
    section 11; the anti-circumvention waiver, section 3; the bar on
    further restrictions, sections 7 and 10); and it extends at least one
    of those obligations, for example by barring technological measures
    that restrict the licensed rights. For software it must also be
    approved by the Open Source Initiative.
(b) The membership decides by amending bylaws §9.4 under Article XV;
    during bootstrap, the founder board under §16.1. The decision is
    recorded in the governance registry and stays open under bylaws §2.3.
(c) The Institute moves works whose copyright it holds in full. Other
    contributors' work moves only as its license allows or with each
    holder's written consent. This friction is deliberate and binds the
    Institute too.

### 2.4 Grants already made stand

Nothing here impairs a license already granted (bylaws §13.2). Every version
published before this part took effect keeps the license it carried.

### 2.5 Others' material

Material from others keeps its own license and is marked. It is incorporated
only where its license allows the combined work to be conveyed under
AGPL-3.0; otherwise it is cited or linked. Work the Institute contributes to
another project follows that project's license.
```

### Carrying it out

**The answer.** Entry 9 is in force now, so the relicensing need not wait for the bylaws act ([Sequence](#sequence) step 6).

- **Eleven CC BY-SA 4.0 repositories to AGPL-3.0:** bylaws, Policies, covenant-rand, economy-information-rand, record-rand, substrate-rand, childcare-trust-network, lighthouse, shanina, shelter and world-chase-tag. Only the NTARI account appears among their contributors.
- **Two GPL-3.0 repositories to AGPL-3.0:** GovOS and governance-rand. The governance-rand#2 report keeps its GPL-3.0 notice and a copy of that license.
- **Notices.** Each README, in every language it is translated into, names AGPL-3.0, says the English text controls, and says earlier versions stay available under their old license. Files with no license line get an SPDX header or footer.
- **Copies elsewhere.** The P2-004 canvas and web post, ntari.org document footers, and PDFs, which must now carry the license text.

## Recommendation

**The answer.** Adopt all three findings, after the federation has tested this note.

1. **Placement.** Put every policy into the bylaws through Schedule P, filed by the bylaws section it serves, with full texts in pinned files. Put only floors and checks in the bylaws text. The founder board adopts the eleven bylaws changes by one §16.1 bootstrap act, ideally inside the v1.1 adoption. The Secretary then opens Schedule P by a registry entry.
2. **P2-004 part 3.** The founder board, acting as the Board under §7.4, ratifies P2-004 v2.0 with the replacement parts 2 and 3: DCO with no bypass, no assignment, no CLA, no governance weight from contribution, and optional enforcement authorizations (option 2).
3. **Documents.** Decided by registry Entry 9: AGPL-3.0 for documents and code alike. Write it into §9.4 with the rest of the new text, carry out the relicensing in [Sequence](#sequence) step 6 now, and adopt the source-and-license rule of the new P2-004 part 2.2.

Follow the [sequence](#sequence). Bootstrap acts stay open under §2.3, so later answers from counsel can still change them.

### Questions for counsel, before adoption

1. Is a Board-kept code of the bylaws (Schedule P) valid under KRS 273.161(6) and 273.191 while the text stays member-only? Can officers and federations issue binding procedures within it? If not, is the fallback under [What this design does not settle](#what-this-design-does-not-settle) sound?
2. What did the CLA text in volunteer letters do, and what form should a release take?
3. Does NTARI own code its officers wrote, the President's included?
4. Do Entries 3–8 meet KRS 273.375 or 273.377? Which test applies to a bootstrap act? Do post-bootstrap asynchronous ballots meet KRS 273.377 and 273.195?
5. Does a director's message in a Slack channel count as a signed written consent? P1-003, P2-004 and the proposed continuous consents all rest on it.
6. What do the filed articles say about dissolution and members?
7. What wording should the optional enforcement authorization use?
8. Can NTARI write "-or-later" on repositories declared "AGPL-3.0" that hold outside contributions?
9. Once policies are part of the bylaws, must a significant change to one be reported as a change to governing documents on any IRS return NTARI files? Not checked; a question for counsel or the Treasurer.

## Questions for #federation-governance

The federation decides these, with no deadline.

1. Should the JFA specification follow Entry 9 to AGPL-3.0? That needs an amendment of the official document's footer under §9.2, and the conformance suite checks the licensing statement, so the suite changes with it.
2. Should NTARI's notices say AGPL-3.0 "or any later version", or "only" with a proxy the membership names? Until this is decided, notices written under Entry 9 name version 3 only.
3. Should Schedule P be a code of the bylaws the Board keeps, while the text stays member-only?
4. Should the delegates hold a power to set aside any Board policy, as the member check on the Board's Schedule P power?
5. Should the §6.9 deliberation procedure be a Board policy, which fits KRS 273.195(2), or a procedure the Governance federation owns?
6. Must a federation vote before a pull request merges into an NTARI-RAND repository? The inventory reported that Voting Workflows requires one and the R&D Submission Guide does not (neither re-read here).
7. Should a pre-v1.0 policy left unratified at the end of bootstrap become superseded (proposed), or lapse after a fixed period?
8. Should the repository security defaults (Entries 6–7) be a Board policy the Board can loosen, or bylaws text only members can change?
9. Who should write the v1.1 §16.2 "internal policy" that decides when bootstrap ends?
10. Do you agree with the collision rule, and with refusing the 2026-03-18 proposal to renumber P3-004 to P3-009?
11. Should a single director's approval of a conflicted transaction be barred outright, going beyond KRS 273.219's safe harbor?
12. Should "the English text controls", a new rule, enter the bylaws text?
13. Should P2-004's line-count seats become a credit record with no governance right, and its "Option C" settlement be struck?
14. For code officers hold personally, should NTARI add officer assignments (option 3), a personal officer covenant, or neither?
15. Should P2-003 be ratified with Gitee as a Tier 2 host, or with the original prohibition?
16. Should P2-002 be ratified with the seven-language standard, adding French and toki pona?
17. The delegates cannot carry a set-aside during bootstrap. Which check on Board policies works today: a recorded founder-board answer to any member's set-aside petition, or a lapse of bootstrap Board policies unless the first post-bootstrap Board reconfirms them?
18. If no disinterested majority of directors can be formed, should a conflicted matter wait (the proposed text), go to a members' decision, or rest on the director proving it fair (KRS 273.219(1)(b))?
19. How many directors sit on the founder board today, and which offices do they hold? The §14.3 disinterested majority and the KRS 273.375 consents depend on it.
20. Must Schedule P, the eleven changes and each ratified policy be translated into the P2-002 languages? Who translates, and at what cost?
21. Should §9.4 leave out logos and brand marks? AGPL-3.0 lets a licensor decline trademark rights (§7(e)), but it would license a logo's copyright.
22. Who drafts the conflict-of-interest policy ([Sequence](#sequence) step 8(b)), and from what model? No draft exists.
23. Once the canonical texts are committed, should each Slack canvas and ntari.org copy carry a banner naming the pinned commit?

## Method and ethics

Claude (Anthropic) did this research at the direction of the author. Fifteen agents ran it, each with a narrow task, followed by a revision pass:

- **Two inventory sweeps and a reconciler.** They searched GitHub, Slack, Confluence, ntari.org and the local document store, and merged the results into one inventory of 61 entries: 52 numbered and 9 unnumbered.
- **A bylaws and Kentucky-law map** of bylaws v1.0 and v1.1 at `3276781` and 27 sections of KRS Chapter 273, read from the Kentucky Legislature's site.
- **License research** from primary license texts and FSF, Creative Commons and OSI pages.
- **P2-004 §3 research**: the canvas, the public post, GitHub rulesets and apps, contributor files, Slack records and US copyright law.
- **Three independent placement designs**, scored by a judge (8, 7 and 6 out of 10).
- **Three adversarial verifiers**, one per finding. Their own tallies, by category as each reported them (the categories do not always sum to the total):
  - placement: 72 claims checked; 39 confirmed, 17 corrected, 4 refuted, 10 unverifiable;
  - documents license: 64 checked; 46 confirmed, 12 corrected, 2 refuted, 6 unverifiable;
  - P2-004 §3: 52 checked; 28 confirmed, 18 corrected, 2 refuted, 7 unverifiable.
- **A drafter and a critic.** The critic re-checked the line links and statutes and listed 24 issues.

Every refuted claim is removed and every correction applied; unverifiable claims are marked or left out. The verification moved the documents-license recommendation from AGPL to CC BY-SA 4.0. After the note was filed, the President decided AGPL-3.0 for documents and code alike (registry Entry 9); a second revision records that decision and keeps the research as the record of the costs it accepts. The first revision pass applied the critic's issues, re-checked every bylaws line link against `3276781`, and re-ran the repository's suite on the exact bylaws text quoted here.

All work was read-only: nothing was posted, pushed, commented or edited anywhere, and tests ran on scratch copies. Quotes from third-party pages are short. The note contains no email addresses or personal data, names no founder board member and no contributor other than the author; consent questions cite pull requests.

Much of this text was drafted by a tool. The choices it recommends are the author's to propose and the federation's to test.

[v10-hdr]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L3-L5
[v10-1.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L19
[v10-1.5]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L33
[v10-2.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L43
[v10-2.3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L45
[v10-2.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L47
[v10-3.3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L69
[v10-3.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L71
[v10-3.7]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L77
[v10-5.6]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L117
[v10-6.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L131
[v10-6.5]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L133-L137
[v10-6.7]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L141
[v10-6.9]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L145
[v10-7.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L153
[v10-7.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L157
[v10-7.5]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L159
[v10-8.1]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L167
[v10-8.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L169
[v10-8.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L173
[v10-8.6]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L177
[v10-9.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L185
[v10-9.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L189
[v10-9.5]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L191
[v10-9.16]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L231
[v10-10.7]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L265
[v10-10.8]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L267
[v10-13.1]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L317
[v10-13.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L319
[v10-13.3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L321
[v10-14.3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L331
[v10-14.6]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L337
[v10-14.7]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L339
[v10-15.1]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L345
[v10-16.1]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L355
[v11-hdr]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L3-L5
[v11-8.3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L179
[v11-8.6]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L185
[v11-9.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L197
[v11-16.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L397-L401
[readme-53]: https://github.com/NTARI-RAND/bylaws/blob/3276781/README.md?plain=1#L53-L58
[readme-62]: https://github.com/NTARI-RAND/bylaws/blob/3276781/README.md?plain=1#L62-L63
[readme-101]: https://github.com/NTARI-RAND/bylaws/blob/3276781/README.md?plain=1#L101-L105
[contrib-9]: https://github.com/NTARI-RAND/bylaws/blob/3276781/CONTRIBUTING.md?plain=1#L9-L13
[contrib-22]: https://github.com/NTARI-RAND/bylaws/blob/3276781/CONTRIBUTING.md?plain=1#L22-L38
[p1005]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-005_Governance-Venue-Policy_v1.0.md?plain=1#L3-L5
[j-15]: https://github.com/NTARI-RAND/Janus/blob/9aa2332/janus-facing-architecture.md?plain=1#L15
[j-dispute]: https://github.com/NTARI-RAND/Janus/blob/9aa2332/jfa-dispute-mechanics.md?plain=1#L3
[j-p1004]: https://github.com/NTARI-RAND/Janus/blob/9aa2332/P1-004_Substrate-Constraints_v0.1.md?plain=1#L6
[j-contrib]: https://github.com/NTARI-RAND/Janus/blob/9aa2332/CONTRIBUTING.md?plain=1#L22

---

*Licensed under the [GNU Affero General Public License, version 3](https://www.gnu.org/licenses/agpl-3.0.txt) (AGPL-3.0), under governance registry Entry 9. This repository's LICENSE file still reads GPL-3.0 until it is relicensed under the same entry.*
