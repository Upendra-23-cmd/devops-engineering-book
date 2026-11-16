# Editorial Guidelines

**Version:** 0.1.0 · **Last updated:** 2026-11-14

These rules implement Parts 3, 4, 7, 10, 12 and 13 of the master prompt. If this file and the master prompt disagree, the master prompt wins and this file must be corrected.

## 1. Language, style, and evidence labels

- **British English** (virtualisation, behaviour, organisation). Product and tool names keep their official spelling.
- **ISO 8601 dates** (`YYYY-MM-DD`). All timestamps are **UTC** unless stated.
- Define every abbreviation at first use in each chapter and add it to [`GLOSSARY.md`](GLOSSARY.md).
- Explain every command and configuration block: its purpose, each non-obvious option, the expected result, and the risk.
- Prefer prose under numbered headings. Use tables for comparisons and diagrams where structure matters. No padding: never lengthen a chapter to raise the page count.
- **Separate three kinds of statement** wherever they could be confused:
  - **Fact**: verified against a primary source or against captured evidence.
  - **Assumption**: needed to proceed but not verified.
  - **Recommendation**: engineering judgement, with the trade-off stated.
- Illustrative numbers (for example, a worked queueing example) must be labelled *illustrative*. They are never presented as measurements.

## 2. Hierarchy, numbering, and identifiers

Hierarchy: Book → Part → Chapter → Section → Subsection (concept) → Concept part. Every concept ends with a laboratory.

| Object | Identifier | Example | Rule |
|---|---|---|---|
| Part | `P01`–`P17` | `P02` | Fixed. |
| Chapter | `CH-001`–`CH-118` | `CH-005` | Assigned once, never reused. The printed number follows book order and may change before the publication freeze; **cross-reference by ID**. |
| Section | `<chapter>.<n>` | `5.2` | One per curriculum topic. |
| Concept | `<section>.<n>` | `5.2.1` | One laboratory each. |
| Concept part | `<concept>.<1–6>` | `5.2.1.3` | See §5. |
| Laboratory | `LAB-<chapter, 3 digits>-<nn>` | `LAB-005-02` | File in `labs/ch-005/`. |
| Baseline assessment | `BASE-nn` | `BASE-01` | Placement and verification of existing skills. |
| Integrated assessment | `IA-<section>` | `IA-5.2` | Closes every section. |
| Part practical review | `PR-P<nn>` | `PR-P02` | Closes every part. |
| Flagship project | `PRJ-<nn>[A–C]` | `PRJ-04B` | Increments are explained in `projects/PORTFOLIO.md`. |
| Professional engineering review | `PER-PRJ-<nn>` | `PER-PRJ-03` | Closes every flagship project. |
| Case study | `CS-<nn>` | `CS-02` | Requires learner-supplied evidence. |
| Incident intake record | `INC-AD-<nnn>` | `INC-AD-001` | AirDive evidence register. |
| Figure / diagram | `FIG-<nnn>` | `FIG-001` | Source is Mermaid text. |
| Architecture Decision Record | `ADR-<nnnn>` | `ADR-0001` | Per project. |
| Programme decision | `D-<nnn>` | `D-004` | Logged in `BOOK_PLAN.md`. |

## 3. Chapter template: 24 mandatory components

Every chapter contains all 24 components of the master prompt. If one does not apply, the chapter says **why** it does not apply; it never carries meaningless filler. The skeleton is in [`chapters/_templates/CHAPTER_TEMPLATE.md`](chapters/_templates/CHAPTER_TEMPLATE.md).

| # | Component | Heading in the chapter file |
|---|---|---|
| 1 | Chapter title and number | `# Chapter N — Title` and metadata block |
| 2 | Chapter introduction | `## Chapter introduction` |
| 3 | Why the topic matters in professional engineering | `## Why this matters in professional engineering` |
| 4 | Prerequisites | `## Prerequisites` |
| 5 | Learning objectives | `## Learning objectives` |
| 6 | Detailed table of contents for the chapter | `## Chapter contents` |
| 7 | Foundational technical explanation | `## Chapter foundations` → `### Foundational technical explanation` |
| 8 | Internal architecture and working mechanisms | `### Internal architecture and working mechanisms` |
| 9 | Every concept broken into numbered sections | `## x.y Section` → `### x.y.z Concept` |
| 10 | Workplace scenarios | Concept part `.2` (plus a chapter-level set if needed) |
| 11 | Practical labs after every concept | Concept part `.3` and the lab files |
| 12 | Controlled failure simulations | Concept part `.4` and `## Integrated failure simulations` |
| 13 | Troubleshooting exercises | Concept part `.5` and `## Integrated troubleshooting exercises` |
| 14 | Real-world case studies | `## Real-world case studies` |
| 15 | Security and reliability considerations | `## Security and reliability considerations` |
| 16 | Senior engineer perspective | `## Senior engineer perspective` |
| 17 | Architect perspective | `## Architect perspective` |
| 18 | Chapter-level integrated project | `## Integrated chapter project` |
| 19 | Production-readiness checklist | `## Production-readiness checklist` |
| 20 | Chapter assessment | `## Chapter assessment` |
| 21 | Practical competency assessment | `## Practical competency assessment` |
| 22 | Chapter summary | `## Chapter summary` |
| 23 | Glossary additions | `## Glossary additions` |
| 24 | References | `## References` |

Each chapter file starts with a metadata block (ID, part, status, version, last updated, labs, prerequisites) and a **version baseline** table (tool, version, date checked, source) for every versioned technology the chapter uses.

## 4. Section close-out

Every numbered section `x.y` ends with an **Integrated assessment** (`IA-x.y`): questions that combine its concepts, plus one practical task that cannot be completed by recalling any single concept.

## 5. Concept template: six parts

Every concept (`x.y.z`) has the same six parts, which implements the 15-step practical sequence of the master prompt.

1. **Concept explanation**: what it is; why it exists; internal working; architecture; how it is used in real engineering environments.
2. **Workplace scenario**: written as an engineering ticket (context, responsibilities, constraints). Illustrative scenarios are labelled as such; evidence about AirDive is never invented.
3. **Practical laboratory**: a link to the lab file. The learner creates or configures the component and verifies its behaviour.
4. **Failure simulation**: a controlled failure the learner investigates. Where no system can be damaged (for example, a process or measurement topic), the simulation breaks the *method* or the *evidence*, and the section says so.
5. **Troubleshooting and verification**: how to diagnose from evidence and how to prove the repair worked.
6. **Prevention, improvement, and checkpoint**: architectural improvements, plus checkpoint questions whose answers are **not** stored in the repository.

## 6. Laboratory rules

- Every lab uses [`labs/_templates/LAB_TEMPLATE.md`](labs/_templates/LAB_TEMPLATE.md) (21 mandatory fields).
- **Assessment mode is the default.** A lab states the scenario, requirements, constraints, and acceptance criteria. It does not state the commands to run or the root cause.
- **Hint ladder.** Hints are released progressively and recorded, because assisted work scores lower:

  | Level | Hint | Effect on assessment |
  |---|---|---|
  | H0 | None. Record your hypothesis first. | Full credit |
  | H1 | A question that redirects attention (no tool names). | Full credit |
  | H2 | The diagnostic area or tool family. | Minor deduction |
  | H3 | A specific command or query and what to look for. | Moderate deduction |
  | H4 | A full walkthrough. | Recorded as *assisted* |

- **Lab phases.** Phase 1 *Build and verify* → Phase 2 *Break* (mentor-released; its contents are deliberately not in the lab file) → Phase 3 *Diagnose and recover* → Phase 4 *Prevent and assess*.
- **Lab gates.** `Drafted` → `Dry-run` (the author executed it in a disposable environment, or piloted an analysis lab on synthetic data) → `Learner-run` → `Accepted` (acceptance criteria met and reviewed).
- Answer keys, root causes of injected failures, and checkpoint answers are held by the mentor and are **not committed**.

## 7. Failure injection and safety

These rules implement §4.5 of the master prompt and are not negotiable.

- Failure injection happens only in **isolated or disposable** environments.
- **Never** deliberately damage live AirDive infrastructure, production databases, real DNS records, customer-facing systems, or important data. AirDive production is touched only read-only, and only for evidence gathering, with the owner's explicit approval.
- Before any risky operation the lab states **cost, risk, backup requirement, and recovery procedure**, plus the teardown that stops billing.
- Cloud labs begin by setting a budget alert. Free-tier terms and prices are verified against current AWS documentation at the point of use; they are never quoted from memory.
- Every lab has a **cleanup procedure**, and the learner confirms it ran.
- No secrets, tokens, private keys, customer data, or internal addresses are pasted into chat, commits, or evidence files. Redact first.

## 8. Troubleshooting protocol

Teach evidence-driven diagnosis. Random command execution is not rewarded.

1. State the **symptom** precisely (what, where, since when, what changed).
2. List the **evidence** collected so far and its source.
3. Write **ranked hypotheses**.
4. For each next step: *which* diagnostic, *what* you expect it to show, and *what result would falsify* the hypothesis.
5. Record the result and update the hypotheses.
6. State the **root cause** only when evidence supports it.
7. **Fix**, then **verify** with a check independent of the fix.
8. Record **prevention**.

## 9. Technical accuracy

- **Sources.** Prefer primary documentation (vendor documentation, standards and RFCs, original papers). Record every source in [`REFERENCES.md`](REFERENCES.md) with its **verification level**: *Primary, read in full*; *Primary, excerpt only*; *Secondary only*. Do not cite a source that has not been opened. Never fabricate a source, a quotation, or a result.
- **Quotation.** Paraphrase. Quote only short phrases where the exact wording matters, and attribute them.
- **Versions.** Pin versions at the point of use. Re-verify them against primary documentation before a chapter is marked *Practically validated*. Explain important version differences.
- **Commands and configuration.** Commands are either executed by the author (and recorded with environment, version, and date) or labelled **Not yet executed**.
- **Command output.** Output blocks are labelled **Captured** (from a recorded run, with environment and date) or **Illustrative** (shape only). Illustrative output never contains realistic-looking performance numbers.
- **Performance numbers, availability percentages, and test results** come only from recorded runs.

## 10. Diagrams

- Mermaid in Markdown (`mermaid` fenced blocks), so diagram source is version-controlled. Shared diagrams live in [`diagrams/`](diagrams/) with a `FIG-nnn` ID; chapter-specific diagrams are inline.
- Quote node labels (`A["Label"]`), give every diagram a caption and an ID, and keep secrets and real hostnames out of diagrams.

## 11. AirDive evidence handling

- Facts require **evidence** (log lines, commit SHAs, build numbers, configuration diffs, timestamps) recorded in an incident intake record.
- Statements that rest on memory only are labelled **Recollection (unverified)**.
- Every case study keeps three separate sections: **Verified facts**, **Hypotheses**, **Proposed solutions**.
- AirDive is used for evidence and case studies. Failure injection uses the reference application ([`BOOK_PLAN.md`](BOOK_PLAN.md), decision D-004), never AirDive production.

## 12. Review and status workflow

Chapter status, in order: **Planned → Drafted → Practically validated → Technically reviewed → Editorially reviewed → Finalised.** A chapter is never marked *Finalised* because the prose is complete. Each transition needs evidence, recorded in [`PROGRESS.md`](PROGRESS.md) and [`CHANGELOG.md`](CHANGELOG.md).

A chapter that is only partly written stays **Planned** and shows its drafting progress separately.

| Review | Questions that must be answered *yes* with evidence |
|---|---|
| Technical correctness | Are explanations accurate? Are commands valid? Are configurations complete? Are versions compatible? Are security practices appropriate? |
| Practical quality | Is the lab executable? Are prerequisites sufficient? Are expected results defined? Can the failure be reproduced? Was the recovery process tested? |
| Educational quality | Does it build progressively? Does it connect concepts? Does every concept have practical work? Does it develop independent reasoning? |
| Architecture quality | Are trade-offs explained? Are failure domains identified? Are security and reliability considered? Are cost and operational complexity evaluated? |
| Publication quality | Are headings and numbering consistent? Are diagrams readable? Are references accurate and cross-references correct? Is repetition removed? |

## 13. Changing the manuscript

- One logical change per commit once the repository is under version control; use pull requests for anything that changes a chapter's status.
- Record every material change in [`CHANGELOG.md`](CHANGELOG.md). If a technical error is found, correct it, note the correction, and update every affected chapter.
