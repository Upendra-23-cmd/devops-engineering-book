# Professional Project Portfolio

**Version:** 0.1.0 · **Last updated:** 2026-11-14 · **Status:** Planned (no project has started)

## 1. Principles

- **Depth over count.** Eight flagship projects, each with a clear business problem, requirements, architecture, implementation, failure testing, and evidence. No dozens of trivial repositories.
- **Quality is not the technology.** A project is not enterprise-grade because it uses Kubernetes, Terraform, or AWS. It is judged on the 20-point standard in §4.
- **Evidence or it did not happen.** Every claim of performance, availability, or recovery is backed by a recorded run. Numbers are never invented.
- **AirDive production is never a lab.** Projects use the reference application and disposable environments (see `BOOK_PLAN.md`, D-004).
- **Business problems are defined with you at gate G0.** They are chosen to be realistic and, where possible, shaped like AirDive work, without using AirDive production systems or data.

## 2. Progression

Projects are delivered in **increments** where the scope in the master prompt includes topics taught in later parts. Phase gates are in [`../BOOK_PLAN.md`](../BOOK_PLAN.md) §5; the dependency diagram is [`FIG-001`](../diagrams/FIG-001-programme-phases.md).

| Increment | Project | Completes after | Notes |
|---|---|---|---|
| PRJ-01 | Production-Ready Linux and Network Operations Environment | Part III | Nginx, DNS and TLS are used at the depth of Parts II–III; Part IX adds edge depth |
| PRJ-02A | Enterprise-Style Container Platform (baseline) | Part V | PostgreSQL and Redis are used as managed-by-you dependencies |
| PRJ-02B | Container platform: database operations | Part X | Backup, restore, replication, and migration evidence added |
| PRJ-03 | AWS Infrastructure as Code Platform | Part VII | Needs Parts VI and VII |
| PRJ-04A | Secure Enterprise CI/CD Platform | Part VIII | Pipeline through deployment, smoke tests, and rollback |
| PRJ-04B | CI/CD: SBOM, signing, verification | Part XIV | Adds the supply-chain controls taught in Part XIV |
| PRJ-05A | Kubernetes Production Application Platform | Part XI | Cluster, workloads, security, failure drills |
| PRJ-05B | Kubernetes platform: GitOps | Part XII | |
| PRJ-05C | Kubernetes platform: monitoring | Part XIII | |
| PRJ-06 | Observability and SRE Platform | Part XIII | |
| PRJ-07 | Internal Developer Platform | Part XIV | Integrates Parts XII–XIV |
| PRJ-08 | Enterprise Cloud Architecture Capstone | Part XVI | Integrates everything; includes recovery under injected failure |

## 3. Project scopes (from the master prompt)

### PRJ-01 — Production-Ready Linux and Network Operations Environment
- **Include:** server provisioning; users and permissions; SSH hardening; firewall; systemd services; Nginx; DNS; TLS; log management; resource monitoring; backup and recovery.
- **Demonstrate:** permission failures; service failures; network failures; disk exhaustion (disposable environment); TLS problems; incident diagnosis and recovery.
- **Deliverables:** architecture diagram; infrastructure documentation; configuration files; hardening checklist; runbooks; incident reports.

### PRJ-02 — Enterprise-Style Container Platform
- **Include:** frontend; backend; PostgreSQL; Redis; Dockerfiles; Compose; persistent storage; container networking; health checks; resource constraints; image scanning; secure configuration.
- **Demonstrate:** container failure; network failure; dependency failure; data-persistence failure; image build failure; recovery.
- **Deliverables:** source repository; Docker configurations; architecture diagrams; test procedures; security review; troubleshooting runbooks.

### PRJ-03 — AWS Infrastructure as Code Platform
- **Include:** VPC; public and private subnets; routing; security groups; IAM; compute; storage; load balancing; logging; monitoring; environment separation; remote state; automated plan-and-apply workflow.
- **Demonstrate:** configuration errors; permission failures; network isolation; infrastructure drift; recovery from failed provisioning.
- **Deliverables:** Terraform modules; architecture diagrams; environment documentation; security controls; cost estimate; deployment and destruction procedures.

### PRJ-04 — Secure Enterprise CI/CD Platform
- **Include:** GitHub; pull-request checks; unit and integration testing; code quality; dependency scanning; container building; image publishing; SBOM generation; image verification; deployment; health checks; smoke tests; rollback.
- **Demonstrate:** failed builds; registry authentication failures; incorrect artifacts; vulnerable dependencies; failed deployment; rollback verification.
- **Deliverables:** pipeline definitions; security policies; build documentation; release process; deployment runbooks; incident reports.
- **Increments:** 04A = everything except SBOM generation and image verification; 04B adds those.

### PRJ-05 — Kubernetes Production Application Platform
- **Include:** cluster architecture; application deployments; services; ingress or Gateway API; Helm; secrets; persistent storage; resource limits; autoscaling; RBAC; network policies; monitoring; GitOps.
- **Demonstrate:** CrashLoopBackOff; image-pull errors; scheduling failures; probe failures; network-policy problems; storage failures; rollback.
- **Deliverables:** Helm charts; Kubernetes manifests; GitOps configuration; architecture documentation; security assessment; operational runbooks.
- **Increments:** 05A = all except GitOps and monitoring; 05B adds GitOps; 05C adds monitoring.

### PRJ-06 — Observability and SRE Platform
- **Include:** Prometheus; Grafana; Alertmanager; OpenTelemetry; application metrics; logs; distributed traces; dashboards; alert rules; SLIs; SLOs; error budgets.
- **Demonstrate:** high latency; high resource utilisation; failed dependencies; missing telemetry; alert failures; recovery procedures.
- **Deliverables:** dashboards; alert definitions; SLO documentation; incident timelines; postmortems; reliability improvements.

### PRJ-07 — Internal Developer Platform
- **Include:** standardised application templates; automated environment provisioning; CI/CD; GitOps; reusable Helm charts; secrets integration; deployment policies; observability; developer documentation; self-service workflows.
- **Demonstrate:** provisioning failures; policy violations; deployment failures; environment drift; multi-team isolation issues.
- **Deliverables:** platform architecture; golden paths; templates; developer documentation; platform operations guide; adoption and reliability measurements.
- **Honest-measurement rule:** with no second team, adoption can only be measured on synthetic tenants or on services the owner agrees to include. Synthetic numbers are always labelled synthetic and are never presented as real adoption.

### PRJ-08 — Enterprise Cloud Architecture Capstone
- **Requirements:** high availability; secure network design; least privilege; Infrastructure as Code; automated CI/CD; container orchestration; GitOps; monitoring and tracing; backup and recovery; disaster recovery; cost controls; incident response; technical documentation.
- Realistic operational failures are introduced and you must recover the platform. The project must show that you can own a complete engineering system, not just individual tools.

## 4. Quality standard (applies to every flagship increment)

| # | Criterion | Evidence expected |
|---|---|---|
| 1 | Business problem and requirements | Problem statement; stakeholders; success measures |
| 2 | Functional and non-functional requirements | Numbered requirements with measurable targets |
| 3 | Architecture diagram | Mermaid source in the repository |
| 4 | Technology selection and justification | Options considered and why one was chosen |
| 5 | Architecture Decision Records | `docs/adr/ADR-nnnn-*.md` |
| 6 | Infrastructure as Code (where applicable) | Code in version control |
| 7 | Reproducible setup | A stranger can rebuild from the README |
| 8 | Automated testing | Test reports from recorded runs |
| 9 | Security controls | Controls mapped to threats |
| 10 | Secrets handling | No secrets in the repository; rotation described |
| 11 | Observability | Dashboards, logs, alerts that were actually exercised |
| 12 | Failure injection | Each failure listed, with the evidence of it |
| 13 | Troubleshooting | Diagnosis records written from evidence |
| 14 | Recovery and rollback | Recovery executed and timed |
| 15 | Performance evaluation | Load-test results from recorded runs |
| 16 | Cost analysis | Estimate, plus actual from billing where available |
| 17 | Runbooks | `docs/runbooks/RB-*.md`, each tested |
| 18 | Operational documentation | Day-2 operations guide |
| 19 | Threat model | Assets, trust boundaries, threats, mitigations |
| 20 | Limitations and future improvements | Honest list |

**Scoring rubric per criterion:** 0 Absent · 1 Stated, not demonstrated · 2 Implemented · 3 Implemented, tested, evidenced, and reviewed. Report the **vector** of 20 scores; a single total is allowed only as a summary and never replaces the vector.

## 5. Evidence of engineering ability

Evidence is collected in an `evidence/` folder inside each project:

`deploy-logs/` · `test-reports/` · `pipeline-runs/` · `terraform-plans/` · `scans/` · `dashboards/` · `load-tests/` · `recovery/` · `incidents/`

**Every evidence file begins with a provenance header:** date (UTC), environment, tool versions, the exact command or job, and who ran it. Evidence without provenance does not count. **Never invent** performance numbers, availability percentages, or test results.

## 6. Project lifecycle gates

| Gate | Name | Exit condition |
|---|---|---|
| G0 | Specification accepted | Business problem, requirements, and architecture agreed; ADRs started |
| G1 | Build complete | Reproducible from the README; tests passing in recorded runs |
| G2 | Failure drills complete | Every listed failure injected, diagnosed from evidence, and recovered |
| G3 | Evidence pack complete | Quality standard scored; evidence has provenance |
| G4 | Professional engineering review (`PER-PRJ-nn`) | Review findings resolved or accepted as documented limitations |
| G5 | Defence rehearsal | Mock `INTERVIEW` on the project passed (§7) |

## 7. Interview defence checklist

For each project you must be able to answer, with evidence:

1. What problem did you solve?
2. Why did you choose this architecture?
3. What alternatives did you consider?
4. What failed?
5. How did you diagnose it?
6. What security risks did you identify?
7. How did you test recovery?
8. What would you change at larger scale?
9. What are the system's limitations?

## 8. Representative repository layout

Use only the folders a project needs.

```text
<project>/
  README.md
  docs/
    architecture/   adr/   runbooks/   postmortems/   security/
  infra/            terraform/   ansible/
  kubernetes/       helm/        gitops/
  applications/     pipelines/   monitoring/   policies/
  scripts/          tests/       examples/     evidence/
```
