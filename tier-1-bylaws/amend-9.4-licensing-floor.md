# Amend bylaws §9.4: AGPL-3.0 for every work, DCO sign-off with no bypass, no assignment

**Tier 1 research · Governance · Bylaws amendment proposal**
**Filed:** 2026-11-13 · **Author:** Jodson Graves
**Base:** NTARI-RAND/bylaws main at `3276781`, P1-001 v1.1 (draft) · registry at [NTARI-RAND/governance-registry][registry]

## Summary

This proposal rewrites one section of the draft bylaws, §9.4 "Licensing floor", so that the bylaws carry the license decision the Institute has already made and the contribution rule it already follows.

- **What changes.** v1.1 §9.4 today licenses JFA software under AGPL-3.0 "or any later version" and "the specification" under CC BY-SA 4.0, and says only that contributions come in "under terms consistent with this floor". The new §9.4 says:
  - every work the Institute publishes, documents and code alike, is under AGPL-3.0, as governance registry Entry 9 decided;
  - the official JFA document keeps the license its own text states (today CC BY-SA 4.0), changed only under §9.2;
  - the floor moves only toward a stronger copyleft, and only by the membership amending the bylaws;
  - every commit carries a DCO sign-off by its own author (a line certifying the author's right to submit the work), with no bypass;
  - authors keep their copyright; the Institute takes no assignment and requires no contributor license agreement (CLA);
  - works published earlier keep their licenses, and within [ninety] days the Institute also licenses under §9.4 every such work it wholly owns.
- **Why.** Entry 9 is a Board act on a Board policy, P2-004, which made AGPL the rule for software "unless a Board resolution says otherwise". A later Board act could undo Entry 9 or choose other terms again. Written into the bylaws text, the floor is something neither the Board nor an officer can lower (§7.5). Only the membership can change it, under Article XV. The same goes for DCO in place of a CLA, which the President chose deliberately.
- **Two choices stay open**, shown as brackets: "[or any later version | only]" and the "[ninety]"-day transition. The v1.1 draft had already chosen "or any later version" for software, before Entry 9. Entry 9 reopened that choice.
- **It stands alone.** It changes only §9.4 and that section's row in the informative appendix. It does not touch Article XVI.
- **It adopts nothing.** Merging this research into governance-rand adopts nothing. Adoption would be a bootstrap act of the founder board under §16.1, folded into the pending v1.1 adoption or made as a new version file, and recorded in the governance registry. Version 1.0 is never edited.
- **Tested.** The patch applies to bylaws `3276781`, and the bylaws suite passes all eight checks B1–B8 on the result.

## Terms

*Governance*

- **Bylaws, P1-001.** The Institute's bylaws. Version 1.0 is in force. Version 1.1 is a draft, pending adoption; it is the target of this proposal.
- **JFA.** The Janus Facing Architecture, the design the Institute stewards. Its specification is the official document (below).
- **Founder board.** The directors who run the Institute until federations elect representatives (§16.1).
- **Bootstrap; bootstrap act.** The period in which the founder board holds the membership's powers, and an act it takes with those powers. Each bootstrap act is recorded in the governance registry and stays open to challenge (§16.1, §2.3).
- **Board act.** An act of the Board as the Board, under its own powers. A later Board can reverse it. Entry 9 is a Board act.
- **Membership; delegates; Article XV.** The members, organized in federations, one per layer of the architecture. Each federation elects a delegate. Article XV lets only the membership amend the bylaws, by a majority of delegates after each federation has voted (§15.1).
- **Governance registry; Entry.** The public, append-only record of governance acts the Secretary keeps (§9.5). Since Entry 10 its record copy is the `main` branch of [NTARI-RAND/governance-registry][registry]. Each act is an Entry.
- **P2-004.** The Board policy *Licensing and Enforcement Strategy*. Entry 9 amended its Part 2. Its Part 3 still calls for a CLA and copyright assignment.
- **Official document.** `janus-facing-architecture.md`, the JFA specification, as §1.5 defines it.
- **Floor.** A minimum rule that no lower instrument or act may go below.
- **#federation-governance.** The channel in the Institute's Slack workspace where Governance-layer research is deliberated, through testing, with no deadline.
- **KRS.** Kentucky Revised Statutes. Chapter 273 governs nonprofit corporations such as the Institute.
- **Provenance appendix.** The table at the end of the bylaws that names the source of each provision. It is informative: it explains, and binds no one.

*Licenses and copyright*

- **Copyleft.** A license condition: anyone may copy, change and share the work, but copies and changed versions must carry the same freedoms.
- **AGPL-3.0.** The [GNU Affero General Public License, version 3][agpl]. A copyleft license written for software, which covers any copyrightable work, documents included. A changed program that people use over a network must offer them its source.
- **CC BY-SA 4.0.** [Creative Commons Attribution-ShareAlike 4.0][ccbysa]. A copyleft license built for documents, images and data.
- **"Or any later version" / "only".** A grant under "or any later version" lets anyone also use later AGPL versions that the Free Software Foundation (FSF) publishes (AGPL §14). A grant under "only" does not.
- **Proxy (AGPL §14).** A person or body the licensor names to decide whether later license versions may be used.
- **Source; object code.** AGPL's words. The source is "the preferred form of the work for making modifications to it": for a document, the Markdown file. Any other form, such as a rendered page, a PDF or a print, is object code (AGPL §1).
- **Relicense.** Publish a work under a different license. Only someone holding the copyright can do it.
- **Dual license.** Offering one work under two licenses, typically copyleft for free and closed terms for a fee.
- **Assignment.** A transfer of copyright ownership.
- **CLA (contributor license agreement).** A contract a contributor signs before their work is accepted. P2-004's CLA transfers the copyright to the Institute.
- **DCO (Developer Certificate of Origin 1.1).** A [short statement][dco] a contributor certifies by adding a `Signed-off-by` line to each commit: that they have the right to submit the work under the license indicated in the file. It transfers no copyright.
- **Commit; commit author.** A commit is one recorded change in a git repository. Its author is the person git records as having made it.
- **Ruleset.** A GitHub repository setting that enforces checks, such as the DCO check, before a change can merge.
- **Bypass.** A setting that lets some accounts, such as administrators, merge a change that fails a required check.
- **SPDX notice.** A standard one-line license tag in a file, such as `SPDX-License-Identifier: AGPL-3.0-only`.
- **Wholly holds.** Owns all the copyright in a work, with no part owned by anyone else.
- **Joint work.** Under US copyright law, a work two or more authors made intending their parts to merge into one whole ([17 U.S.C. §101][usc101]). Its authors co-own the whole.

*Testing*

- **Conformance suite.** A program that checks a document. The bylaws suite (`bylaws-conformance-suite.py`) checks structure only: articles, numbering, cross references, version, privacy, translations, history. It does not judge meaning.
- **Patch.** A file listing the exact lines to change. `git apply` makes the change in a copy of the repository.

## The amendment

Two changes to `P1-001_Bylaws_v1.1.md`: §9.4 is replaced, and its row in the provenance appendix is replaced. Nothing else changes, and no section is added.

### §9.4 Licensing floor (replace; [v1.1 line 197][v11-9.4])

**Current v1.1 text:**

> **9.4 Licensing floor.** JFA software is licensed under the GNU Affero General Public License, version 3 or any later version (AGPL-3.0-or-later), and the specification under the Creative Commons Attribution-ShareAlike 4.0 International license (CC BY-SA 4.0). The Institute never relicenses either into proprietary terms, accepts contributions only under terms consistent with this floor, and signs no agreement that would let any party — including the Institute — close what is open.

**Proposed text:**

> **9.4 Licensing floor.** Every work the Institute publishes, software and documents alike, JFA software, the conformance suites, these bylaws, its policies, research, and educational material included, is licensed under the GNU Affero General Public License, version 3 [or any later version | only] (AGPL-3.0); the official document alone keeps the license its own text states, which changes only under §9.2. The floor moves only toward stronger copyleft: the membership may, by amendment under Article XV, name a successor license that keeps every freedom and every reciprocal obligation of AGPL-3.0, the duty to offer source to network users included, and no act moves a work to a weaker license. Work the Institute did not write keeps its own license, and the Institute's changes to it follow this floor wherever that license allows. The Institute never relicenses any work into proprietary terms and never offers a work under a second license for any party's private advantage. It accepts a contribution only when each commit carries a sign-off under the Developer Certificate of Origin by the commit's author, and that check admits no bypass; the author keeps the copyright, and the Institute takes no assignment of copyright and requires no contributor license agreement, so that copyright stays spread among those who wrote the work. It signs no agreement that would let any party — including the Institute — close what is open. Works published before this section took its present form keep the licenses they carry (§13.2), and within [ninety] days of that day the Institute also licenses under this section every such work whose copyright it wholly holds.

**Why.** The text starts from the §9.4 text tested in [governance-rand#4][pr4] ("The new bylaws text"), adapted to v1.1. Each part is explained below.

**One license for every work.** Governance registry Entry 9 (2026-11-13) decided: "Every work the Institute publishes is licensed under the GNU Affero General Public License, version 3 (AGPL-3.0): software, and documents alike." It adds: "This holds until a stronger copyleft appears." The President's direction was "we want to be AGPL-3 across the board until a stronger version of copyleft appears", and then "AGPL-3 for all docs and code" ([registry][registry], Entry 9). The text lists kinds of work so that no one reads "work" narrowly: JFA software, the conformance suites (the JFA suite and the bylaws suite), the bylaws themselves, policies, research and educational material. The word "publishes" matters: the floor licenses what the Institute makes public. It does not force an internal document into public view. Entry 10, for example, kept a security report internal.

**What AGPL means for a document.** AGPL treats a document exactly as it treats code ([governance-rand#4][pr4], "What AGPL means for a document").

- It covers any work. AGPL defines "the Program" as "any copyrightable work licensed under this License" (§0).
- The Markdown file is the source. A rendered web page, a PDF and a print are object code (§1).
- Every copy carries its source. A copy in another form must come with the source, or with a written offer of it for a print (§6(b)), or with clear directions to a server that holds it (§6(d)). CC BY-SA never required this. It is the reason Entry 9 chose AGPL for prose.
- Every copy carries the license. The full license text goes with each copy, not only a link (§4).
- These duties bind everyone who passes a copy on. For work the Institute wholly owns, the Institute is the licensor, and a licensor is generally not bound by its own license; counsel can confirm this reading. governance-rand#4 proposes that the Institute bind itself to the same practice in P2-004 part 2.2. That policy text is not adopted, and this amendment does not adopt it.

**The costs Entry 9 accepted.** governance-rand#4 first recommended CC BY-SA 4.0 for documents because of these costs ("Costs the decision accepts"). Entry 9 accepts them:

- every PDF, handout and slide deck must carry the full license text;
- AGPL does not itself bar copies locked with digital rights management (DRM);
- whether AGPL reaches database rights is uncertain;
- AGPL text cannot go into CC BY-SA commons such as Wikipedia;
- CC BY-SA images are, as a rule, linked rather than copied into AGPL documents. Entry 9 says they "cannot be placed" there. The narrow exception: Creative Commons allows a one-way route from CC BY-SA 4.0 into GPLv3, but calls it "not for general use", and no CC or FSF statement covers a route onward into AGPL (governance-rand#4, "Compatibility facts").

**The official document keeps its own license.** The words "the official document alone keeps the license its own text states, which changes only under §9.2" replace v1.1's "and the specification under ... CC BY-SA 4.0".

- **Today the result is the same.** The official document's footer reads "Specification: CC BY-SA 4.0" ([Janus line 168][j-168]). The President directed that it keep that footer for now, and Entry 9 left it unchanged.
- **The bylaws stop restating it.** The official document's own text decides its license. Only an amendment under §9.2 changes it: a majority of delegates, with the JFA conformance suite passing. Two instruments that state the same license can drift apart. One that cites the other cannot. This follows §14.7: where the official document governs a matter, the bylaws "cite it rather than restate it".
- **The term is now a defined one.** v1.1 said "the specification", which the bylaws never define. §1.5 defines "the official document" as one file, `janus-facing-architecture.md`. Other JFA documents, such as the dispute-mechanics design and the open-questions document, are not the official document, so they follow the floor like any other work, as Entry 9 already provides.

**The bracket: "[or any later version | only]".** This choice stays visibly open.

- **What v1.1 says now.** The v1.1 draft had already chosen "or any later version" for software, before Entry 9 ([v1.1 line 197][v11-9.4]). The official document's footer says the same for software, without qualification: "Software: AGPL-3.0-or-later" ([Janus line 168][j-168]). Its introduction is softer: JFA software is designed for a copyleft environment, "generally the GNU Affero General Public License, version 3 or later (AGPL-3.0-or-later)" ([Janus line 15][j-15]). governance-rand#4 counted 84 "AGPL-3.0-or-later" notices across six NTARI repositories and no "-only" notices (code search, 2026-11-13, not re-checked here).
- **What Entry 9 says.** Entry 9 left the choice open. Until it is made, notices written under Entry 9 name version 3 only, because the Institute can later widen its own grants but never narrow one once made. The registry's own footer already reads "AGPL-3.0-only" (Entry 10).
- **For "or any later version".** It matches existing practice and v1.1. A later FSF version could be used without anyone's consent, which fits "until a stronger copyleft appears".
- **For "only".** The FSF, not the membership, judges what a later version is. AGPL §14 promises only that later versions will be "similar in spirit". Under "only", a move to a later version would come through this section's successor-license clause, or through a proxy the Institute names under AGPL §14.
- **Adoption needs one side.** The adopted text cannot keep the bracket. The founder board picks one after the federation deliberates. The short name in parentheses stays "AGPL-3.0"; notices would use `AGPL-3.0-or-later` or `AGPL-3.0-only` to match.

**The floor moves only toward stronger copyleft.** Today the rule lives in a Board policy, and a Board can change its own policies.

- **The gap today.** Entry 9's authority line quotes P2-004 §2.1: software is AGPL-3 "unless a Board resolution says otherwise". Entry 9 withdrew P2-004's criteria for other licenses, but a later Board act could restore them.
- **What the bylaws text adds.** The Board may not amend the bylaws (§7.5). Once the floor is in §9.4, only the membership can change it, by an Article XV ballot that every member of every federation may vote in (§15.1).
- **What "only toward stronger copyleft" means.** The membership may name a successor license only if it keeps every freedom and every reciprocal duty of AGPL-3.0, the duty to offer source to network users included. And "no act moves a work to a weaker license".
- **Its honest limit.** No text can bind a future amendment absolutely. The membership could amend this sentence itself under Article XV. During bootstrap, the founder board holds the membership's powers (§16.1), so it could amend §9.4 by a recorded bootstrap act, open to challenge under §2.3. What the text does is take the choice away from the Board and every officer, and make any weakening a noticed member ballot. Grants already made stand whatever happens (§13.2).
- **Why a ratchet.** The floor is a check that protects the commons from the Institute itself. §2.2 requires every power to name its check. The power to license the Institute's works is checked here.
- **Detail stays in policy.** What counts as a qualifying successor (for example, listed as free by the FSF, and approved by the Open Source Initiative for software) is set out in governance-rand#4's draft P2-004 part 2.3. The bylaws keep only the floor.

**Others' work keeps its license.** "Work the Institute did not write keeps its own license." For example, the Phase 1 Conformance Report in governance-rand ([governance-rand#2][gr2]) stays GPL-3.0 unless its author agrees otherwise, as Entry 9 records. AGPL §13 lets AGPL and GPL parts sit in one work. The Institute's own changes to such work follow the floor wherever that work's license allows.

**No proprietary relicensing, no dual licensing for sale.**

- "Never relicenses any work" replaces "never relicenses either". In v1.1 "either" meant software and the specification. In v1.0 the same sentence said "either" with only one object named ([v1.0 line 189][v10-9.4]), as governance-rand#4 noted.
- "Never offers a work under a second license for any party's private advantage" bars selling closed licenses beside the copyleft one. It does not touch old licenses that stay alive under §13.2, or the official document's own license.

**DCO by the commit's author, with no bypass; no CLA, no assignment.**

- **What v1.1 lacks.** v1.1 says only that the Institute "accepts contributions only under terms consistent with this floor". A CLA that assigns copyright to the Institute could pass that test on paper. P2-004 v1.0 Part 3 calls for exactly that.
- **The direction.** The President decided that DCO instead of a CLA is deliberate. Spread-out copyright adds friction for anyone, the Institute included, who would take a work out of copyleft. Relicensing a contribution needs the consent of whoever holds its copyright. If a file were a joint work ([17 U.S.C. §101][usc101]), each co-owner could license it non-exclusively alone, owing the others an accounting for any profits. Whether NTARI's collaborative files are joint works is a question for counsel (below); it bears on how much friction DCO gives, and does not reopen the decision. Under assignment, one owner holds everything, and only a promise stands between the commons and a relicense ([governance-rand#4][pr4], "Why DCO is deliberate").
- **It is today's practice.** The bylaws repository's contributing guide requires a `Signed-off-by` line matching the commit author on every commit ([CONTRIBUTING lines 22–38][contrib-22]). Entry 4 records that the DCO check "has no bypass", and Entry 10 repeats it for the registry. governance-rand#4 reported that all 27 NTARI-RAND repositories then had a "Require DCO" ruleset with no bypass actors (GitHub API, 2026-11-13; not re-checked here).
- **The license must be indicated in the file.** DCO 1.1 certifies the right to submit under the open source license "indicated in the file". Most NTARI Markdown files indicate none, so each needs a one-line SPDX notice or footer (governance-rand#4, "Compatibility facts"). Entry 9 point 4 already directs that notices change to AGPL-3.0.
- **"By the commit's author".** The sign-off is the author's own, as the DCO check enforces. DCO 1.1 lets that author certify work they did not write, such as compatible code from elsewhere, when they have the right to submit it.
- **What it makes inconsistent.** Once adopted, this floor conflicts with P2-004 Part 3's CLA and assignment. governance-rand#4 proposes replacement text for that part (P2-004 v2.0), which the Board would ratify. That is a separate act.

**Works published earlier: the transition, moved here from §16.4.**

- **Where it was.** governance-rand#4 put this sentence in a new §16.4: "Works published before §9.4 took its present form keep the licenses they carry (§13.2), and within [ninety] days the Institute brings into §9.4 every such work whose copyright it wholly holds." §16.4 belongs to sibling proposal B (Schedule P). Here the sentence ends §9.4 itself, so this proposal stands alone and does not touch Article XVI.
- **What was adapted.** "Before §9.4" became "before this section". "Within [ninety] days" gained "of that day", so the period has a clear start. "Brings into §9.4" became "also licenses under this section". The word "also" says what §13.2 requires: the old license stays, and the AGPL grant is added beside it. Entry 9 says the same: earlier versions stay "available under that license as well".
- **"Keep the licenses they carry".** No act may impair a license already granted (§13.2). This also covers the 84 "or-later" notices if the bracket goes to "only": those grants stand as made.
- **"Whose copyright it wholly holds".** The Institute can relicense only what it owns in full. Other holders' work moves only with their consent. Whether the Institute owns its officers' commits is unverified: governance-rand#4 found no employment record or officer assignment.
- **"[ninety]" is a choice.** It is a backstop deadline, not the start of the work (see below).

**Relicensing does not wait for this amendment.** Entry 9 already directs the Institute to bring its repositories into line: LICENSE files, notices and descriptions changed to AGPL-3.0 wherever it holds the copyright. The registry records that this is "being carried out from 2026-11-13". If that work is done before adoption, the ninety-day sentence is spent but harmless. What this amendment adds is permanence: the floor becomes something neither the Board nor an officer can lower.

**Sections that point here still read true.** §9.8 says the Institute "licenses" the covenant scale, LBTAS, "under §9.4". §9.17 says the suite is "published and executable by anyone under §9.4". §10.8 asks members to comply with the AGPL. §13.2 says the official document and the software "survive the Institute". §1.4(b) stewards JFA software "under copyleft terms". None of them needs a change.

### Appendix — Provenance of Demands, row §9.4 (replace; [v1.1 line 441][v11-app])

**Current v1.1 text:**

> | Bylaws provision | Demand | Source |
> |---|---|---|
> | §9.4 | AGPL-3.0-or-later software, CC BY-SA 4.0 specification, copyleft commons | Official document, Introduction and footer |

**Proposed text:**

> | Bylaws provision | Demand | Source |
> |---|---|---|
> | §9.4 | AGPL-3.0 for every work, software and documents, until a stronger copyleft; the official document keeps its own license until §9.2; works published earlier keep their licenses; DCO sign-off by the commit's author with no bypass; authors keep copyright; no assignment, no contributor license agreement | President's direction of 2026-11-13; governance registry Entries 4 and 9; P2-004 part 2, as amended by Entry 9; official document, footer |

The header row is quoted for readability and does not change.

**Why.** The appendix names the source of each provision. The old row no longer describes the new §9.4. The new row adapts governance-rand#4's appendix row for §9.4, with three changes:

- **One row replaced, none added.** v1.1 already has a §9.4 row, so it is replaced in place, and "(as amended)" is dropped.
- **"P2-004 part 2, as amended by Entry 9" replaces "P2-004 parts 2 and 3, as amended and corrected".** Part 3 has not been corrected; its correction is only proposed. The DCO rule's sources are the President's direction and Entry 4.
- **"Official document, footer" stays**, as the source of the exception.

## How it would be adopted

1. **Deliberation first.** #federation-governance deliberates this proposal through testing, with no deadline. Merging it into governance-rand adopts nothing.
2. **Fill both brackets.** Before adoption, the founder board picks "or any later version" or "only", and a transition period. The adopted text carries no brackets.
3. **A bootstrap act under §16.1.** The founder board, exercising the membership's powers, adopts the text. It is folded into the pending v1.1 adoption, which takes effect only that way anyway ([v1.1 lines 3–5][v11-hdr]), or made later as a new version file. If it is folded into v1.1, the adopting act should say so. The v1.1 header lists what v1.1 carries, and this patch leaves the header alone.
4. **Never by editing v1.0.** The bylaws README says the adopted text is "never patched" ([README lines 53–58][readme-53]). v1.1's header says version 1.0 "stays in the record unchanged".
5. **Recorded in the governance registry** under §9.5, as a new entry added to [NTARI-RAND/governance-registry][registry] by a signed-off pull request (Entry 10). The entry should record how the act was taken. Which consent test applies to a bootstrap act is a question for counsel (below).
6. **Translations updated.** The bylaws are published in seven other languages: Arabic, Spanish, French, Hindi, Portuguese, toki pona and Chinese. Each v1.1 translation carries this section and its appendix row, so 14 passages change. Suite check B7 only checks that the seven files exist, not what they say. They must be updated on adoption.
7. **After bootstrap,** a change to §9.4 needs an Article XV ballot of the delegates (§15.1).
8. **Separate follow-up acts.** The bylaws repository's README still says its license is CC BY-SA 4.0 and that AGPL-3.0 "does not apply here" ([README lines 99–105][readme-99]). Entry 9 already directs that notice to change. P2-004 Part 3 needs its own Board act (governance-rand#4's P2-004 v2.0).

## What this proposal does not decide

- **The bracket and the period.** Both are choices for the founder board after deliberation.
- **The JFA specification's license.** It stays CC BY-SA 4.0 until an amendment of the official document under §9.2. The JFA conformance suite checks the licensing statement, so it would change too (Entry 9).
- **The official document's translations.** Whether its seven translations share its exception is not settled. §1.5 names only the English file.
- **Code officers hold personally.** §9.4 binds "the Institute", not individual authors. Code an officer owns personally falls outside the floor, as governance-rand#4 notes. It lists ways to close this gap: voluntary officer assignments, or a personal covenant signed by the officer. This proposal chooses neither.
- **Who owns the officers' commits.** Unverified. The answer sets how far the transition sentence reaches.
- **P2-004 Part 3, the volunteer letters and enforcement.** This proposal does not replace the CLA text in P2-004. It does not deal with CLA wording already sent to volunteers, or with optional enforcement authorizations. governance-rand#4 covers each.
- **Whether to name a proxy** under AGPL §14, if "only" is chosen.
- **Logos and brand marks.** Whether §9.4 should leave them out is governance-rand#4's question 21.
- **Where policies are filed.** Schedule P is sibling proposal B.
- **Notices and LICENSE files.** Entry 9 already governs them, and this patch edits none.

## How it fits the other amendment proposals

Three proposals are filed together. Each is meant to be adoptable on its own:

- **(A) amend-9.4-licensing-floor**: this one.
- **(B) [amend-schedule-p](https://github.com/NTARI-RAND/governance-rand/pull/6)**: one register of policies, Schedule P.
- **(C) [amend-board-consent-and-conflicts](https://github.com/NTARI-RAND/governance-rand/pull/7)**: Board written consent and conflicts of interest.

This proposal's wording assumes neither sibling. It cites only §9.2, §13.2 and Article XV, which v1.1 already has.

The combined tests below used the three patches as filed, on 2026-11-13. Every order of every pair, and all six orders of the three, gave the same file each time. If a patch changes, run them again.

**With B (Schedule P).** B carries governance-rand#4's Schedule P texts: it changes §7.5, §8.4, §9.5 and §15.1, adds §14.8–§14.10 and §16.4, adds two appendix rows right after the §14.7 row ([v1.1 line 477][v11-477]), and adds the Schedule P file.

- **The transition sentence.** governance-rand#4 ended its §16.4 with the transition sentence, which this proposal moves into §9.4. B's §16.4 leaves it out, so the sentence appears once, here.
- **Overlapping patches.** B's §9.5 is two lines below §9.4, and the two patches share context lines. Tested in both orders on fresh copies of `3276781`: the first patch applies with a plain `git apply`; the second fails a plain `git apply` and applies cleanly with `git apply --3way` (stage the first patch's change with `git add -A` before applying the second; without that, `--3way` stops with "does not match index"). The texts do not conflict. With both applied, the suite passes all checks: 112 provisions; 370 references, 94 distinct.
- **The appendix.** B's new rows go right after the §14.7 row (v1.1 line 477), far from the §9.4 row (line 441), so they do not touch this patch's appendix change.
- **What B expects of this proposal.** B's register files P2-004, Entry 9 and the DCO rule under §9.4. It says a rule "moves into the §9.4 text" only if §9.4 is amended to carry it. This proposal is that amendment. If B is adopted without it, those rules stay where they are today: in a Board act, a Board policy and practice.
- **Order of instruments.** B's §14.8 would state the order of instruments: the official document above the bylaws text, and Board policies below it. That would make two readings explicit: the official document's own license statement stands, and P2-004 Part 3 yields to §9.4. It has a third effect, on the bracket: with B's §14.8, choosing "only" would yield to the official document's "or-later" software line (its footer, line 168) unless the official document is amended under §9.2 first or at the same time. This proposal does not depend on B. Without B, the rank of a Board policy below the bylaws text rests on general corporate law, which counsel should confirm.

**With C (Board consent and conflicts).** C changes §7.4 and §14.3 and their appendix rows. Its §7.4 row sits five lines above the §9.4 row, but the two patches change no shared line. Tested in both orders: both apply with a plain `git apply`, and the suite passes all checks: 108 provisions; 320 references, 89 distinct. Two links:

- **Consent.** C states how the Board acts by written consent (§7.4). Whether a bootstrap act that adopts bylaws text follows that rule, or the rule for member action, is a question for counsel (below).
- **Conflicts.** If officers choose to assign their own NTARI work to the Institute, to bring it under this floor, each assignment is a transaction with an officer. It calls for disclosure under §14.3, in its current or C's form.

**All three together.** Tested in all six orders. A and C apply on top of each other with a plain `git apply`. B needs `git apply --3way` when it follows A or C, and A or C need it when they follow B (stage each patch's change with `git add -A` before applying the next). Every order gives the same file, with no conflict markers, and the suite passes all checks: 112 provisions; 372 references, 94 distinct.

## Test it yourself

You need git and Python 3. Until this proposal's pull request merges, its patch is only on that pull request's branch. After cloning governance-rand, check out that branch, or download the `.patch` file from the pull request instead. Then:

```
git clone -c core.autocrlf=false https://github.com/NTARI-RAND/governance-rand.git
git clone https://github.com/NTARI-RAND/bylaws.git
cd bylaws
git checkout 3276781
git apply --check path/to/governance-rand/tier-1-bylaws/amend-9.4-licensing-floor.v1.1.patch
git apply path/to/governance-rand/tier-1-bylaws/amend-9.4-licensing-floor.v1.1.patch
python bylaws-conformance-suite.py --doc P1-001_Bylaws_v1.1.md
git diff --word-diff
```

Two notes for Windows:

- **Keep the patch's line endings.** The `-c core.autocrlf=false` above stops git from rewriting the patch's line endings when it checks out governance-rand, which has no `.gitattributes` file. A patch rewritten that way fails `git apply`. If you download the patch instead, keep it as downloaded.
- **Print the section sign.** Run the suite as `python -X utf8 bylaws-conformance-suite.py --doc P1-001_Bylaws_v1.1.md`.

`git diff --word-diff` shows each changed word in place: `[-removed-]` and `{+added+}`.

## Test results

The patch was applied to a fresh copy of NTARI-RAND/bylaws at `3276781`. `git apply --check` passed. The suite printed:

```
Bylaws conformance: P1-001_Bylaws_v1.1.md
-----------------------------------------
[PASS] B1 preamble, sixteen articles in order, appendix
[PASS] B2 provisions numbered 1..n inside each article -- 108 provisions across 16 articles
[PASS] B3 every section cross reference resolves -- 318 references, 88 distinct, all resolve
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

For comparison, unpatched v1.1 gives 108 provisions and 315 references, 88 distinct. The three new references are §9.2 and §13.2 in §9.4, and §9.2 in the appendix row. No provision is added or renumbered. The suite checks structure, not meaning: it cannot tell whether the text is wise or lawful.

## Questions for #federation-governance

The federation deliberates these, with no deadline.

1. **The bracket.** Should §9.4 say AGPL-3.0 "or any later version", or "only"? The v1.1 draft had chosen "or any later version" for software before Entry 9. Until this is decided, notices name version 3 only.
2. **A proxy.** If "only": should the bylaws name a proxy under AGPL §14, such as the Institute or its successor steward under §13.3? Or should every move to a later version go through the successor-license clause, by Article XV?
3. **The official document's software line.** If "only": the official document's footer states without qualification "Software: AGPL-3.0-or-later" ([line 168][j-168]), while its line 15 says "generally" AGPL-3.0-or-later ([line 15][j-15]); the two lines differ in force. §15.2 says no amendment may "override the official document". Should a §9.2 amendment align the official document first, or at the same time? Without proposal B, whether "only" in the bylaws would count as overriding it is unverified. With B's §14.8, which ranks the official document above the bylaws text, choosing "only" would yield to the official document's "or-later" software line unless the official document is amended under §9.2 first or at the same time.
4. **The transition period.** Ninety days, another period, or no deadline at all, given that Entry 9 already directs the relicensing now?
5. **The JFA specification.** Should it follow Entry 9 to AGPL-3.0? That is a separate amendment of the official document under §9.2.
6. **Translations of the official document.** Should they share its license exception?
7. **Officer-held code.** For NTARI work that officers own personally, should the Institute ask for voluntary assignments, a personal covenant, or neither? It decides how far "wholly holds" reaches.
8. **Dual licensing.** Should the bar on "a second license for any party's private advantage" stand as written?
9. **Logos and brand marks.** Should §9.4 leave them out? AGPL §7(e) lets a licensor decline trademark rights, but AGPL would still license a logo's copyright.
10. **Timing.** Fold this into the v1.1 adoption, or adopt it later as a new version file?

## Questions for counsel

1. **Officers' commits.** Does the Institute own code its officers wrote? No employment record or officer assignment was found (governance-rand#4). The answer sets the reach of "whose copyright it wholly holds".
2. **The licensor's own duties.** Is the Institute, as licensor of works it wholly owns, bound by AGPL's source-and-license duties, or only those who receive copies from it?
3. **The bootstrap act.** Which consent test applies to a bootstrap act that adopts a bylaws text: every director (KRS 273.375) or every voting member (KRS 273.377)? governance-rand#4 asks this too. Proposal C bears on it, and cites KRS 273.201(4): where a corporation has no members with a right to vote, the directors hold the sole voting power.
4. **"Or later" on mixed repositories.** Can the Institute write "-or-later" on repositories declared "AGPL-3.0" that hold outside contributions? This is governance-rand#4's counsel question 8.
5. **Rank of a Board policy.** Without B's §14.8, does a Board policy such as P2-004 Part 3 yield to the bylaws text where they conflict?
6. **Joint works.** Are the Institute's collaboratively edited files joint works under 17 U.S.C. §101? If so, each co-owner could license a whole file non-exclusively without the others, subject to a duty to account for profits. The answer sets how much friction DCO actually gives against relicensing; it does not reopen the DCO decision.

## Method and ethics

Claude (Anthropic) drafted this proposal at the author's direction, as one of three sibling proposals filed together.

- **Starting point.** The §9.4 text and appendix row tested in [governance-rand#4][pr4] ("The new bylaws text"), together with its reasoning on licenses, DCO and the transition.
- **Adapted to v1.1.** governance-rand#4 wrote against v1.0 line numbers (§9.4 at v1.0 line 189). Here the target is v1.1 line 197, which already carried an "or later" grant and a CC BY-SA clause, and v1.1 line 441 for the appendix row. The transition sentence moved from governance-rand#4's §16.4 into §9.4, with the small wording changes explained above.
- **Sources read.** The bylaws at `3276781`: v1.0, v1.1, README, CONTRIBUTING and the suite. The governance registry, Entries 1–10. The governance-rand READMEs. Read-only GitHub queries confirmed that bylaws `main` is still `3276781`, and that Janus `main` is `9aa2332` with the license footer at line 168.
- **How the text was made.** The edit was made by a script that asserts each target text occurs exactly once. The suite ran on scratch copies. The patch was checked against a fresh copy of the bylaws repository. Further scratch copies tested it together with the sibling patches, in several orders.
- **Code run.** No code from outside contributors was run. The only program run was the bylaws repository's own suite, which uses Python's standard library.
- **Nothing published while drafting.** Nothing was posted, pushed, committed or commented anywhere until this pull request was opened.
- **Privacy.** The proposal holds no email addresses and no personal data. It names offices, never people, apart from the author line and the President's quoted directions.
- **Unverified claims are marked.** Counts reported by governance-rand#4 and not re-checked here are marked as such.
- **Reviewed.** Review passes checked the draft against the bylaws, governance-rand#4, the official document and the law it cites. Each correction was checked against those sources before it was made. The bylaws text in the patch did not change in review; the suite was run again on a fresh copy, and the combined tests with the sibling patches were repeated.

Much of this text was drafted by a tool. The choices it proposes are the author's to put forward and the federation's to test.

[registry]: https://github.com/NTARI-RAND/governance-registry/blob/main/GOVERNANCE-REGISTRY.md
[pr4]: https://github.com/NTARI-RAND/governance-rand/pull/4
[gr2]: https://github.com/NTARI-RAND/governance-rand/pull/2
[agpl]: https://www.gnu.org/licenses/agpl-3.0.txt
[ccbysa]: https://creativecommons.org/licenses/by-sa/4.0/legalcode.en
[dco]: https://developercertificate.org/
[usc101]: https://www.law.cornell.edu/uscode/text/17/101
[v11-hdr]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L3-L5
[v11-9.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L197
[v11-app]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L441
[v11-477]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L477
[v10-9.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L189
[readme-53]: https://github.com/NTARI-RAND/bylaws/blob/3276781/README.md?plain=1#L53-L58
[readme-99]: https://github.com/NTARI-RAND/bylaws/blob/3276781/README.md?plain=1#L99-L105
[contrib-22]: https://github.com/NTARI-RAND/bylaws/blob/3276781/CONTRIBUTING.md?plain=1#L22-L38
[j-15]: https://github.com/NTARI-RAND/Janus/blob/9aa2332/janus-facing-architecture.md?plain=1#L15
[j-168]: https://github.com/NTARI-RAND/Janus/blob/9aa2332/janus-facing-architecture.md?plain=1#L168

---

*Licensed under the [GNU Affero General Public License, version 3](https://www.gnu.org/licenses/agpl-3.0.txt) (AGPL-3.0), under governance registry Entry 9. This repository's LICENSE file still reads GPL-3.0 until it is relicensed under the same entry.*
