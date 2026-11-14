# Put every policy into the bylaws through one register, Schedule P

**Tier 1 research · Governance · Bylaws amendment proposal**
**Filed:** 2026-11-13 · **Author:** Jodson Graves
**Base:** NTARI-RAND/bylaws main at `3276781`, P1-001 v1.1 (draft) · registry at [NTARI-RAND/governance-registry][reg-repo]
**Builds on:** [governance-rand#4][gr4] · **Patch:** [`amend-schedule-p.v1.1.patch`](amend-schedule-p.v1.1.patch)

## Summary

**The answer.** Give every policy of the Institute one entry in a single register, Schedule P, filed under the bylaws section it serves. Schedule P is part of the bylaws, but it is not their text. The membership alone still amends the text. The Board, offices and federations keep Schedule P, under checks the text sets.

- **What changes.** Four provisions of the v1.1 draft are amended: §7.5, §8.4, §9.5 and §15.1. Four are added: §14.8 (order of instruments), §14.9 (Schedule P), §14.10 (changing a policy) and §16.4 (transition). Two informative rows join the appendix. One new file joins the bylaws repository, `P1-001_Schedule-P_Register-of-Policies.md`. It is the register's draft opening, with a row for each of the 76 rows of the placement table in governance-rand#4.
- **Why.** Today the Institute's policies sit in Slack canvases, Confluence pages, ntari.org posts and local files. Several numbers name more than one document. Nothing says which policies bind, which rule wins in a conflict, or how a policy changes. Kentucky defines bylaws as any code of rules for a corporation's affairs, whatever it is called ([KRS 273.161(6)][krs-161]). It vests the power to amend them in the board "unless otherwise provided in the articles of incorporation or the bylaws" ([KRS 273.191][krs-191]). governance-rand#4 reads these two sections to allow a register that is part of the bylaws but changes by a lighter path than the text. No KRS 273 section expressly allows or forbids that, and the filed articles of incorporation, not yet retrieved, could say otherwise. Counsel question 1 asks.
- **The checks.** No entry may touch member rights, votes, quorum, notice, directors or reserved powers. Nothing binds unless its text is pinned where members can read it. The delegates may set aside any board policy, and any Board act that amends or revokes a procedure. Every act is recorded in the public governance registry.
- **What it leaves alone.** It does not touch §9.4, which sibling proposal A amends, or §7.4 and §14.3, which sibling proposal C amends.
- **It adopts nothing.** Merging this file into governance-rand adopts nothing. Adoption would be a bootstrap act of the founder board under §16.1. It would be folded into the pending v1.1 adoption, or made as a new version file, and recorded in the governance registry. Schedule P would then open by a registry entry of its own.
- **Changes from governance-rand#4's texts.** Besides adapting them to v1.1, this version closes gaps a review found. §9.5 records every act under §14.10 and §16.4. §14.8 keeps the invariant registry with the official document. §14.9 reads §5.6 and §6.9 as meaning the text, and limits its moving-branch rule to entries. §14.10's set-aside also reaches a Board act on a procedure. §16.4 says how acts already recorded enter Schedule P. Each change is stated under its Why.
- **Tested.** The patch applies to bylaws `3276781`, and the bylaws suite passes all checks B1–B8: 112 provisions, 367 section references, all resolving.

**Already decided, and not reopened here.** The President directed on 2026-11-13 that every policy goes into the bylaws, and that where they are placed matters most; governance-rand#4 recommends one register, Schedule P. AGPL-3.0 covers every work the Institute publishes, documents and code alike, until a stronger copyleft appears ([registry Entry 9][reg]). The Developer Certificate of Origin, in place of a contributor license agreement, is deliberate. The JFA specification keeps its CC BY-SA 4.0 footer for now.

## Terms

*The bylaws and how they change*

- **JFA.** The Janus Facing Architecture, the design the Institute stewards. Its specification is the official document (§1.5).
- **KRS.** Kentucky Revised Statutes. Chapter 273 governs nonprofit corporations such as NTARI.
- **Instrument.** A formal governing document: the articles of incorporation, the bylaws, the JFA official document.
- **Bylaws text.** The numbered provisions of P1-001, such as §9.5. Only the membership amends them.
- **Article XV.** The bylaws' amendment article. Under §15.1 the text changes only by a delegates' ballot in which every member of each federation may vote.
- **Federation.** The members of one layer of the architecture: Substrate, Record, Covenant, Governance, or Economy & Information (§5.3).
- **Delegate.** The director a federation elects. The delegate casts the federation's one vote as the federation decided it (§5.7).
- **Seat.** An office together with the federation that §7.2 binds it to. The Record seat is the Secretary and the Record federation.
- **Founder board; bootstrap.** Until federations elect their directors, a founder board of three to five directors serves as the Board and holds the membership's powers (§16.1). That period is bootstrap.
- **Bootstrap act.** An act the founder board takes with the membership's powers under §16.1. Each is recorded in the governance registry.
- **Board act.** An act of the Board under §7.4, in a meeting or by written consent. During bootstrap the founder board also acts as the Board; registry Entry 9 is recorded that way.
- **Governance registry.** The public, append-only record the Secretary keeps under §9.5. Since registry Entry 10 (2026-11-13), the record copy is the `main` branch of [NTARI-RAND/governance-registry][reg-repo].
- **#federation-governance.** The Institute's Slack channel where Governance research is deliberated, through testing, with no deadline.
- **Written consent.** A Board decision taken without a meeting. Kentucky's default is that every director signs it ([KRS 273.375][krs-375]).
- **Code of the bylaws.** Kentucky treats any code of rules for a corporation's affairs as bylaws, whatever its name ([KRS 273.161(6)][krs-161]). Schedule P is drafted as such a code. Whether Kentucky allows a Board-kept one is Counsel question 1.

*Schedule P*

- **Schedule P.** The register of policies proposed here. The Secretary keeps it as a separate file beside the bylaws. It holds one entry for each policy, filed under the bylaws section the policy serves.
- **Inventory; placement table.** governance-rand#4 first listed the Institute's policy documents in an inventory of 2026-11-13: 61 entries, 52 numbered and 9 unnumbered. It then gave each a place in its table "Where each policy goes", 76 rows in all. This register follows that table.
- **Entry; row; pointer row.** An entry is the row for one document. A pointer row only points to the section where a document is entered, so a reader of every section it serves can find it.
- **Class.** What kind of document an entry is: (a) cited instruments, (b) board policies, (c) office and federation procedures, (d) informative documents, (e) documents not in force. Only (b) and (c) can bind.
- **Board policy.** A rule the Board adopts within a bylaws section the entry names.
- **Procedure.** A rule an office or a federation issues within its own area.
- **Set-aside.** A decision of the delegates that a board policy, or a Board act amending or revoking a procedure, no longer binds.
- **Pinning; commit; digest.** Pinning is citing a text at a fixed point so it cannot change under the citation. A commit is one fixed, named state of a git repository. A digest is a short fingerprint of a text; any change to the text changes it.
- **Moving branch.** A branch such as `main` whose content changes over time. Citing it pins nothing.
- **Incorporation by reference.** One document makes another part of itself by naming it. The name must identify exactly which text is meant.
- **Ministerial.** Done because stated conditions are met, without discretion, as the Secretary recognizes members under §3.3.
- **Published notice.** A text the Institute has published to the public, such as the ntari.org Privacy Policy, kept in force by §16.4 until the Board acts on it.
- **Savings clause.** A transition rule saying which earlier acts and rules still stand when a new instrument takes effect.
- **Number collision; suffix.** A collision is one policy number used for more than one document. Each extra use takes a lowercase suffix, such as P2-004a.
- **Gen-1.** The 2025 Confluence policy numbering. Many gen-1 pages are lost.

*Licenses and tools*

- **AGPL-3.0.** The GNU Affero General Public License, version 3: a copyleft license, meaning copies and changed versions must carry the same freedoms. Entry 9 applies it to every work the Institute publishes, from 2026-11-13 forward. The JFA official document keeps CC BY-SA 4.0 until a §9.2 amendment, and work others contributed keeps its own license.
- **DCO.** The Developer Certificate of Origin: a `Signed-off-by` line on each commit, by which its author certifies the right to submit it. It transfers no copyright.
- **CLA.** A contributor license agreement: a contract a contributor signs before their work is accepted.
- **Slack canvas; Confluence.** Two hosted tools where many of the Institute's policies were drafted. A canvas is a document inside Slack; Confluence is a wiki. Neither gives a pinned, public text.
- **Patch.** A file that lists exact line changes. `git apply` makes them.
- **The suite.** `bylaws-conformance-suite.py`, the bylaws repository's own script. It checks structure (B1–B8), not meaning.

## The amendment

Every quoted text below is exact. "Current" is P1-001 v1.1 at `3276781`. "Proposed" is the same provision after the patch. The proposed texts are governance-rand#4's tested texts, which were written against v1.0 line numbers. Where v1.1 differs, the text is adapted, and the difference is stated. Where review found a gap in governance-rand#4's text, the text is changed, and the change is stated under its Why.

### §7.5 Reserved powers (first sentence)

**Current** ([v1.1 L167][v11-7.5]):

> **7.5 Reserved powers.** The Board may not amend these bylaws, amend the official document, expel any party, dispose of the Institute's stewardship of the official document or the conformance suite, or dissolve the Institute. Those powers belong to the membership alone. Where these bylaws give a matter to the delegates, a director casting their federation's decision under §5.7 acts as that federation's delegate and not as the Board; this section bars the Board from deciding such a matter on its own motion.

**Proposed:**

> **7.5 Reserved powers.** The Board may not amend these bylaws, other than Schedule P as §14.10 provides, amend the official document, expel any party, dispose of the Institute's stewardship of the official document or the conformance suite, or dissolve the Institute. Those powers belong to the membership alone. Where these bylaws give a matter to the delegates, a director casting their federation's decision under §5.7 acts as that federation's delegate and not as the Board; this section bars the Board from deciding such a matter on its own motion.

**Why.** §7.5 bars the Board from amending the bylaws. Schedule P is a code of the bylaws (§14.9), so without a carve-out the Board could not keep it. The carve-out is narrow. It reaches only Schedule P, and only as §14.10 provides. Everything else §7.5 reserves stays with the membership. Kentucky lets the bylaws decide who amends them ([KRS 273.191][krs-191]). Only the first sentence changes; v1.1's remainder is kept word for word.

### §8.4 Secretary (one clause)

**Current** ([v1.1 L181][v11-8.4]):

> **8.4 Secretary.** Elected by the Record Federation, the Secretariat keeps governance records, performs the ministerial recognition of members under §3.3, maintains the governance registry of §9.5, receives and records the publications of Article XI, and issues the notices these bylaws require.

**Proposed:**

> **8.4 Secretary.** Elected by the Record Federation, the Secretariat keeps governance records, performs the ministerial recognition of members under §3.3, maintains the governance registry of §9.5 and Schedule P under §14.9, receives and records the publications of Article XI, and issues the notices these bylaws require.

**Why.** It names the office that keeps Schedule P, as §8.4 already names it for the registry. Only the clause "maintains the governance registry of §9.5," changes, as governance-rand#4 proposed. The clause reads the same in v1.1 as in v1.0; v1.1 only adds a comma after "Record Federation".

### §9.5 The governance registry

**Current** ([v1.1 L199][v11-9.5]):

> **9.5 The governance registry.** The Secretary maintains a public, append-only governance registry recording: recognitions and lapses of membership, and the federation elections and changes of §3.9; the publications of Article XI; expulsions, readmissions, and re-entries under Article XII; and each amendment of the official document and of these bylaws. The registry honors §2.4.

**Proposed:**

> **9.5 The governance registry.** The Secretary maintains a public, append-only governance registry recording: recognitions and lapses of membership, and the federation elections and changes of §3.9; the publications of Article XI; expulsions, readmissions, and re-entries under Article XII; each amendment of the official document and of these bylaws; and each act under §14.10 or §16.4, with the vote, the signed consents, or the officer's recorded act by which it was taken. The registry honors §2.4.

**Why.**

- Today's list leaves out policy acts. Under §14.10 a Schedule P act takes effect only when it is recorded here, so the registry must record it.
- **Every act, not a list of verbs.** governance-rand#4's text listed acts that enter, amend, ratify, set aside or retire an entry. That left out issuing a procedure, the Board's authorizing or revoking one, the Secretary's annotations, and the opening entries of §16.4. This text names every act under §14.10 or §16.4.
- **The vote, the consents, or the officer's act.** An office issues a procedure "by a recorded act of the officer" (§14.10), and the Secretary's entries are an officer's acts too. Neither is a vote or a consent, so §9.5 names the officer's recorded act beside them. Recording how each act was taken lets any member check it.
- v1.1 added "and the federation elections and changes of §3.9", which v1.0 lacks. That clause is kept.
- The registry is now public in fact: Entry 10 published it in its own repository on 2026-11-13.

### §14.8 Order of instruments (new)

**Where:** a new provision after §14.7, at the end of Article XIV.

**Proposed:**

> **14.8 Order of instruments.** Where instruments conflict, the higher controls, in this order: law, including KRS Chapter 273 and the requirements of the Institute's federal recognition; the articles of incorporation; the official document, with its invariant registry, which §9.16 amends as part of it, and the twelve lines, which no amendment may override (§15.2); the text of these bylaws; the runnable conformance suite, apart from its invariant registry, and the dispute-mechanics design, as §1.5 binds them; the board policies of Schedule P; and the office and federation procedures of Schedule P. Within one rank the later controls the earlier. An entry of Schedule P that conflicts with a higher instrument is void to the extent of the conflict, and is otherwise read to serve Article II. A document's number and series are filing labels and decide neither its rank nor who may change it. The English text of every instrument controls; a translation is made for reach, not for interpretation.

**Why.**

- **One order for every conflict.** P2-001's hierarchy (its "Authority Hierarchy") leaves out the articles and the official document, and cites bylaws from 2025. Kentucky already makes the articles control an inconsistent bylaw, except on the number of directors, where a bylaw change controls unless the articles say otherwise ([KRS 273.247(4)][krs-247]). §14.8 ranks law first, so that exception holds.
- **The invariant registry sits with the official document,** because §9.16 makes every change to the registry an amendment of the official document ([v1.1 L239][v11-9.16]). §1.5 and §9.13 count the registry as part of the conformance suite. So the rank below the text names "the runnable conformance suite, apart from its invariant registry". governance-rand#4's text said "the executable conformance suite", which could be read to pull the registry down to that rank.
- **A rank the bylaws only imply.** The bylaws do not say outright that the suite and the dispute-mechanics design rank below the text. This states it. It is a proposal to confirm.
- **Labels are not rank.** A P1 number does not make a document stronger than a P2 number.
- **A new rule in the last sentence.** The bylaws README says translations "are provided for reach, not for interpretation, per NTARI Policy P2-002 §2.2" ([README L62-63][readme-62]). governance-rand#4 found no such rule in P2-002 §2.2, so the rule is stated here instead. Whether it belongs in the text is Question 10.

### §14.9 Schedule P (new)

**Where:** a new provision after §14.8.

**Proposed:**

> **14.9 Schedule P.** Every policy of the Institute, and every document filed in its policy series, has one place in Schedule P, the register of policies the Secretary keeps beside these bylaws in the Institute's public repository of them. Schedule P is a code of these bylaws kept under §14.10 rather than Article XV; it is not their text, and no entry restates or alters their text. Where these bylaws place a policy outside them (§5.6, §6.9), they mean outside their text. It is arranged by the Article and section of these bylaws that each entry serves, so that a reader of any Article finds there every policy on its subject; an entry that serves more than one section is placed once and pointed to from the others. Each entry states its number, title, version, the section it serves, its class, its owner and the office that keeps it, its status, the registry entry recording the act, and where its text is kept. The classes are:
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
> Only an entry of class (b) or (c) marked in force, or marked a published notice under §16.4, binds, and only for the version it names. An entry is marked in force only when its text is published where members can read it, at a fixed location that cannot change under it: a commit of a public repository of the Institute, or a registry entry carrying the text or its digest. In an entry of Schedule P, a reference to a moving branch, and a text held only in a proprietary venue, incorporates nothing (§5.6, §13.1). No entry may create or alter a class of membership or a member's rights, set a member's vote, quorum, or notice outside the limits §6.4 and §6.5 set, set the number, election, term, or removal of directors, exercise a power §7.5 reserves, or insert the Board as a gate §7.6 forbids; an entry that attempts any of these is void to that extent, and the matter is taken up under Article XV.

**Why.**

- **One place for every policy.** A reader of any Article finds every policy on its subject there. A reader of §9.4 finds P2-004, the DCO mechanics, Entry 9 and the AGPL papers together.
- **Part of the bylaws, not their text.** That is the reading of [KRS 273.161(6)][krs-161] this proposal relies on (Counsel question 1). It keeps the adopted text, its seven translations and the suite untouched when a policy changes.
- **"Outside these bylaws" means outside the text.** §5.6 says changing venues "never requires amendment of these bylaws", and §6.9 keeps the deliberation procedure "rather than in these bylaws". Once Schedule P is a code of the bylaws, those words would contradict it. A new sentence reads them as meaning the text. governance-rand#4's text lacked it.
- **Five classes; only two bind.** Research and drafts never bind by accident.
- **Nothing binds unless pinned.** Incorporation by reference needs an exact text. A commit, or a registry entry that carries the text or its digest, gives one. A moving branch or a proprietary venue does not (§5.6, §13.1). The rule is limited to entries of Schedule P, because §1.5 itself defines the official document and the dispute-mechanics design by links to the `main` branch of Janus. Read generally, it would empty those definitions. governance-rand#4's text lacked the limit.
- **Limits no entry may cross.** Member classes and rights, votes, quorum and notice, and directors stay in the member-amended text by design. [KRS 273.187(1)][krs-187] requires member classes, qualifications and rights in "the articles of incorporation or the bylaws", and [KRS 273.211][krs-211] does the same for the number, election, terms and removal of directors. Keeping these in the text keeps them valid even if counsel rejects Schedule P as a code of the bylaws. The reserved powers of §7.5 and the bar on new Board gates in §7.6 stay out of reach too.
- **Why "outside the limits".** The §6.9 deliberation procedure is a class (b) slot. It may set a voting window and a majority, but only within §6.4 and §6.5. By the inventory's reading of the Voting Workflows canvas (not re-read here), its seven-business-day window survives, since it gives at least §6.4's one week. So does its simple majority, read as a majority of votes cast (§6.5).
- **The three slots** in (b) are the ones v1.1 already calls for: the venue policy of §5.6, the deliberation procedure of §6.9 and the conflict-of-interest policy of §14.3. Naming the §14.3 policy here does not edit §14.3.

### §14.10 Changing a policy (new)

**Where:** a new provision after §14.9.

**Proposed:**

> **14.10 Changing a policy.** The Board enters, amends, ratifies, and retires board policies by action under §7.4. An office or federation issues, amends, and retires its procedures — an office by a recorded act of the officer, a federation by its internal majority under §6.5 — and never for its own powers or duties, which these bylaws and the Board set; a procedure that commits the Institute's funds or binds it to an outside party takes effect only when the Board also authorizes it under §7.4, and the Board may amend or revoke any procedure by the same action. The checks on a board policy, and on a Board act amending or revoking a procedure, are the recall of §6.8 and setting aside by the delegates: any member may propose that such a policy or act be set aside, and a set-aside noticed under §6.4 and carried as §6.5 provides is a decision of the membership, open under §2.3 and §6.7. The Secretary makes entries of classes (a), (d), and (e) of §14.9 ministerially, enters every proposed policy as a draft, and annotates an entry when its status changes; a refusal to make an entry states which requirement failed and is challengeable through Article XII, as under §3.3. Every act under this section takes effect when recorded in the governance registry under §9.5 with its text published as §14.9 requires; entries are corrected by annotation or a new version under §2.5, never rewritten or deleted, and remain open to the checks this section names. A number names one document and is never reissued; where a number was issued to more than one document, Schedule P records each use under a distinguishing suffix. Making or annotating an entry by these acts is not an amendment of the text of these bylaws.

**Why.**

- **Each class has one path.** The Board acts on board policies. Offices and federations act on their own procedures, never on their own powers or duties. Kentucky sets an officer's duties by the bylaws, by the Board, or "by direction of an officer authorized by the board of directors to prescribe the duties of other officers" ([KRS 273.228][krs-228]). That last route is why Board authorization is the fallback for class (c) procedures (see "What this proposal does not decide").
- **Money and outside parties need the Board.** A procedure that commits funds or binds an outside party needs Board authorization.
- **The set-aside is spelled out on purpose.** Reopening under §6.7 reaches only decisions of the membership (§2.3), and §6.5 is only a quorum-and-majority rule. Without this sentence a board policy would have no member check, which §2.2 forbids.
- **The set-aside also reaches a Board act on a procedure.** §14.10 lets the Board amend or revoke any procedure, and §2.2 says every power must name its check. governance-rand#4's text named a check for board policies only. Whether the power should reach a federation's own procedures at all is Question 17.
- **The Secretary's role is ministerial and challengeable,** as with recognition under §3.3. But Article XII has no procedure for this challenge yet. §12.5 lists five kinds of proceeding, each decided by ratings "of the offense", and a challenge to a refusal is not one of them. The same gap already exists for refusals under §3.3. This proposal does not fill it (Question 13).
- **Append-only, and open to the named checks.** Entries are corrected by annotation, never rewritten (§2.5). governance-rand#4's text said entries "remain open under §2.3", but §2.3 reaches only decisions of the membership. Entries made by the Board, an officer, a federation or the Secretary are not. So this text says they remain open to the checks §14.10 names.
- **One number, one document.** P2-001 bars reuse only for executive-action numbers. This adds the rule for P1, P2 and P3 numbers, as §9.16 already does for invariant identifiers.

### §15.1 By the membership alone

**Current** ([v1.1 L385][v11-15.1]):

> **15.1 By the membership alone.** These bylaws are amended only by a majority vote of the delegates, each federation having decided under §6.5 with every member of that federation holding the vote, prosumer members included, in a ballot noticed under §6.4 carrying the full text of the amendment.

**Proposed:**

> **15.1 By the membership alone.** These bylaws, other than Schedule P, are amended only by a majority vote of the delegates, each federation having decided under §6.5 with every member of that federation holding the vote, prosumer members included, in a ballot noticed under §6.4 carrying the full text of the amendment. Schedule P is kept under §14.10.

**Why.** Schedule P is a code of the bylaws, so without this change §15.1 would send every policy act to a delegates' ballot. The text stays member-only. §15.1 reads the same in v1.1 as in v1.0, so governance-rand#4's text applies unchanged.

### §16.4 Transition (new)

**Where:** a new provision after §16.3, following its second paragraph, at the end of Article XVI.

**Proposed:**

> **16.4 Transition.** Until bootstrap ends, the founder board serves as the Board for every act §14.10 gives the Board, and takes those acts under §7.4 as the Board, not in exercise of the membership's powers under §16.1, so that a later Board may revisit them. A policy approved before 2026-08-31, when version 1.0 of these bylaws took effect, or claimed as adopted with no record of the act, does not bind until the Board ratifies it, conformed to these bylaws, by an act recorded under §9.5; until then its entry is marked awaiting ratification. A notice the Institute has published to the public stays in effect as published until the Board confirms, replaces, or withdraws it; the Secretary commits a copy of it under §14.9 when making its entry, and that copy is the version the entry names. On opening Schedule P, the Secretary enters, each as an entry of its own, the acts recorded under §9.5 on or after 2026-08-31 that made or changed a policy, marked in force where the registry records them as valid; an earlier policy that such an act changed keeps its own status. A policy still awaiting ratification when bootstrap ends under §16.2 is marked superseded. Acts already taken in reliance on such a policy stand, open to the same checks as any other act of the body that took them.

**Why.**

- **The founder board acts as the Board here, not as the membership.** A rule adopted with the membership's powers under §16.1 could later be changed only by the membership. A board policy must stay changeable by a later Board. The sentence covers only the acts §14.10 gives the Board. governance-rand#4's text said "every act under §14.10", which would also have covered the delegates' set-aside, a decision of the membership. Who hears a set-aside during bootstrap is Question 3.
- **A savings clause v1.1 lacks.** v1.0's header supersedes only the v6.0–v8.0 bylaws ([v1.0 L3-5][v10-hdr]), and v1.1's header only keeps v1.0 in the record ([v1.1 L3-5][v11-hdr]). P2-004 (approved in Slack on 2026-02-15) and P1-003 (accepted 2026-04-21) both predate v1.0. A test by date catches them; a test by bylaws version might not.
- **Published notices stay in force.** The website Privacy Policy and Terms keep working while the pinning rule holds: their pinned version is the committed copy.
- **How recorded acts enter Schedule P.** §14.10 lets the Secretary make only entries of classes (a), (d) and (e), and drafts. Acts recorded since v1.0 took effect that made or changed a policy, such as Entries 6–9, need a way in. The new sentence has the Secretary enter each as an entry of its own, marked in force where the registry records it as valid. The earlier policy such an act changed keeps its own status: Entry 9 is in force, while P2-004 v1.0, which it amends, still awaits ratification. governance-rand#4's text had no such sentence. Its Sequence had the Secretary make every row in the status the table gives, which §14.10 does not allow for classes (b) and (c).
- **Two smaller changes.** "A policy not ratified" now reads "a policy still awaiting ratification", so the recorded acts above are not swept up when bootstrap ends. And acts taken in reliance stay "open to the same checks as any other act of the body that took them", in place of "remain open under §2.3", which reaches only decisions of the membership.
- **Difference from governance-rand#4.** Its §16.4 ended with a sentence about works published before the new §9.4 and their licenses. That sentence is left out here. It belongs with §9.4, which sibling proposal A amends and where it now sits.

### Appendix: two provenance rows (informative)

**Where:** two new rows in the appendix table, right after the §14.7 row ([v1.1 L477][v11-app-14.7]).

**Proposed:**

| Bylaws provision | Demand | Source |
|---|---|---|
| §14.8 | Order of instruments: law, articles, official document and invariant registry, bylaws text, suite and dispute design, board policies, procedures | P2-001 Authority Hierarchy, corrected; §1.2; §15.2; KRS 273.247(4) |
| §14.9, §14.10, §16.4 | Every policy has one place, filed under the section it serves; authority by class, not series; pinned by commit; numbers never reissued; pre-v1.0 policies ratified only as conformed | KRS 273.161(6), 273.191, 273.228; P1-001 v8.0 Appendix B precedent; §9.16 (identifiers never reused); President's direction of 2026-11-13 |

**Why.** The appendix records the source of each structural demand. It is informative, not operative. governance-rand#4's other two rows, for §9.4 and §14.3, belong to sibling proposals A and C.

### New file: the Schedule P register (draft opening)

**Where:** a new file beside the bylaws, `P1-001_Schedule-P_Register-of-Policies.md`. The suite checks only the bylaws file, so B1–B8 are unaffected by it.

**What it holds.**

- **The opening** from governance-rand#4's "The Schedule P file", with "opened by governance registry Entry [n]" kept as a bracket.
- **A draft notice.** The file says it is a draft opening. It takes effect only when §14.8–§14.10 and §16.4 are adopted and the Secretary opens it by that registry entry. Until then no row binds. It also says what the Secretary enters at opening, and that no other row is marked in force.
- **Rules of the register,** 1–8 as in governance-rand#4, and two more. Rule 9 sets the Text column. Rule 10 names the registry of record. The file says which act issues the rules: the opening entry, as the Secretary's procedure for keeping the register. Rule 8 is changed in two ways. A stale draft is annotated with the date of its last change, in place of a "lapsed" status that rule 3 does not list. And the yearly review of board policies and procedures is marked as only proposed to the Board, since a Secretary's procedure cannot set the Board's duties.
- **96 rows under 13 Article headings.** 80 rows enter a document or a registry decision: one for each of the 76 rows of the placement table, with two rows split and two added (listed below). The other 16 rows point from a second section the table names to the row where the document is entered.
- **Columns** as rule 2 names them: Number · Title · Version · Serves · Class · Owner / kept by · Status · Registry entry · Text.

**How the rows were made.**

- **Statuses** are carried as the table gives them, except as listed under "Facts updated" below. Where the table's last column ("Changed afterwards by") stated a fact about the document, the status carries it too. The change paths themselves are not a column: §14.10 sets them by class.
- **Text column.** A pinned location where the table gives one: bylaws `4246602` for v1.0, Janus `9aa2332`, the Agrinet blobs, SoHoLINK `167f15b`, bylaws `3276781` for CONTRIBUTING. Otherwise "to commit and pin". Where no text exists to pin, such as the retired P2-014 or the vacant conflict-of-interest slot, the column says "—".
- **Number collisions** follow the suffix rule of governance-rand#4's "Number collisions". The two retired aliases, P1-005a and P1-006a, are shown in the Number cell of the document each one named.
- **Registry entries** link to the published registry wherever the table names one.
- **Two rows split by subject.** Entries 3 and 4 get one pointer row each. The repository codes of conduct (§14.6) and security policies (§13.1) get one row each, since the table places them under different sections.
- **Two rows added.** A pointer row for Entry 10 under §9.5, because the registry it publishes is the one §9.5 requires; the table predates Entry 10, and whether the row should stay is Question 14. And a row under §14.9 for the register's own rules, because they are a procedure of the Secretary and every policy has one place.

**Facts updated since governance-rand#4.**

- The registry is published (Entry 10). Registry entries can now serve as pins under §14.9, so each row for a registry entry cites the entry itself as its text. "Publish the registry", step 4 of governance-rand#4's sequence, is done.
- **§9.4 rows made conditional.** Where the table said a rule "goes into §9.4", the row says it moves there "when §9.4 is amended to carry it": the rows for Entry 4, Entry 9, P2-004 and the DCO rule. This proposal does not amend §9.4; sibling proposal A does. The P2-004 row also says it is "to be" split and corrected, since the correction of its Part 3 is only proposed. Until §9.4 carries the floor, the Board holds what Entry 9 decided.
- **DCO mechanics: awaiting ratification.** The table marked them "(c), in force as practice, to be confirmed by a recorded act". No act adopting them for the whole organization is recorded: Entry 4 notes the no-bypass check, and Entry 10 sets it for the registry repository only. §16.4 says such a policy does not bind until the Board ratifies it, so the row marks the mechanics awaiting ratification. The practice continues. The President's choice of DCO over a CLA is decided; what waits is a recorded act.
- **Recorded acts entered at opening.** The rows for Entries 6–7, 8 and 9 say they are entered under §16.4's opening sentence. Entry 8's row now says "in force", as that sentence provides, and keeps the table's "pending a confirming Board act".
- **No phantom rows.** The table said the P1-005 draft and the Voting Workflows canvas are "listed in (e)". No separate rows exist for them, and one document has one place, so each row now says its draft is class (e) and where it is.
- **Entry 5's row** says a reading of a membership condition stays out of board policy by design. It cites KRS 273.187(1) as the reason to keep such matters in the text, not as a bar on Schedule P.
- The register carries an AGPL-3.0 notice under Entry 9. At `3276781` the bylaws repository's LICENSE file still reads CC BY-SA 4.0.

**Before opening, the Secretary** confirms each suffix and reads the texts the inventory never read. The file lists them. Three kinds of fact in the table were reported by the inventory and never re-checked: the 2026-03-18 renumbering proposal, the P2-003 canvas's "[Board resolution required]" line and its Gitee ban, and whether each gen-1 Confluence page is deleted or current.

## How it would be adopted

1. **Deliberation and notice.** #federation-governance deliberates this proposal through testing, with no deadline. v1.1 does not say whether §15.1's notice under §6.4 binds a bootstrap act. This proposal recommends at least one week's notice in #federation-governance (§6.4), and a record of why if the founder board acts sooner.
2. **A bootstrap act under §16.1.** The founder board adopts the bylaws changes as a bootstrap act. Best: fold them into the pending v1.1 adoption, which already takes effect only that way ([v1.1 L3-5][v11-hdr]). Its header sentence would then also name these changes; the patch does not touch the header. If v1.1 is adopted first, these changes go into a new version file instead.
3. **Never by editing v1.0.** The README says an adopted instrument is "never patched" ([L53-58][readme-53]). The v1.1 header says v1.0 "stays in the record unchanged".
4. **Recorded in the registry.** The act is entered in [NTARI-RAND/governance-registry][reg-repo] by a pull request whose every commit carries a DCO sign-off (Entry 10), with the consents counsel confirms: every director under KRS 273.375, or every voting member under KRS 273.377 (Counsel question 3).
5. **Translations.** The seven translations of the bylaws (Arabic, Spanish, French, Hindi, Portuguese, toki pona, Chinese) are updated on adoption. Suite check B7 only checks that they exist, not that they match. Whether the register itself is translated is Question 11.
6. **Then Schedule P opens.** The same day, the Secretary opens Schedule P by a registry entry, after the checks listed above. That entry also issues the register's rules as the Secretary's procedure. The Secretary enters rows of classes (a), (d) and (e) and every draft ministerially (§14.10), and the published notices under §16.4. Under §16.4's opening sentence, the Secretary enters Entries 6–7, 8 and 9, each as an entry of its own, marked in force because the registry records them as valid. No other row is marked in force. Class (b) and (c) slots that are vacant, and drafts, wait for their own acts under §14.10.
7. **Housekeeping, outside this patch.**
   - The bylaws CONTRIBUTING file limits the repository to P1-001 and its translations ([L3-5][contrib-3]), and tells contributors to edit v1.0 in place, with the Board approving amendments in review ([L9-13][contrib-9]). Both need updating.
   - Canonical texts are committed to NTARI-RAND/Policies so that rows can be pinned.
   - The Board acts governance-rand#4 lists follow, each under §14.10: adopt P1-005, adopt a conflict-of-interest policy, ratify P2-004 v2.0, confirm Entries 6–8, ratify the DCO mechanics, and ratify or retire P1-003.

## What this proposal does not decide

- **§9.4, §7.4 and §14.3.** Siblings A and C own them.
- **Opening Schedule P.** That is a separate registry entry, "Entry [n]".
- **Any policy.** No policy is adopted, ratified or retired here. The register shows only each document's status on the day of opening.
- **If counsel rejects a Board-kept code of the bylaws.** The fallback keeps Schedule P as the one register but drops its claim to be a code of the bylaws. Board policies then bind as Board resolutions within the slots the text names (KRS 273.207, [273.228][krs-228], [273.195(2)][krs-195]). Every class (c) entry needs Board authorization. Any rule that is a bylaw in substance moves into the text under Article XV.
- **Procedures made by officers and federations.** A class (c) procedure issued by one officer or by a federation would be part of a code of the bylaws. KRS 273.191 vests the amending power in the board "unless otherwise provided in the articles of incorporation or the bylaws", so this is not plainly unlawful. It sits uneasily with KRS 273.228, which sets officer duties by the bylaws, by the Board, or by an officer the Board authorizes to prescribe other officers' duties. Counsel should confirm it. The fallback: Board authorization for every class (c) entry, which fits that last route.
- **The set-aside and the Board's management power.** The set-aside is a member power stated in the bylaws, which KRS 273.201 allows. How it fits KRS 273.207 (the board manages) is unverified.
- **A Board act on a federation's procedure.** §14.10 lets the Board amend or revoke any procedure, including one a federation adopted by its own majority. §6.5 leaves a matter given to a federation to that body. This proposal names the delegates' set-aside as the check on such a Board act, as §2.2 requires, but does not settle whether the power should reach a federation's procedures at all (Question 17).
- **Challenges to a refusal.** Article XII has no procedure for challenging a refusal under §3.3 or §14.10 (Question 13).
- **The member check during bootstrap.** A set-aside needs a delegates' ballot with at least three federations casting (§6.5). No federation has elected a delegate yet, so none can be held. The founder board holds the membership's powers (§16.1), so it could hear a set-aside petition itself. But then the body that adopted a board policy (§16.4) would also review it: the Board reviewing itself. §2.2 voids a power without a check. Question 3 asks whether the founder board may hear a set-aside with the membership's powers, and offers two other candidate checks.
- **Validity of past acts.** Entries 3–6 and 10 are bootstrap acts "decided by the President, for the founder board". Entry 9 is a Board act decided the same way. Entry 8 was decided by the President. No all-director consents are recorded for them. Whether Entry 9 meets KRS 273.375, and whether the bootstrap acts meet KRS 273.375 or KRS 273.377, is unverified. Schedule P would enter Entries 6–9 as the registry records them; it does not cure them.
- **After bootstrap.** Whether asynchronous majority ballots are valid member action under KRS 273.377 and 273.195 is unverified. It changes the later path for the text, not the placement.
- **The suite and dispute design.** §14.8 ranks them, but the dispute-mechanics design still has no amendment path in the bylaws, although it was revised on 2026-10-07.
- **The registry's mechanical form.** The registry names a future "policy register" in the record machinery. Schedule P is not that machine: it is the document-form index of policies, kept by the same office. When the policy register ships, Schedule P's rows migrate into it with the registry's entries.
- **Unread texts and unchecked facts.** Several Slack canvases and files were never read and may hold policies that need rows. The register lists them, with the three kinds of fact the inventory did not re-check.

## How it fits the other amendment proposals

Three proposals are filed together, each adoptable on its own:

- **A: [amend-9.4-licensing-floor](https://github.com/NTARI-RAND/governance-rand/pull/5)** amends §9.4 and its appendix row.
- **B: amend-schedule-p** (this one).
- **C: [amend-board-consent-and-conflicts](https://github.com/NTARI-RAND/governance-rand/pull/7)** amends §7.4 and §14.3, with appendix rows for each.

**Shared sections.** None. This proposal does not touch §9.4, §7.4 or §14.3.

**Patches that touch neighboring lines.** Each patch applies alone to `3276781`. Their edits sit close together in three places:

- A's §9.4 (L197) is next to this proposal's §9.5 (L199).
- C's §7.4 (L165) is next to this proposal's §7.5 (L167).
- C adds a §14.3 row just before the §14.7 appendix row; this proposal adds its rows just after it.

So when two patches are applied in turn, the second may not apply as it stands. A and C apply on top of each other cleanly. B needs `git apply --3way` when it goes after A or C, and A or C need it when they go after B. All six orders of the three were tested on fresh copies of `3276781`, with no conflict. Each gives the same file, which passes the suite with 112 provisions and 372 section references, 94 distinct, all resolving. B with A alone gives 370 references; B with C alone gives 369. These are the results for the three patches as filed, on 2026-11-13. If a patch changes, test again.

**Wording that assumes another proposal.**

- **§16.4 and licenses.** This §16.4 leaves out governance-rand#4's last sentence on works published before the new §9.4. A carries that sentence in §9.4. Without A, v1.1's §9.4 is unchanged, so no license transition is needed.
- **Without A, the version choice is made for JFA software.** The v1.1 draft had chosen "version 3 or any later version" for JFA software before Entry 9. Entry 9 then left "or any later version" against "only" open, with notices naming version 3 only meanwhile. If v1.1 is adopted without A, that wording becomes bylaws text, and §14.8 ranks it above Entry 9's version-3-only notices. For JFA software the open choice would then in effect be made as "or any later version" until §9.4 is amended. That follows from adopting v1.1's §9.4 as drafted, with or without B; B's §14.8 only states the order. A keeps the choice open as a bracket, "[or any later version | only]".
- **§14.9(b) and the conflict-of-interest policy.** §14.9 names "the conflict-of-interest policy of §14.3" as a vacant board-policy slot. v1.1's §14.3 and C's §14.3 both say the Board maintains that policy, so the slot fits either. C's §14.3 does not name Schedule P, so C stands without this proposal.
- **Consents.** §9.5 records "the signed consents" behind an act, and §14.10 and §16.4 send Board acts through §7.4. v1.1's §7.4 allows written consent under KRS 273.375. C would state that such consent must be signed by every director in office. The provisions here read correctly either way. With C, a Board act on Schedule P taken without a meeting needs every director's signature.
- **Rows that point to §9.4.** The register's rows for Entry 4, Entry 9, P2-004 and the DCO rule say their rules move into §9.4 "when §9.4 is amended to carry it". That is A. Without A, they stay where they are: Entry 9 binds as a Board act amending P2-004, P2-004 v1.0 awaits ratification, and the DCO rule rests on Entries 4 and 10 and practice, with its mechanics awaiting ratification.

## Test it yourself

You need git and Python 3. Until this proposal's pull request merges, its patch is only on that pull request's branch. After cloning governance-rand, check out that branch, or download the `.patch` file from the pull request instead. Then:

```
git clone -c core.autocrlf=false https://github.com/NTARI-RAND/governance-rand.git
git clone https://github.com/NTARI-RAND/bylaws.git
cd bylaws
git checkout 3276781
git apply --check path/to/governance-rand/tier-1-bylaws/amend-schedule-p.v1.1.patch
git apply path/to/governance-rand/tier-1-bylaws/amend-schedule-p.v1.1.patch
python bylaws-conformance-suite.py --doc P1-001_Bylaws_v1.1.md
git add -N P1-001_Schedule-P_Register-of-Policies.md
git diff --word-diff
```

- **Keep the patch's line endings.** The `-c core.autocrlf=false` above stops git from rewriting the patch's line endings when it checks out governance-rand, which has no `.gitattributes` file. A patch rewritten that way fails `git apply`. If you download the patch instead, keep it as downloaded.
- **Print the section sign.** On Windows, run the suite as `python -X utf8 bylaws-conformance-suite.py --doc P1-001_Bylaws_v1.1.md`.
- `git add -N` makes the new register file show in the diff. `git diff --word-diff` shows each changed word in place: `[-removed-]` and `{+added+}`.
- To try this proposal together with A or C, stage each patch before the next (`git add -A`), and use `git apply --3way` for any patch that does not apply as it stands.

## Test results

The patch applied cleanly (`git apply --check`, then `git apply`) to a fresh copy of NTARI-RAND/bylaws at `3276781`, and gave files byte-identical to the working copy it was made from. The suite then printed:

```
Bylaws conformance: P1-001_Bylaws_v1.1.md
-----------------------------------------
[PASS] B1 preamble, sixteen articles in order, appendix
[PASS] B2 provisions numbered 1..n inside each article -- 112 provisions across 16 articles
[PASS] B3 every section cross reference resolves -- 367 references, 94 distinct, all resolve
[PASS] B4 every lettered sub-item reference resolves -- 16 sub-item references, all resolve
[PASS] B5 header version agrees with the filename -- version 1.1
[PASS] B6 no personal data beyond the organizational footer
[PASS] B7 translations present beside the instrument -- 7 translations present
[PASS] B8 prior instruments preserved -- 10 prior instruments archived

This suite checks that the instrument is internally whole. It does
not check that a provision is wise, lawful, or consistent with the
architecture; those bind a reader, not a parser.

RESULT: all checks PASS
```

Before the patch, v1.1 had 108 provisions and 315 section references (88 distinct). The four new provisions bring it to 112.

Four further checks, by throwaway scripts that are not part of the patch:

- **Texts.** §7.5, §8.4 and §15.1 match governance-rand#4's tested texts word for word, with v1.1's own wording kept where stated above. §9.5, §14.8, §14.9, §14.10 and §16.4 differ from them only in the changes stated under each Why; §16.4 also leaves out its last sentence. §7.4, §9.4 and §14.3 are unchanged.
- **Register.** All 76 rows of the placement table have a row. Every section a row serves exists in the patched v1.1, including the lettered sub-items §1.4(b), §1.4(c), §1.4(d) and §3.2(b). Every row names a class and a status. The file holds no email address.
- **Siblings.** All six orders of applying A, B and C give the same file and pass the suite, as described above. So do all six ordered pairs.
- **Line endings.** The patch converted to CRLF line endings fails `git apply --check` on a fresh copy, which is why the steps above clone governance-rand with `core.autocrlf=false`.

## Questions for #federation-governance

The federation decides these, with no deadline.

1. Should Schedule P be a code of the bylaws the Board keeps, while the text stays member-only?
2. Should the delegates hold a power to set aside any board policy, and any Board act amending or revoking a procedure, as the member check on the Board's Schedule P power?
3. The delegates cannot carry a set-aside during bootstrap, since no federation has elected a delegate. May the founder board hear a set-aside petition with the membership's powers under §16.1, knowing it would be reviewing its own board policy? If not, which check on board policies works today: a recorded founder-board answer to any member's set-aside petition in #federation-governance, or a lapse of bootstrap board policies unless the first post-bootstrap Board reconfirms them?
4. Should the §6.9 deliberation procedure be a board policy, which fits KRS 273.195(2), or a procedure the Governance federation owns?
5. Must a federation vote before a pull request merges into an NTARI-RAND repository? The inventory reported that the Voting Workflows canvas requires one and the R&D Submission Guide does not (neither re-read here).
6. Should a pre-v1.0 policy left unratified at the end of bootstrap become superseded (proposed), or lapse after a fixed period?
7. Should the repository security defaults (Entries 6–7) be a board policy the Board can loosen, or bylaws text only members can change?
8. Who should write the v1.1 §16.2 "internal policy" that decides when bootstrap ends? The register leaves its class unset.
9. Do you agree with the collision rule, and with refusing the 2026-03-18 proposal to renumber P3-004 to P3-009?
10. Should "the English text controls", a new rule in §14.8, enter the bylaws text?
11. Must Schedule P and the changed provisions be translated into the seven languages? Who translates, and at what cost?
12. Once the canonical texts are committed, should each Slack canvas and ntari.org copy carry a banner naming the pinned commit?
13. A refusal to make an entry is "challengeable through Article XII, as under §3.3". But §12.5 lists five kinds of proceeding, each decided by ratings of "the offense", and a challenge to a refusal is not one of them; the same gap exists for §3.3 today. Should §12.5 add "a challenge to a refusal under §3.3 or §14.10", with its own way of deciding, or should such a challenge go to the delegates?
14. Should the register keep its pointer row for Entry 10, which governance-rand#4's table predates?
15. Should the suite gain a register check: every row names an existing section, a class and a status, and every in-force row names a commit or a registry entry?
16. Should Schedule P open on the day of the bylaws act (proposed), or only once the canonical texts are committed?
17. Should the Board's power to amend or revoke a procedure reach a procedure a federation adopts by its own majority (§6.5), or only office procedures and procedures that commit funds or bind outside parties?
18. Should the Board adopt the yearly review in register rule 8 as a board policy?

## Questions for counsel

1. Is a Board-kept code of the bylaws (Schedule P) valid under [KRS 273.161(6)][krs-161] and [273.191][krs-191] while the text stays member-only? Can officers and federations issue binding procedures within it, given [KRS 273.228][krs-228]? If not, is the fallback under "What this proposal does not decide" sound?
2. Is the delegates' set-aside, a member power stated in the bylaws (KRS 273.201), consistent with the board's power to manage (KRS 273.207)?
3. Which test applies to a bootstrap act: consent of every director ([KRS 273.375][krs-375]) or of every member entitled to vote ([KRS 273.377][krs-377])? While no member entitled to vote is recorded, does KRS 273.201(4) give the directors the sole voting power? Proposal C asks the same. Do the bootstrap acts decided by the President for the founder board (Entries 3–6 and 10), and Entry 8, meet it? Entry 9 is recorded as a Board act, not a bootstrap act: does it meet KRS 273.375? After bootstrap, do asynchronous majority ballots meet KRS 273.377 and 273.195?
4. Does a director's message in a Slack channel count as a signed written consent? Chapter 273 counts an electronic signature as a signature (KRS 273.161(21)); proposal C sets out the rest of the question.
5. Is citing a text by repository, commit and path enough to incorporate it by reference? Kentucky case law on this was read only in secondary summaries.
6. Once policies are part of the bylaws, must a significant change to one be reported as a change to governing documents on an IRS return the Institute files? Not checked; a question for counsel or the Treasurer.
7. What do the filed articles of incorporation say? They control an inconsistent bylaw, except on the number of directors, where a bylaw change controls unless the articles say otherwise ([KRS 273.247(4)][krs-247]); §14.8 ranks law first, so that exception holds. The register lists the articles as a copy still to obtain.

## Method and ethics

Claude (Anthropic) drafted this proposal at the direction of the author. It is one of three proposals split from the research note in governance-rand#4:

- **Texts.** It started from the note's eleven tested bylaws texts and took the eight changes and two appendix rows that put Schedule P into the bylaws. Each was checked against v1.1's actual wording and adapted where v1.1 differs: v1.1's §3.9 clause in §9.5 is kept, and §16.4 drops its sentence on licenses, which moves to sibling A. A review of the first draft then found gaps: who enters existing acts when Schedule P opens, what "these bylaws" means in §5.6 and §6.9, the check on a Board act on a procedure, and what §2.3 reaches. This version closes them, and each change from governance-rand#4's text is stated under its Why.
- **Register.** The register was built row by row from the note's placement table. A script then checked that every table row is present and every section a row serves exists.
- **Statutes.** KRS 273.187, 273.191, 273.211, 273.228 and 273.247 were re-read from the Kentucky Legislature's published texts for this version. Other sections are cited as governance-rand#4 read them.
- **Editing.** The bylaws file was edited by a script in which every replacement must match exactly once. The patch was made with `git diff`, applied to a fresh copy of the bylaws repository at `3276781`, and checked with the repository's own suite.
- **Siblings.** The sibling patches were applied with this one in every order, to name the overlaps honestly.
- **What ran.** The only code run was the bylaws repository's own suite and the drafting scripts. No code from contributors was run.
- **Read-only while drafting.** Nothing was committed, pushed, posted or commented anywhere until this pull request was opened.
- **No personal data.** The proposal contains no email addresses and no Slack user or message IDs. It names no founder board member and no contributor other than the author; the President is named only as the source of directions.
- **Not re-checked.** Statuses come from governance-rand#4's inventory and verification of 2026-11-13 and were not re-checked here, except the bylaws text, the registry entries, and the sibling patches.

Much of this text was drafted by a tool. The choices it proposes are the author's to propose and the federation's to test.

[gr4]: https://github.com/NTARI-RAND/governance-rand/pull/4
[reg]: https://github.com/NTARI-RAND/governance-registry/blob/main/GOVERNANCE-REGISTRY.md
[reg-repo]: https://github.com/NTARI-RAND/governance-registry
[v10-hdr]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L3-L5
[v11-hdr]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L3-L5
[v11-7.5]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L167
[v11-8.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L181
[v11-9.5]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L199
[v11-9.16]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L239
[v11-15.1]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L385
[v11-app-14.7]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L477
[readme-53]: https://github.com/NTARI-RAND/bylaws/blob/3276781/README.md?plain=1#L53-L58
[readme-62]: https://github.com/NTARI-RAND/bylaws/blob/3276781/README.md?plain=1#L62-L63
[contrib-3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/CONTRIBUTING.md?plain=1#L3-L5
[contrib-9]: https://github.com/NTARI-RAND/bylaws/blob/3276781/CONTRIBUTING.md?plain=1#L9-L13
[krs-161]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=49017
[krs-187]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=13621
[krs-191]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=13623
[krs-195]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44387
[krs-211]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=48301
[krs-228]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=13640
[krs-247]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=36676
[krs-375]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44380
[krs-377]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44388

---

*Licensed under the [GNU Affero General Public License, version 3](https://www.gnu.org/licenses/agpl-3.0.txt) (AGPL-3.0), under governance registry Entry 9. This repository's LICENSE file still reads GPL-3.0 until it is relicensed under the same entry.*
