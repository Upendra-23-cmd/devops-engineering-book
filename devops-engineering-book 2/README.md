# The Practical DevOps Engineer

*From Linux Fundamentals to Enterprise Cloud Infrastructure, Platform Engineering, and DevOps Architecture*

A textbook, enterprise engineering laboratory, and portfolio programme. The manuscript is plain Markdown and is the **source of truth**; any PDF is generated from it later and is never the editable source.

> **Status (2026-11-16, version 0.2.0).** Scaffold complete. Chapter 1 is in drafting (front matter and concepts 1.1.1–1.1.2). **No chapter has been practically validated, no lab has been run, and no skill has been verified yet.** Treat everything here as a draft until its status says otherwise.

## What this is, and what it is not

- It is a structured programme to develop an engineer who can build, operate, break, diagnose, recover, automate, and design infrastructure, and who can defend those decisions.
- It produces **evidence of ability**: tested labs, documented projects, recovery records, and a defended portfolio.
- It is **not** a guarantee of employment, and it does not describe you as senior. Skills start as *claimed — unverified* and are assessed honestly.

## Where to start

1. Read [`BOOK_PLAN.md`](BOOK_PLAN.md) (about 10 minutes).
2. Take [`labs/diagnostic/BASE-01-baseline-assessment.md`](labs/diagnostic/BASE-01-baseline-assessment.md): closed-book, about two hours.
3. Read concept 1.1.1 in [`chapters/part-01-devops-foundations/ch-001-from-silos-to-devops.md`](chapters/part-01-devops-foundations/ch-001-from-silos-to-devops.md), then do Phase 1 of [`labs/ch-001/LAB-001-01-value-stream-map.md`](labs/ch-001/LAB-001-01-value-stream-map.md).
4. Then read concept 1.1.2 and do Phase 1 of [`labs/ch-001/LAB-001-02-handoff-chain-reconstruction.md`](labs/ch-001/LAB-001-02-handoff-chain-reconstruction.md), which reuses your first lab's data.

## Key files

| File | Purpose |
|---|---|
| [`BOOK_PLAN.md`](BOOK_PLAN.md) | Objectives, starting position, roadmap and gates, policies, decision log |
| [`TABLE_OF_CONTENTS.md`](TABLE_OF_CONTENTS.md) | 17 parts, 118 chapters, 291 sections |
| [`EDITORIAL_GUIDELINES.md`](EDITORIAL_GUIDELINES.md) | Templates, identifiers, lab rules, safety, evidence rules, review workflow |
| [`PROGRESS.md`](PROGRESS.md) | Six separate progress tracks and the chapter register |
| [`GLOSSARY.md`](GLOSSARY.md) · [`REFERENCES.md`](REFERENCES.md) · [`CHANGELOG.md`](CHANGELOG.md) | Terms, verified sources, history |
| [`projects/PORTFOLIO.md`](projects/PORTFOLIO.md) | Eight projects (twelve increments), quality standard, gates |
| [`case-studies/README.md`](case-studies/README.md) | AirDive case-study rules and subject register |

## Layout

```text
devops-engineering-book/
  README.md  BOOK_PLAN.md  TABLE_OF_CONTENTS.md  EDITORIAL_GUIDELINES.md
  PROGRESS.md  GLOSSARY.md  REFERENCES.md  CHANGELOG.md
  chapters/       one Markdown file per chapter; _templates/
  labs/           one file per substantial lab, in labs/ch-NNN/; diagnostic/; _templates/
  projects/       PORTFOLIO.md; one folder per flagship project as it starts; _templates/
  case-studies/   rules, subject register, incident intake template
  diagrams/       shared Mermaid diagrams (FIG-nnn)
  appendices/     planned appendices
  publication/    export plan (PDF and other formats, after editorial review)
```

## How learning works here

Every concept follows the same loop: **teach → build → verify → break → diagnose → recover → prevent → assess**. Labs run in *assessment mode*: the scenario, requirements, constraints, and acceptance criteria are given; commands and root causes are not. Hints are released on a ladder (H0–H4) and recorded. Details: [`EDITORIAL_GUIDELINES.md`](EDITORIAL_GUIDELINES.md) §5–§8.

## Rules of engagement (non-negotiable)

- **Never** damage live AirDive infrastructure, production databases, real DNS records, customer-facing systems, or important data. Failure injection happens only in isolated or disposable environments.
- **Never** paste secrets, tokens, private keys, customer data, or internal hostnames or addresses into chat, commits, or evidence files. Redact first.
- Cost, risk, backup, and recovery are stated before any risky or billable step, and every lab ends with a cleanup you confirm.
- Nothing is invented: no sources, command output, performance figures, or test results. Output is labelled *Captured* or *Illustrative*.

## Conventions

British English · ISO 8601 dates · UTC timestamps · permanent chapter IDs (`CH-001`…) · diagrams in Mermaid · Markdown with relative links, so the repository works on any git host.
