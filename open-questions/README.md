# Open questions

This folder holds the questions that research in governance-rand has not answered yet. Each question is one Markdown file. Together, the files are the repository's list of open questions. The list is kept up to date.

## What it is for

Research finds gaps as well as answers. A record may be missing, two sources may disagree, or a question may need a lawyer or NTARI's board to answer it. Writing the gap down keeps it from being lost. Then the next researcher, a lawyer or NTARI's board can work on it. A clear gap is a useful result.

The Janus Facing Architecture (JFA) asks every JFA project to keep a list like this one, and to keep it up to date. See the [concept triage](https://github.com/NTARI-RAND/Janus/blob/main/jfa-concept-triage-2026-08-24.md) and [Janus's own list](https://github.com/NTARI-RAND/Janus/blob/main/OPEN-QUESTIONS.md). A question leaves the list only when it is resolved, or when the people who live with the outcome make an explicit decision about it. If this list is out of date, the repository no longer tells the truth about what is known. Check this folder whenever you send a pull request.

## Adding a question

1. Check that the question is not already here. If it is, add what you found to that file instead. Write it under **What was checked**, with your name and the date.
2. Create a new file in this folder. Start the file name with the tier, then add a few words from the question. Use only lowercase letters a to z, digits and hyphens. For example: `tier-1-first-annual-report.md`.
3. Copy the template below into the file, and fill in every heading.
4. Send the file in a pull request with a DCO sign-off. Use the same steps as for other research (see [How we research](../README.md#how-we-research)), but put the file in this folder, not in a tier folder.

Write in plain English. This repository is public, and deleting a file later does not remove it from the history. Never include home addresses, personal phone numbers or emails, handwritten signatures, dates of birth, personal ID numbers (such as passport numbers), bank details or donor names. NTARI's own numbers, such as its EIN, are safe to include.

## Template

```markdown
# The question, in one sentence

**Status:** open

**Asked by:** your name, YYYY-MM-DD

**Tier:** 1 (Bylaws), 2 (JFA adherence) or 3 (Governance platform)

## Why it matters

One or two sentences: what depends on the answer.

## What was checked

Each source you checked and what it showed, with its link. If the source is
in your evidence log, also give the log's path and the ID, for example
tier-1-bylaws/your-name/evidence-log.csv, E003. Also say what you looked for
and did not find.

## Constraints inherited

The rules any answer must respect, such as bylaws sections, governance
registry entries, the JFA's Lines That Cannot Be Crossed, or laws.
Write "None known" if there are none.

## Who might answer

For example: a Kentucky attorney, NTARI's board, or the Kentucky Secretary of State.

## Resolution

Leave this empty while the question is open.
```

## When a question is answered

Update its file in a pull request. Set **Status** to `resolved (YYYY-MM-DD)`, and write the answer under **Resolution**, with its evidence and links. Keep the file. The list keeps its history.

A question can also leave the list without an answer. This needs an explicit decision by the people who live with the outcome, such as NTARI's board or a vote in #federation-governance. The person who asked the question cannot close it alone. Set **Status** to `closed (YYYY-MM-DD)`. Under **Resolution**, write who decided, what they decided and why, with a link to where the decision is recorded, such as a governance registry entry.
