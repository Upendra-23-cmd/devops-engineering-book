# Book Plan

**Book:** The Practical DevOps Engineer · **Version:** 0.1.0 · **Last updated:** 2026-11-14

## 1. Purpose and graduation outcome

The programme exists to develop an engineer who can build infrastructure from nothing, operate complex systems, deliberately reproduce failures, diagnose problems from evidence, recover services, automate delivery, design secure and reliable platforms, and defend architecture decisions.

Completing it produces **credible evidence of engineering ability**: tested labs, documented projects, recovery records, and a defended portfolio. It does not guarantee employment, and no document in this repository claims that it does.

Graduation requirements are in [§12](#12-graduation).

## 2. Starting position (evidence-based)

**What this plan knows about you.** Only what the master prompt states. It does not hold your AirDive incident history, configurations, team size, scale, or your lab hardware, so none of your skills has been **verified**.

**Status of every skill below: *Claimed — unverified*.** Placement comes from [`BASE-01`](labs/diagnostic/BASE-01-baseline-assessment.md), the first lab, and the challenge labs in each part.

| Area | Self-reported exposure | Status | First verification |
|---|---|---|---|
| Linux | Practical exposure | Claimed — unverified | BASE-01 Q5, Q15; Part II |
| Git and GitHub | Practical exposure | Claimed — unverified | BASE-01 Q11; Part IV |
| AWS EC2 and S3 | Practical exposure | Claimed — unverified | BASE-01 Q4, Q8, Q12; Part VI |
| Docker and Compose | Practical exposure | Claimed — unverified | BASE-01 Q1, Q2, Q6, Q7, Q8; Part V |
| Jenkins and CI/CD | Practical exposure | Claimed — unverified | BASE-01 Q9; LAB-001-01; Part VIII |
| GitHub Container Registry | Practical exposure | Claimed — unverified | Not probed by BASE-01; Chapter 35 and PRJ-04A |
| Nginx, DNS, TLS | Practical exposure | Claimed — unverified | BASE-01 Q3, Q13; Parts III, IX |
| Node.js and TypeScript deployments | Practical exposure | Claimed — unverified | BASE-01 Q3, Q6 |
| PostgreSQL and Redis | Practical exposure | Claimed — unverified | BASE-01 Q14 (PostgreSQL only); Part X, Redis in Chapter 72 |
| EC2 ARM64/Graviton | Practical exposure | Claimed — unverified | BASE-01 Q8 |
| Blue-green, canary, health checks, rollback | Concept-level exposure | Claimed — unverified | BASE-01 Q2, Q10; Part VIII |
| Deployment troubleshooting | Practical exposure | Claimed — unverified | BASE-01 Q1; LAB-001-01 Phases 2–3 |

**No exposure claimed** (treated as *not yet demonstrated*, which is not the same as *unknown to you*): IAM and VPC design, Route 53/CloudFront/ACM, Auto Scaling, Terraform, Ansible, Kubernetes, Helm, GitOps, Prometheus/Grafana/OpenTelemetry, service-level objectives and error budgets, DevSecOps (scanning, SBOM, signing), threat modelling, subnetting and routing, Linux and container internals, database internals (replication, point-in-time recovery), incident command and postmortems, architecture documentation.

**Assumptions to test (not findings).** These shape where the first assessments probe:

1. Happy-path operation is stronger than knowledge of internals (kernel primitives, the TCP and TLS handshakes, the Git object model).
2. Configuration skill is ahead of design reasoning (failure domains, trade-offs, alternatives considered).
3. Backup-and-restore testing and observability are the likeliest unverified operational areas.

## 3. Programme architecture

- **17 parts, 118 chapters, 291 sections.** Every curriculum topic maps to exactly one section ([`TABLE_OF_CONTENTS.md`](TABLE_OF_CONTENTS.md)).
- **8 phases** (A–H), each ending in a gate and a coherent portfolio increment.
- **8 flagship projects, delivered as 12 increments** ([`projects/PORTFOLIO.md`](projects/PORTFOLIO.md)).
- Phase and project dependencies: [`diagrams/FIG-001-programme-phases.md`](diagrams/FIG-001-programme-phases.md).

## 4. The learning loop

Every concept follows the same loop. The master prompt's 15 steps group into six movements:

| Movement | Steps | What happens |
|---|---|---|
| Teach | 1–6 | Concept, why it exists, internal working, architecture, real-world use, workplace scenario |
| Build | 7–9 | You implement it and verify its behaviour (lab Phase 1) |
| Break | 10 | A controlled failure is released by the mentor (Phase 2) |
| Diagnose | 11–12 | You investigate from evidence; the diagnosis is evaluated |
| Recover | 13 | You repair and verify |
| Prevent and assess | 14–15 | Architectural improvements; checkpoint assessment |

**Cadence.** A laboratory after every concept → an integrated assessment (`IA`) after every section → a practical review (`PR`) after every part → a professional engineering review (`PER`) after every flagship project.

**Interaction modes** (use the command word at the start of a message):

| Mode | Use |
|---|---|
| `TEACH` | Teach a concept and develop its section |
| `WRITE CHAPTER` | Write a complete chapter to the strict structure |
| `CONCEPT LAB` | Create the lab for one concept |
| `BUILD` | Guided implementation of a component |
| `BREAK` | Introduce a controlled failure |
| `TROUBLESHOOT` | Receive an incident; diagnostic process is assessed |
| `RECOVER` | Guided recovery after you have attempted diagnosis |
| `CASE STUDY` | Convert an actual incident into a documented case study |
| `PROJECT` | Build or review a flagship project |
| `ARCHITECT` | Receive an architecture problem; design is evaluated |
| `REVIEW CHAPTER` | Technical and editorial review |
| `BOOK AUDIT` | Find gaps, duplication, incomplete chapters |
| `PORTFOLIO REVIEW` | Evaluate whether a project demonstrates professional ability |
| `INTERVIEW` | Realistic technical interview |
| `REVISION` | Test retained knowledge |
| `ROADMAP` | Show progress across all six tracks |
| `EXPORT` | Prepare reviewed content for publication |

## 5. Roadmap

| Phase | Name | Parts | Chapters | Project increments | Exit gate |
|---|---|---|---|---|---|
| A | Foundations | I–III | 1–22 (22) | PRJ-01 | PR-P01 to PR-P03 passed; PRJ-01 engineering review passed; mock interview on Linux and networking |
| B | Delivery foundations | IV–V | 23–36 (14) | PRJ-02A | PR-P04, PR-P05 passed; PRJ-02A review passed |
| C | Cloud and Infrastructure as Code | VI–VII | 37–54 (18) | PRJ-03 | PR-P06, PR-P07 passed; PRJ-03 review passed; cost record kept |
| D | Delivery systems, edge, and data | VIII–X | 55–73 (19) | PRJ-04A, PRJ-02B | PR-P08 to PR-P10 passed; both reviews passed; verified restore evidence |
| E | Orchestration and platform | XI–XII | 74–90 (17) | PRJ-05A, PRJ-05B | PR-P11, PR-P12 passed; PRJ-05A/B reviews passed |
| F | Reliability and security | XIII–XIV | 91–103 (13) | PRJ-06, PRJ-05C, PRJ-04B, PRJ-07 | PR-P13, PR-P14 passed; four reviews passed |
| G | Senior and architect | XV–XVI | 104–114 (11) | PRJ-08 | PR-P15, PR-P16 passed; PRJ-08 review passed |
| H | Case studies and graduation | XVII | 115–118 (4) | (case studies) | Final evaluation (§12) |

**Each phase ends with a coherent, demonstrable portfolio.** You can pause after any phase with evidence of a complete capability, so the plan is driven by gates, not by the calendar.

**Planning assumption (replace with measured velocity after Part I).** About 12–20 hours per chapter (reading, labs, assessment) and 25–60 hours per project increment. On those figures: 118 chapters ≈ 1,400–2,400 hours; 12 increments ≈ 300–720 hours; total ≈ 1,700–3,100 hours. At 10 hours a week that is roughly 3.3–6 years; at 20 hours a week, 1.6–3 years; at 30 hours a week, 1.1–2 years. These are estimates to be corrected by data, not commitments.

## 6. Portfolio progression

| Increment | Project | Starts after | Completes after |
|---|---|---|---|
| PRJ-01 | Production-Ready Linux and Network Operations Environment | Part II | Part III |
| PRJ-02A | Enterprise-Style Container Platform (baseline) | Part V begins | Part V |
| PRJ-02B | Container platform: database-operations hardening | Part X begins | Part X |
| PRJ-03 | AWS Infrastructure as Code Platform | Part VI | Part VII |
| PRJ-04A | Secure Enterprise CI/CD Platform (through verified rollback) | Part VIII begins | Part VIII |
| PRJ-04B | CI/CD: SBOM, image signing, verification | Part XIV begins | Part XIV |
| PRJ-05A | Kubernetes Production Application Platform | Part XI begins | Part XI |
| PRJ-05B | Kubernetes platform: GitOps | Part XII begins | Part XII |
| PRJ-05C | Kubernetes platform: monitoring | Part XIII begins | Part XIII |
| PRJ-06 | Observability and SRE Platform | Part XIII begins | Part XIII |
| PRJ-07 | Internal Developer Platform | Part XIV (integrates XII–XIV) | Part XIV |
| PRJ-08 | Enterprise Cloud Architecture Capstone | Part XV | Part XVI |

Why increments: several projects in the master prompt contain elements taught in later parts (for example, SBOM and signing in Project 4 are taught in Part XIV). Splitting them keeps every project buildable with what has been taught while still delivering the full specification.

## 7. Laboratory environment and cost policy

- **Local first** for Parts I–V; **AWS from Part VI**, with a budget alert set *before* any billable resource exists.
- **Reference application (`refapp`).** All failure injection uses a purpose-built application that mirrors the *shape* of the AirDive stack (TypeScript frontend and API, PostgreSQL, Redis, Nginx; builds for arm64 and amd64) without touching AirDive. It is introduced in Chapter 2 and lives in its own repository (decision D-004).
- **Hardware (assumption).** About 8 GB of RAM is workable for Parts II–V; 16 GB or more is recommended from Part XI (multi-node Kubernetes). Confirm against your machine (decision D-005).
- Prices, free-tier terms, and quotas are verified against current AWS documentation at the point of use.
- Every lab has a teardown, and you confirm it ran.

## 8. Assessment and progression policy

**Five dimensions**, each rated separately: (1) conceptual understanding, (2) independent implementation, (3) troubleshooting and root-cause analysis, (4) production operations and reliability, (5) architecture and engineering judgement.

| Level | Name | Evidence |
|---|---|---|
| 1 | Learning | Can follow instructions; explanation incomplete |
| 2 | Guided implementation | Completes the task with hints; understands the steps |
| 3 | Independent engineering | Completes and verifies without hints; diagnoses unfamiliar variants |
| 4 | Advanced production engineering | Designs for failure, operates under pressure, prevents recurrence |
| 5 | Architect-level competence | Chooses between designs, justifies trade-offs, defends them under challenge |

**A successful explanation does not by itself show practical competence.** For important topics you must build, break, diagnose, recover, and explain.

**Completion criteria for a chapter (recommendation):** every concept lab accepted; every failure drill diagnosed from evidence; chapter assessment passed; competency assessment at **Level 3** for core chapters. Level 4 is targeted for the operations-critical parts (II, V, VIII, X, XI, XIII). Level 5 is expected only in Parts XV–XVI and PRJ-08.

**Placement challenge.** Where BASE-01 or an earlier lab shows strong competence, a chapter's labs may be taken in *challenge mode* (timed, no hints). Every lab is still done; only the support changes.

**Six separate progress tracks** are maintained in [`PROGRESS.md`](PROGRESS.md): book completion, learning progress, lab completion, project completion, portfolio quality, interview readiness.

## 9. Tooling status (as of 2026-11-14)

| Capability | Status | Notes |
|---|---|---|
| GitHub (source of truth) | **Not connected in this chat** | The manuscript is plain Markdown with relative links, so it works in any git host. No repository has been created or modified. Creating one needs your explicit approval (D-009). |
| Technical research | Available | Built-in web research. Every source carries a verification level in `REFERENCES.md`. |
| Diagrams | Mermaid in Markdown | Source stays in the repository. |
| Project management | Not set up | GitHub Issues and Projects by default, once a repository exists. |
| PDF / publication | Deferred | Generated from reviewed Markdown at `EXPORT`; a PDF is never the editable source. |
| Knowledge-management platform | Not used | Would be used only if you choose it. |

## 10. Decision log

Status key: **Mandated** (from the master prompt) · **Proposed** (the author's proposal; in force until you change it) · **Open** (needs your input).

| ID | Decision | Status |
|---|---|---|
| D-001 | 118 chapters; curriculum order preserved within each part; Part XVII grouped by failure theme because the master prompt lists its subjects as "potential" | Proposed |
| D-002 | Permanent chapter IDs; printed numbers derived from book order | Proposed |
| D-003 | Projects delivered in 12 increments where scope spans parts (§6) | Proposed |
| D-004 | Failure injection uses the reference application, never AirDive production. AirDive is used read-only for evidence and for case studies | Mandated (safety) / mechanism Proposed |
| D-005 | **Laboratory environment baseline**: your machine's OS and RAM, the OS of the AirDive hosts, and local-versus-cloud split. Needed before Chapter 4 | **Open** |
| D-006 | Case studies are harvested as matching parts are completed, then compiled in Part XVII | Proposed |
| D-007 | Assessment tiers, hint ladder, and chapter completion criteria (§8; guidelines §6) | Proposed |
| D-008 | Diagrams are Mermaid with `FIG-nnn` IDs | Mandated (Mermaid) / IDs Proposed |
| D-009 | Repository name, visibility, and any creation or push require your explicit approval | Mandated |
| D-010 | British English; ISO dates; UTC timestamps | Proposed |
| D-011 | Plan by gates, not by calendar (§5) | Proposed |

## 11. Risks to the programme

| Risk | Mitigation |
|---|---|
| Scale: hundreds of hours of work | Phase gates give a coherent portfolio at each stage; measured velocity replaces the estimate after Part I |
| Tool-first drift (collecting tools without understanding) | Concept-first chapters; assessment mode; no chapter completes without a diagnosed failure |
| Labs that have never been executed | Lab gates (`Drafted` → `Dry-run` → `Learner-run` → `Accepted`); statuses never overstate |
| Version drift (tools change faster than chapters) | Version baseline table per chapter; re-verification before *Practically validated* |
| Cloud cost overrun | Budget alert first; teardown in every lab; costs recorded per project |
| Over-reliance on one system (AirDive) | Reference application for labs; AirDive only for evidence |
| Author knowledge limits | Primary-source verification and a verification level on every reference |

## 12. Graduation

You must be able to take an unfamiliar infrastructure requirement and independently: understand the business problem; gather requirements; design an architecture; explain technology choices; build infrastructure; automate provisioning; secure the environment; deploy applications; implement CI/CD; monitor the system; define reliability objectives; simulate failures; diagnose root causes; recover services; perform postmortems; improve the architecture; analyse costs; document the solution; and defend your decisions.

The final evaluation consists of **a practical architecture challenge, a live troubleshooting exercise, and a technical defence of the portfolio projects.**
