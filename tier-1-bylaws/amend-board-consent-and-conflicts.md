# Two checks on the Board: every director signs action without a meeting (§7.4), and no conflicted transaction is approved by one director (§14.3)

**Tier 1 research · Governance · Bylaws amendment proposal**
**Filed:** 2026-11-13 · **Author:** Jodson Graves
**Base:** NTARI-RAND/bylaws main at 3276781, P1-001 v1.1 (draft) · registry at NTARI-RAND/governance-registry

## Summary

This proposal changes two sections of the draft bylaws, v1.1, and two rows of its appendix. Both changes are checks on the Board.

- **§7.4 Action.** The Board may act without a meeting only by a written consent that every director in office signs. This is already Kentucky's default rule ([KRS 273.375][krs-273.375]), and neither v1.0 nor v1.1 departs from it; whether the filed articles of incorporation do is unverified, because they have not been retrieved. The text now says so, so that no one reads "continuously" as a lighter rule.
- **§14.3 Conflicts of interest.** A transaction in which a director holds a direct or indirect interest is authorized, approved, or ratified only after disclosure, by a majority of the directors who hold no interest in it, and never by a single director. Kentucky law does not forbid a single director's approval; it only denies that approval the safe harbor of KRS 273.219(1)(a) ([subsection (3)][krs-273.219]). This text forbids it outright, by choice. The duty to disclose, the duty to abstain and the duty to keep a conflict-of-interest policy stay word for word.
- **Appendix.** The §7.4 row is updated to match. A new §14.3 row says where the demand comes from.
- **Two gaps it names but does not close.** If buying insurance for every director under §14.5 counts as a transaction in which a director holds an interest, no disinterested majority could approve it. And because §7.4's quorum still applies, interested directors who stay away from a meeting could block approval. Both are left to the federation ([Questions 4 and 6](#questions-for-federation-governance)).
- **Why in the bylaws text.** Every power must name its check (§2.2). A check on the Board belongs where the Board cannot lift it: in the bylaws text, which only the membership amends (§7.5, §15.1).
- **Where the texts come from.** They are the tested §7.4 and §14.3 texts of [governance-rand#4][pr4], adapted to v1.1. §14.3 here leaves out that note's mention of Schedule P.
- **It adopts nothing.** Merging this file publishes research. Adoption would be a later bootstrap act of the founder board under §16.1, folded into the v1.1 adoption or made as a new version file, and recorded in the [governance registry][registry]. The patch beside this file passes the bylaws suite (checks B1–B8).

## Terms

- **KRS.** Kentucky Revised Statutes. Chapter 273 governs nonprofit corporations such as NTARI.
- **Counsel.** A lawyer advising the Institute.
- **The Board.** The board of directors. Every officer is a director (§8.1). Until bootstrap ends, the founder board serves as the Board ([§7.2][v11-7.2]).
- **Bootstrap; founder board.** The period before federations elect their directors. Until then a founder board of three to five directors serves as the Board and holds the membership's powers ([§16.1][v11-16.1]).
- **Bootstrap act.** An act the founder board takes with the membership's powers. It is recorded in the governance registry and stays open to the membership under §2.3.
- **Member; member entitled to vote.** Under §3.3, membership begins when the Secretary recognizes a member and records the recognition in the registry. Kentucky law speaks of members "entitled to vote". The registry records no recognition of a member so far.
- **Federation.** The members of one layer of the architecture. Each federation elects one director (§7.2).
- **#federation-governance.** The channel where the federation deliberates this research, through testing, with no deadline.
- **Governance registry.** The public, append-only record of governance acts the Secretary keeps under §9.5. Since registry Entry 10, the `main` branch of NTARI-RAND/governance-registry holds the registry of record.
- **Meeting.** Under §7.4, a Board meeting is synchronous or asynchronous, needs one week's notice, has a quorum of a majority, and is decided by a majority of those present.
- **Quorum.** The number of directors who must be present for a meeting to act. Under §7.4 it is a majority of the Board.
- **Written consent.** A Board decision taken without a meeting. It is a written document that describes the action, and the directors sign it. Kentucky's default is that every director signs (KRS 273.375).
- **Director in office.** A director who is serving now. A vacant seat has no one to sign.
- **Conflict-of-interest transaction.** Kentucky's term for "a transaction with the corporation in which a director of the corporation has a direct or indirect interest" ([KRS 273.219(1)][krs-273.219]).
- **Indirect interest.** In short: another organization is a party, and the director has a material financial interest in it or holds a post in it, such as director or officer. KRS 273.219(2) gives the exact test.
- **Disinterested director.** A director who holds no interest in the matter.
- **Authorize, approve, ratify.** Agree in advance, agree at the time, or confirm afterwards.
- **Abstain.** Take no part in deciding.
- **Safe harbor.** A rule that protects a transaction from challenge when stated conditions are met. Under KRS 273.219(1), a court will not grant equitable relief, such as undoing the transaction, on the ground of the director's interest if an informed board approved it, or if it was fair.
- **Federal recognition.** The IRS's recognition of NTARI as tax-exempt under section 501(c)(3) of the Internal Revenue Code (§14.2).
- **Conflict-of-interest policy.** A written Board policy on how interests are disclosed, judged and recorded.
- **Appendix — Provenance of Demands.** The informative table at the end of the bylaws that names the source of each demand. It is not operative.
- **Conformance suite; B1–B8.** The bylaws repository's own script. Its eight checks test that the text is whole: provisions numbered in order, every section reference pointing at a real section, translations present. It does not check meaning or law.
- **Patch.** A file listing exact line changes, which `git apply` applies to a copy.
- **Schedule P.** One register of every policy, kept as part of the bylaws, which sibling proposal B ([amend-schedule-p](https://github.com/NTARI-RAND/governance-rand/pull/6)) puts forward. It is not part of this proposal.
- **AGPL-3.0.** The GNU Affero General Public License, version 3, the copyleft license the Institute uses for every work it publishes under registry Entry 9.

## The amendment

### §7.4 Action (replace; v1.1 L165)

**Current v1.1 text** ([L165][v11-7.4]; the same words as [v1.0 L157][v10-7.4]):

> **7.4 Action.** The Board acts in meetings, synchronous or asynchronous, on one week's notice to its members, a majority constituting a quorum and a majority of those present deciding. Board proceedings are open to observation by members, and their records are kept under §2.5. The Board holds no recurring meeting requirement: its action may be taken continuously by written consent under KRS 273.375, recorded under §2.5 like any other proceeding.

**Proposed text:**

> **7.4 Action.** The Board acts in meetings, synchronous or asynchronous, on one week's notice to its members, a majority constituting a quorum and a majority of those present deciding. Board proceedings are open to observation by members, and their records are kept under §2.5. The Board holds no recurring meeting requirement: it may act without a meeting only by written consent signed by every director in office, under KRS 273.375, and such consents may be gathered continuously, each recorded under §2.5 like any other proceeding.

Only the last sentence changes. Meetings, notice, quorum and majority stay as they are.

**Why.**

- **It states the rule that applies today.** [KRS 273.375(1)][krs-273.375] reads: "Unless the articles of incorporation or bylaws provide otherwise", Board action without a meeting may be taken "if the action is taken by all members of the board". The written consents must be "signed by each director" and kept with the minutes or corporate records. v1.0 and v1.1 cite the statute and set no other rule, so, unless the articles say otherwise, every director must sign today. The filed articles of incorporation have not been retrieved ([governance-rand#4][pr4]), so whether they say otherwise is unverified.
- **It closes a misreading.** "Continuously" could be taken as a lighter rule, such as a majority of replies gathered in a channel over some days. The new text keeps continuous gathering but says every director signs. Under [KRS 273.375(2)][krs-273.375], the action takes effect when the last director signs, unless the consent names another date.
- **It is a check (§2.2).** Unanimity gives each director a veto over action without a meeting. Any one director can withhold consent and bring the matter to a meeting, which members may observe (§7.4).
- **"Only" is new.** governance-rand#4's tested text read "it may act without a meeting by written consent signed by every director in office". The word "only" is added so that no other way to act without a meeting can be read in.
- **What it does not try.** Whether Kentucky would let the bylaws allow fewer signatures than every director's was not checked. This proposal keeps the default.

### §14.3 Conflicts of interest (replace; v1.1 L371)

**Current v1.1 text** ([L371][v11-14.3]; the same words as [v1.0 L331][v10-14.3]):

> **14.3 Conflicts of interest.** Every director, officer, and delegate discloses any interest they hold in a matter before acting on it, and abstains where the interest conflicts. The Board maintains a conflict-of-interest policy consistent with the Institute's federal recognition; disclosures are recorded under §2.5.

**Proposed text:**

> **14.3 Conflicts of interest.** Every director, officer, and delegate discloses any interest they hold in a matter before acting on it, and abstains where the interest conflicts. A transaction in which a director holds a direct or indirect interest is authorized, approved, or ratified only after disclosure, by a majority of the directors who hold no interest in it, and never by a single director. The Board maintains a conflict-of-interest policy consistent with the Institute's federal recognition; disclosures are recorded under §2.5.

One sentence is added in the middle. The first and last sentences are unchanged.

**Why.**

- **What Kentucky law says.** [KRS 273.219][krs-273.219] protects a conflict-of-interest transaction from equitable relief on the ground of the director's interest if (a) the facts and the interest were disclosed or known to the board, and the board authorized, approved, or ratified it; or (b) it was fair to the corporation. Under subsection (3), approval counts if made "by a majority vote of the directors who do not have a direct or indirect interest", "even if the majority is less than a quorum", "but a transaction may not be authorized, approved, or ratified by a single director". Under subsection (4), the interested director must prove fairness. Subsection (3) also lets the articles or bylaws require "a higher number than a majority", so the statute leaves room for bylaws that ask more.
- **How far the text goes.** Kentucky law does not forbid a single director's approval; it only denies that approval the safe harbor of KRS 273.219(1)(a) (subsection (3)). A transaction approved that way can still stand if the director proves it fair (subsections (1)(b) and (4)). The proposed text forbids it outright, by choice: under the bylaws, a single director cannot approve it at all.
- **Why in the text, not a policy.** A check on the Board must sit where the Board cannot lift it. The Board can change a Board policy. Only the membership can change the bylaws text (§7.5, §15.1). [§2.2][v11-2.2] requires every power to name its check.
- **How the majority is counted.** "A majority of the directors who hold no interest in it" reads as a majority of all such directors in office, not only of those present. That is the drafter's reading; [Question 5](#questions-for-federation-governance) asks whether it is the right one. Either way, at least two disinterested directors must agree.
- **Quorum still applies.** The statute lets the disinterested majority act "even if the majority is less than a quorum" (KRS 273.219(3)). The proposed text does not carry those words. So in a meeting, §7.4's quorum, a majority of the Board, still applies. §7.4 does not say whether an interested director who attends and abstains counts toward the quorum; the drafter reads presence as counting. Either way, interested directors who stay away can leave a meeting without a quorum, and so block approval. With five directors, three interested ones who stay away leave two present, short of the quorum of three. Here the text departs from the statute. [Question 6](#questions-for-federation-governance) asks whether to add the statute's words.
- **Written consent and abstention.** Under the proposed §7.4, action without a meeting needs every director's signature. Under §14.3, the interested director abstains. So, as drafted, a conflicted transaction is decided in a meeting, not by written consent. Whether an interested director may sign a consent while abstaining on the merits is a [question for counsel](#questions-for-counsel).
- **The size of the board today.** §16.1 sets the founder board at three to five directors. How many directors sit today, and which offices they hold, is unconfirmed. So whether a disinterested majority can be formed today is unconfirmed too. With three directors, a matter in which two hold an interest leaves one disinterested director, who may not act alone. Where no disinterested majority can be formed, the matter waits under this text. Other routes are [federation questions](#questions-for-federation-governance): a members' decision, or relying on the director to prove the transaction fair (KRS 273.219(1)(b), (4)).
- **No conflict-of-interest policy has been found.** governance-rand#4's inventory (as reported there; not re-checked here) found none in the Institute's records. One is cited in an earlier bylaws draft, but its text was not found. An earlier one is lost. The policy slot §14.3 calls for is vacant. v1.0 §14.3, in force since 2026-08-31, already says the Board maintains one. Adopting a policy is a separate Board act under §7.4. It is not part of this amendment.
- **What federal recognition asks.** The IRS's [Instructions for Form 1023][irs-i1023] (Rev. December 2024) include a sample conflict-of-interest policy as Appendix A. They say the sample "doesn't prescribe any specific requirements" and that adopting a policy "isn't required to obtain tax-exempt status". The sample is one possible model ([Question 7](#questions-for-federation-governance)).
- **Disclosure is already in use.** Registry Entry 5 records a disclosure under §14.3.
- **A known conflict with §14.5.** §14.5 says the Institute indemnifies its directors, officers, and delegates, and "may purchase insurance for the purpose". Insurance that covers every director gives every director an interest in buying it. The same may hold for an indemnification decision in which every director has the same stake, such as a claim against the whole Board. If such a decision is a transaction in which a director holds a direct or indirect interest, the proposed §14.3 leaves no disinterested director to approve it, and the Board could not use the §14.5 power to buy insurance. Whether it is such a transaction is unverified and is a [question for counsel](#questions-for-counsel). This proposal names the conflict but does not resolve it; [Question 4](#questions-for-federation-governance) offers one possible text.

### Appendix — Provenance of Demands (informative; two rows)

**§7.4 row (replace; v1.1 [L436][v11-app-7.4]).** Current:

> | §7.4 | Continuous board action by written consent | KRS 273.375; P1-001 v8.0 Appendix B (P1-003) |

Proposed:

> | §7.4 | Continuous board action by written consent signed by every director in office | KRS 273.375(1); P1-001 v8.0 Appendix B (P1-003) |

**§14.3 row (new).** v1.1 has no §14.3 row today. The new row goes between the §13.1 row and the §14.7 row ([L476–L477][v11-app-14.7]):

> | §14.3 | Disclosure and abstention; a conflicted transaction authorized, approved, or ratified only after disclosure, by a majority of the directors who hold no interest in it, never by a single director | KRS 273.219(1)(a) and (3), whose safe harbor a single director's approval does not earn; the outright bar goes further by choice; §2.2 (a power names its check) |

**Why.** The appendix names the source of each demand. The §14.3 row adapts governance-rand#4's row to v1.1's format: v1.1's rows name a provision without "(as amended)", and this row also names the disclosure duty and §2.2. The §7.4 row now matches the text it describes.

## How it would be adopted

1. **Notice and deliberation.** This file is research. Merging it adopts nothing. #federation-governance deliberates it through testing, with no deadline.
2. **A bootstrap act.** Only the membership amends the bylaws ([§15.1][v11-15.1]); the Board may not ([§7.5][v11-7.5]). During bootstrap the founder board exercises the membership's powers ([§16.1][v11-16.1]). So adoption would be a §16.1 bootstrap act.
3. **Into v1.1, or a new version file.** The best path is to fold it into the pending v1.1 adoption, which takes effect only by such an act ([v1.1 header][v11-hdr]). If v1.1 is adopted first, the change goes into a new version file, such as v1.2. It is never made by editing v1.0 in place: the bylaws README says an adopted instrument is "never patched" ([README L53–58][readme-53]), and v1.1's header says v1.0 stays in the record unchanged (§2.5).
4. **Recorded in the registry, with signed consents.** The act is recorded under §9.5 in the registry of record. It should carry the signed consents counsel confirms: every director in office under KRS 273.375, the rule this proposal writes down; or every member entitled to vote under [KRS 273.377][krs-273.377], if counsel finds that test applies to acts taken with the membership's powers. [KRS 273.201(4)][krs-273.201] bears on the choice: "If a corporation has no members or its members have no right to vote, the directors shall have the sole voting power." The registry records no recognition of a member under §3.3, so whether the Institute has any member entitled to vote is unverified. If it has none, every director's consent under KRS 273.375 may be the test even for acts taken with the membership's powers. Counsel should confirm.
5. **Translations.** The seven v1.1 translations (Arabic, Spanish, French, Hindi, Portuguese, toki pona and Chinese) each carry §7.4, §14.3 and the §7.4 appendix row. On adoption, each must be updated to match, and the §14.3 row added. Suite check B7 only checks that the files exist, not what they say ([CONTRIBUTING L93–98][contrib-93]). The bylaws repository's contributing guide treats the English text as authoritative; sibling B proposes writing that rule into §14.8.
6. **Open afterwards.** Like every bootstrap act, the adoption stands open to the membership under [§2.3][v11-2.3].
7. **The policy is a separate act.** Adopting a conflict-of-interest policy is a Board act under §7.4, taken by the founder board serving as the Board (§7.2). It is not a bylaws amendment.

## What this proposal does not decide

- **Whether past acts met Kentucky's consent rules.** No registry entry records a meeting vote or a consent signed by every director. Registry Entries 3, 4, 5 and 6 name their decider as the President, "for the founder board". Entry 7 is an annotation of Entry 6; it names no decider and rests on the act Entry 6 records. Entry 8 names the President alone, acting as the office of §8.2, with §16.1 because no federation has yet elected that office. Entries 9 and 10, of 2026-11-13, use the same "for the founder board" form as Entries 3–6; Entry 9 is recorded as a Board act amending a Board policy, Entry 10 as a bootstrap act. Entries 1 and 2 record acts of the founder board and name no decider. Whether those acts meet KRS 273.375, or KRS 273.377 where the founder board used the membership's powers, is unverified. Which test applies may turn on KRS 273.201(4) and on whether the Institute has any member entitled to vote, which is also unverified. It is a question for counsel. The bylaws say bootstrap acts remain valid and stay open under §2.3 (§16.1); whether Kentucky law agrees is part of the same question. This amendment does not settle it: it states a rule for acts taken after adoption. Raising the question is not an accusation.
- **The founder board's size, and who holds which office.** Unconfirmed.
- **The conflict with §14.5.** If insurance under §14.5 that covers every director, or an indemnification decision in which every director has the same stake, counts as a transaction in which a director holds an interest, the proposed §14.3 would stop the Board from deciding it. This is a known conflict in the amended text. It is left open, not fixed.
- **The quorum.** The text keeps §7.4's quorum for conflicted transactions decided in a meeting, unlike KRS 273.219(3). Whether to add the statute's "even if less than a quorum" rule is left to the federation.
- **Other routes when no disinterested majority can be formed.** The text makes the matter wait. A members' decision, or reliance on fairness, would need a further amendment.
- **The content of the conflict-of-interest policy,** who drafts it, or when the Board adopts it.
- **Whether an "asynchronous" meeting is a meeting.** [KRS 273.217(2)][krs-273.217] lets directors take part in a meeting from a distance by means through which they "may simultaneously communicate with each other". Whether §7.4's asynchronous meetings meet that test is unverified. If they do not, asynchronous Board action may be valid only as a written consent every director signs. This proposal leaves the words "synchronous or asynchronous" as they are.
- **What counts as a signature.** Chapter 273 counts an electronic signature as a signature ([KRS 273.161(21)][krs-273.161]). Whether a director's message in a chat channel is a signed written consent "describing the action taken", filed as KRS 273.375(1) requires, is unverified (see [Questions for counsel](#questions-for-counsel)).
- **Exact definitions.** The text does not tie "transaction" or "direct or indirect interest" to KRS 273.219's definitions.
- **The articles of incorporation.** They were not retrieved. Where an article is inconsistent with a bylaw, the article controls ([KRS 273.247(4)][krs-273.247]). Whether the articles say anything on Board consent or conflicts is unverified.
- **Members' action without a meeting** ([KRS 273.377][krs-273.377]). Unchanged.

## How it fits the other amendment proposals

Three proposals are filed together. Each is meant to be adoptable on its own. This one, C, depends on neither A nor B.

- **(A) [amend-9.4-licensing-floor](https://github.com/NTARI-RAND/governance-rand/pull/5).** No shared sections. A changes §9.4 and its appendix row (v1.1 L197 and L441). C's appendix change at L436 sits five lines above A's row, so the two patches share context lines, but no line is changed by both. Tested on 2026-11-13 in both orders on fresh copies of `3276781`: both patches apply with a plain `git apply`, and the suite passes all checks: 108 provisions, 320 references (89 distinct).
- **(B) [amend-schedule-p](https://github.com/NTARI-RAND/governance-rand/pull/6).** Three points.
  - **The policy slot.** If B is adopted, the conflict-of-interest policy §14.3 requires is the class (b) slot that B's §14.9 names. §14.3 therefore needs no words about Schedule P. B does not change §14.3.
  - **Wording that relies on §7.4.** B's §14.10 has the Board enter board policies "by action under §7.4", and its §16.4 has the founder board take those acts "under §7.4 as the Board". Under C, each such act needs a meeting or a consent every director signs. The wordings do not conflict; C states what B's acts need.
  - **Neighbouring lines.** B changes §7.5 (v1.1 L167), two lines below this proposal's §7.4 (L165), and adds appendix rows just after the §14.7 row, where this proposal's §14.3 row goes just before it. Applied one after the other, the second patch fails a plain `git apply`. Stage the first (`git add -A`) and apply the second with `git apply --3way`; without staging, `--3way` stops with "does not match index". The texts themselves do not conflict. Tested in both orders on 2026-11-13: 112 provisions, 369 references (94 distinct), all checks PASS.
- **All three together.** Tested on 2026-11-13 in all six orders of A, B and C on fresh copies of `3276781`. A and C apply to each other with a plain `git apply`. B applied after A or C, and any patch applied after B, needs `git apply --3way`, after the earlier changes are staged. Every order gave a byte-identical result with no conflict markers, and the suite passes all checks: 112 provisions, 372 references (94 distinct).
- **governance-rand#4.** That note carries the same two texts written against v1.0. This proposal is their v1.1 form, without the Schedule P clause. Adopt from one or the other, not both.

## Test it yourself

Clone governance-rand with `git clone -c core.autocrlf=false https://github.com/NTARI-RAND/governance-rand.git` and check out the pull request that adds this file. Without that flag, git on Windows rewrites the patch's line endings and `git apply` fails ("patch does not apply"); a copy with Windows line endings failed this way when tested. `path/to/governance-rand` below is that clone.

```
git clone https://github.com/NTARI-RAND/bylaws.git
cd bylaws
git checkout 3276781
git apply --check path/to/governance-rand/tier-1-bylaws/amend-board-consent-and-conflicts.v1.1.patch
git apply path/to/governance-rand/tier-1-bylaws/amend-board-consent-and-conflicts.v1.1.patch
python bylaws-conformance-suite.py --doc P1-001_Bylaws_v1.1.md
git diff --word-diff
```

On Windows, if the suite stops on a text-encoding error, run it as `python -X utf8 bylaws-conformance-suite.py --doc P1-001_Bylaws_v1.1.md`.

## Test results

Run on 2026-11-13 on a fresh copy of NTARI-RAND/bylaws at `3276781`, after `git apply --check` and `git apply` succeeded, with `python -X utf8 -I bylaws-conformance-suite.py --doc P1-001_Bylaws_v1.1.md`:

```
Bylaws conformance: P1-001_Bylaws_v1.1.md
-----------------------------------------
[PASS] B1 preamble, sixteen articles in order, appendix
[PASS] B2 provisions numbered 1..n inside each article -- 108 provisions across 16 articles
[PASS] B3 every section cross reference resolves -- 317 references, 89 distinct, all resolve
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

Unpatched, v1.1 gives 315 references, 88 distinct. The two new references are §14.3 and §2.2 in the new appendix row. The provision count does not change, because no section is added. `git diff --stat` shows one file changed, 4 insertions and 3 deletions. For the results with sibling proposals A and B, see [How it fits the other amendment proposals](#how-it-fits-the-other-amendment-proposals).

## Questions for #federation-governance

The federation decides these, with no deadline.

1. Should a single director's approval of a conflicted transaction be barred outright, going beyond KRS 273.219?
2. If no disinterested majority of directors can be formed, should the matter wait (the proposed text), go to a members' decision, or rest on the director proving it fair (KRS 273.219(1)(b), (4))? During bootstrap, a members' decision would be taken by the same founder board under §16.1, so it adds no independent check until federations elect.
3. How many directors sit on the founder board today, and which offices do they hold? The disinterested majority of §14.3 and the consents of §7.4 depend on it.
4. Some matters may touch every director alike, such as the insurance §14.5 allows. As drafted, no disinterested majority could approve them. Should such matters be named and given another route? One possible text, untested: "A matter in which every director holds the same interest, such as indemnification or insurance under §14.5, is decided by the Board after disclosure."
5. Should the disinterested majority be counted among all such directors in office (the drafter's reading), or among those present at a meeting?
6. Should §14.3 add the statute's quorum rule, so that the disinterested majority may act "even if they are fewer than a quorum" (KRS 273.219(3))? Without it, interested directors who stay away can block approval.
7. Who drafts the conflict-of-interest policy, and from what model? The IRS sample in Appendix A of the Form 1023 instructions is one option. No draft exists.
8. Where should written consents be gathered and kept, so that each director's signature can be found from the registry entry that records the act?

## Questions for counsel

1. Do registry Entries 3–6 and 10, recorded as acts "for the founder board", meet KRS 273.375, or KRS 273.377 where the founder board used the membership's powers? Entry 7 only records that Entry 6 took effect. Entry 8 is a reading by the office of the President under §8.2 and §16.1: did it need the founder board's consent at all? Entry 9 is recorded as a Board act: does it meet KRS 273.375? Entries 1 and 2 record acts of the founder board, name no decider and record no consent: does the same question apply to them?
2. Which consent test applies to a bootstrap act? While no member entitled to vote has been recognized, does [KRS 273.201(4)][krs-273.201] ("If a corporation has no members or its members have no right to vote, the directors shall have the sole voting power") give the directors sole voting power, making KRS 273.375 (every director) the test for bootstrap acts? Whether any voting member exists is unverified; the registry records no recognition under §3.3.
3. Does a director's message in a chat channel count as a signed written consent under KRS 273.375? Chapter 273 itself says "'Sign' or 'signature' includes any manual, facsimile, or conformed or electronic signature" ([KRS 273.161(21)][krs-273.161]), so an electronic signature counts. That narrows the question. Is a chat message, made with the intent to sign, a signature on a written consent "describing the action taken"? Is that record "included in the minutes or filed with the corporate records" (KRS 273.375(1))? The Uniform Electronic Transactions Act may guide what shows intent: it defines an electronic signature as one made "with the intent to sign the record" ([KRS 369.102(8)][krs-369.102]). But that act covers only records and signatures "relating to a transaction" ([KRS 369.103(1)][krs-369.103]), so Chapter 273's own definition is the firmer ground.
4. Is an "asynchronous" meeting under §7.4 a meeting under KRS 273.217(2)? If not, is every asynchronous Board action valid only as a written consent every director signs?
5. May an interested director sign a written consent under KRS 273.375 while abstaining under §14.3? If not, are conflicted transactions decided only in meetings?
6. Is buying insurance under §14.5 that covers every director, or an indemnification decision in which every director has the same stake, a transaction "in which a director of the corporation has a direct or indirect interest" under KRS 273.219(1)? If so, how may the Board decide it under the proposed §14.3?
7. Should §14.3 tie "transaction" and "direct or indirect interest" to KRS 273.219's definitions?
8. Do the filed articles of incorporation say anything about Board action without a meeting or conflicts of interest?

## Method and ethics

Claude (Anthropic) drafted this proposal at the direction of the author, as one of three sibling proposals.

- **Starting point.** The tested §7.4 and §14.3 texts of governance-rand#4, written against v1.0 line numbers, and that note's provenance row, inventory, open points and questions.
- **Adapted to v1.1.** v1.1's §7.4 and §14.3 were confirmed to be word for word the same as v1.0's. §14.3 drops the note's Schedule P clause. §7.4 adds the word "only". The appendix row follows v1.1's format, and the §7.4 row is updated to match.
- **Applied and tested.** A script made each change in a scratch copy of NTARI-RAND/bylaws at `3276781`, asserting that each target text occurs exactly once. The repository's own suite passed B1–B8. The patch was made with `git diff`, then checked with `git apply --check`, applied with `git apply` to a fresh copy, and tested again. It was also applied with sibling patches A and B in every order, and a copy with Windows line endings was tried, to confirm the warning in the test steps.
- **Reviewed.** Separate verification passes read the draft against the bylaws, the registry and the statutes. Each finding was checked against those sources before it was applied or answered. The bylaws text in the patch did not change in review; the explanations, questions and test notes did.
- **Sources read.** KRS 273.161, 273.201, 273.217, 273.219, 273.247, 273.375 and 273.377, and KRS 369.102, 369.103 and 369.107, read on 2026-11-13 from the Kentucky Legislature's site. The IRS Instructions for Form 1023 (Rev. December 2024), read from irs.gov. The governance registry, Entries 1–10, read from a copy byte-identical to the registry of record.
- **What ran.** Only the bylaws repository's own conformance suite, git, and the drafting and test scripts. No code from outside contributors was run.
- **Read-only while drafting.** Nothing was posted, pushed, commented or edited in any repository or channel until this pull request was opened.
- **Personal data.** None. The proposal names offices, never people, apart from the author line. Statute and IRS quotations are short.

Much of this text was drafted by a tool. The choices it recommends are the author's to propose and the federation's to test.

[pr4]: https://github.com/NTARI-RAND/governance-rand/pull/4
[registry]: https://github.com/NTARI-RAND/governance-registry/blob/main/GOVERNANCE-REGISTRY.md
[v11-hdr]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L3-L5
[v11-2.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L43
[v11-2.3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L45
[v11-7.2]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L161
[v11-7.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L165
[v11-7.5]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L167
[v11-14.3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L371
[v11-15.1]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L385
[v11-16.1]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L395
[v11-app-7.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L436
[v11-app-14.7]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.1.md?plain=1#L476-L477
[v10-7.4]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L157
[v10-14.3]: https://github.com/NTARI-RAND/bylaws/blob/3276781/P1-001_Bylaws_v1.0.md?plain=1#L331
[readme-53]: https://github.com/NTARI-RAND/bylaws/blob/3276781/README.md?plain=1#L53-L58
[contrib-93]: https://github.com/NTARI-RAND/bylaws/blob/3276781/CONTRIBUTING.md?plain=1#L93-L98
[krs-273.161]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=49017
[krs-273.201]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=13627
[krs-273.217]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=48305
[krs-273.219]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=48304
[krs-273.247]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=36676
[krs-273.375]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44380
[krs-273.377]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44388
[krs-369.102]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=44375
[krs-369.103]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=49526
[krs-369.107]: https://apps.legislature.ky.gov/law/statutes/statute.aspx?id=35206
[irs-i1023]: https://www.irs.gov/pub/irs-pdf/i1023.pdf

---

*Licensed under the [GNU Affero General Public License, version 3](https://www.gnu.org/licenses/agpl-3.0.txt) (AGPL-3.0), under governance registry Entry 9. This repository's LICENSE file still reads GPL-3.0 until it is relicensed under the same entry.*
