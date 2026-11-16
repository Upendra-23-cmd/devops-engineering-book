# Progress

**Last updated:** 2026-11-16 · **Manuscript version:** 0.2.0

Six tracks are kept **separately**, because finishing the prose is not the same as learning the material, and learning it is not the same as being able to defend it.

## 1. Dashboard

| Track | Measure | Current value |
|---|---|---|
| **Book completion** | Chapters by status (Planned → Drafted → Practically validated → Technically reviewed → Editorially reviewed → Finalised) | 118 Planned · 0 Drafted · 0 Practically validated · 0 Technically reviewed · 0 Editorially reviewed · 0 Finalised. `CH-001` is *in drafting*: components 1–8 drafted; 9–11 drafted for concepts 1.1.1 and 1.1.2; 12–22 planned; 23–24 partial |
| **Learning progress** | Level (1–5) on each of five dimensions, per part | **Not assessed.** `BASE-01` has not been taken |
| **Lab completion** | Labs Accepted / labs written | 0 accepted · 2 labs drafted, not yet run (`LAB-001-01`, `LAB-001-02`) · 1 assessment drafted, not yet taken (`BASE-01`) · 8 further lab IDs reserved for Chapter 1 |
| **Project completion** | Flagship increments past gate G4 | 0 of 12 started |
| **Portfolio quality** | 20-criterion vector per project | Not scored |
| **Interview readiness** | Mock interviews passed; question-bank coverage | 0 mock interviews · question bank (Appendix D) planned |

A chapter is never reported as *Finalised* because the prose is complete (`EDITORIAL_GUIDELINES.md` §12).

## 2. Verification register (claimed versus verified)

Initial values come from the master prompt and are **self-reported**. Status changes only on evidence from `BASE-01`, a lab, or a project.

| Area | Status | Evidence | Level (1–5) |
|---|---|---|---|
| Linux | Claimed — unverified | — | — |
| Git and GitHub | Claimed — unverified | — | — |
| AWS EC2 and S3 | Claimed — unverified | — | — |
| Docker and Compose | Claimed — unverified | — | — |
| Jenkins and CI/CD | Claimed — unverified | — | — |
| GitHub Container Registry | Claimed — unverified | — | — |
| Nginx | Claimed — unverified | — | — |
| DNS and TLS | Claimed — unverified | — | — |
| Node.js and TypeScript deployments | Claimed — unverified | — | — |
| PostgreSQL and Redis | Claimed — unverified | — | — |
| EC2 ARM64/Graviton | Claimed — unverified | — | — |
| Blue-green, canary, health checks, rollback | Claimed — unverified (concept level) | — | — |
| Deployment troubleshooting | Claimed — unverified | — | — |

Areas for which no exposure was claimed (IAM and VPC design, Terraform, Ansible, Kubernetes, GitOps, observability tooling, service-level objectives, DevSecOps, threat modelling, subnetting and routing, database internals, incident command, architecture documentation) are *not yet demonstrated*; they are assessed when their parts begin.

## 3. Five-dimension matrix (per part)

Dimensions: **D1** conceptual understanding · **D2** independent implementation · **D3** troubleshooting and root-cause analysis · **D4** production operations and reliability · **D5** architecture and engineering judgement. Levels: 1 Learning · 2 Guided implementation · 3 Independent engineering · 4 Advanced production engineering · 5 Architect-level competence.

| Part | D1 | D2 | D3 | D4 | D5 |
|---|---|---|---|---|---|
| I–XVII | — | — | — | — | — |

*(One row per part is added as each part begins; every cell is currently "not assessed".)*

## 4. Chapter register

| ID | No. | Part | Chapter | Status | Drafting progress |
|---|---|---|---|---|---|
| CH-001 | 1 | I | From Silos to DevOps: Evolution, Principles, and Culture | Planned (drafting in progress) | Front matter, §1.1.1 and §1.1.2 drafted; §1.1.3–§1.2 and chapter-level components planned |
| CH-002 | 2 | I | The Software Lifecycle, Production Systems, and Environment Strategy | Planned | Not started |
| CH-003 | 3 | I | Automation, CI/CD Foundations, and the DevOps Engineer's Role | Planned | Not started |
| CH-004 | 4 | II | Linux Architecture: Kernel, User Space, and the Filesystem Hierarchy | Planned | Not started |
| CH-005 | 5 | II | Linux Users, Groups, Permissions, Ownership, and ACLs | Planned | Not started |
| CH-006 | 6 | II | Processes, Signals, and systemd Services | Planned | Not started |
| CH-007 | 7 | II | Package Management and Shell Scripting | Planned | Not started |
| CH-008 | 8 | II | CPU and Memory | Planned | Not started |
| CH-009 | 9 | II | Disk, Storage, and Filesystems | Planned | Not started |
| CH-010 | 10 | II | Logs and journald | Planned | Not started |
| CH-011 | 11 | II | Linux Networking | Planned | Not started |
| CH-012 | 12 | II | SSH, Server Security, and Linux Hardening | Planned | Not started |
| CH-013 | 13 | II | Production Server Administration | Planned | Not started |
| CH-014 | 14 | III | OSI, TCP/IP, and IP Addressing | Planned | Not started |
| CH-015 | 15 | III | Subnetting and Routing | Planned | Not started |
| CH-016 | 16 | III | TCP and UDP | Planned | Not started |
| CH-017 | 17 | III | DNS | Planned | Not started |
| CH-018 | 18 | III | HTTP, HTTPS, and TLS | Planned | Not started |
| CH-019 | 19 | III | Ports, Sockets, Firewalls, and NAT | Planned | Not started |
| CH-020 | 20 | III | Reverse Proxies and Load Balancing | Planned | Not started |
| CH-021 | 21 | III | Network Troubleshooting | Planned | Not started |
| CH-022 | 22 | III | Cloud Networking and Network Security | Planned | Not started |
| CH-023 | 23 | IV | Git Internals | Planned | Not started |
| CH-024 | 24 | IV | Branching, Merging, Rebase, and Conflict Resolution | Planned | Not started |
| CH-025 | 25 | IV | Pull Requests, Code Review, and Branch Protection | Planned | Not started |
| CH-026 | 26 | IV | Release Tags and Versioning | Planned | Not started |
| CH-027 | 27 | IV | GitHub Actions | Planned | Not started |
| CH-028 | 28 | IV | GitOps Foundations, Repository Security, and Engineering Collaboration | Planned | Not started |
| CH-029 | 29 | V | Virtualisation, Containers, Namespaces, and cgroups | Planned | Not started |
| CH-030 | 30 | V | Docker Engine, Images, and Layers | Planned | Not started |
| CH-031 | 31 | V | Dockerfiles, BuildKit and Caching, and Multi-Stage Builds | Planned | Not started |
| CH-032 | 32 | V | Container Networking and Volumes | Planned | Not started |
| CH-033 | 33 | V | Docker Compose, Health Checks, and Resource Management | Planned | Not started |
| CH-034 | 34 | V | Container Security | Planned | Not started |
| CH-035 | 35 | V | Registries, Image Tagging, and ARM64/AMD64 | Planned | Not started |
| CH-036 | 36 | V | Container Debugging and Production Container Operations | Planned | Not started |
| CH-037 | 37 | VI | Cloud Computing and AWS Global Infrastructure | Planned | Not started |
| CH-038 | 38 | VI | AWS IAM | Planned | Not started |
| CH-039 | 39 | VI | VPC, Subnets, and Route Tables | Planned | Not started |
| CH-040 | 40 | VI | Internet Gateways, NAT Gateways, Security Groups, and Network ACLs | Planned | Not started |
| CH-041 | 41 | VI | EC2 and EBS | Planned | Not started |
| CH-042 | 42 | VI | S3 | Planned | Not started |
| CH-043 | 43 | VI | Load Balancers and Auto Scaling | Planned | Not started |
| CH-044 | 44 | VI | Route 53, CloudFront, and ACM | Planned | Not started |
| CH-045 | 45 | VI | CloudWatch and AWS Cost Management | Planned | Not started |
| CH-046 | 46 | VI | High Availability and Disaster Recovery | Planned | Not started |
| CH-047 | 47 | VII | Infrastructure as Code Principles and Terraform Architecture | Planned | Not started |
| CH-048 | 48 | VII | Providers, Resources, Data Sources, Variables, and Outputs | Planned | Not started |
| CH-049 | 49 | VII | Terraform State and Remote State | Planned | Not started |
| CH-050 | 50 | VII | Modules, Workspaces, and Environment Separation | Planned | Not started |
| CH-051 | 51 | VII | Import, Drift, Terraform Testing, and Terraform Security | Planned | Not started |
| CH-052 | 52 | VII | Ansible Architecture, Inventories, and Playbooks | Planned | Not started |
| CH-053 | 53 | VII | Roles, Configuration Drift, Idempotency, and Secret Handling | Planned | Not started |
| CH-054 | 54 | VII | Infrastructure Automation Pipelines | Planned | Not started |
| CH-055 | 55 | VIII | CI/CD Principles and Jenkins Architecture | Planned | Not started |
| CH-056 | 56 | VIII | Pipeline Design, Jenkinsfiles, and Build Automation | Planned | Not started |
| CH-057 | 57 | VIII | Testing, Code Quality, and Security Scanning | Planned | Not started |
| CH-058 | 58 | VIII | Image Creation, Registry Publishing, and Artifact Management | Planned | Not started |
| CH-059 | 59 | VIII | Deployment Automation and Immutable Releases | Planned | Not started |
| CH-060 | 60 | VIII | Blue-Green, Canary, and Progressive Delivery | Planned | Not started |
| CH-061 | 61 | VIII | Rollback, Pipeline Security, and Release Governance | Planned | Not started |
| CH-062 | 62 | IX | Web Server Architecture and Nginx Internals | Planned | Not started |
| CH-063 | 63 | IX | Reverse Proxies, Upstreams, Load Balancing, and HTTP Routing | Planned | Not started |
| CH-064 | 64 | IX | Headers, TLS, Certificates, and Renewal | Planned | Not started |
| CH-065 | 65 | IX | Unprivileged Containers, File Permissions, and Configuration Validation | Planned | Not started |
| CH-066 | 66 | IX | Proxy Troubleshooting and Secure Edge Design | Planned | Not started |
| CH-067 | 67 | X | Database Fundamentals and PostgreSQL Architecture | Planned | Not started |
| CH-068 | 68 | X | Transactions, Indexes, and Connection Pooling | Planned | Not started |
| CH-069 | 69 | X | Persistent Storage and Replication | Planned | Not started |
| CH-070 | 70 | X | Backups and Point-in-Time Recovery | Planned | Not started |
| CH-071 | 71 | X | Migrations and Schema Compatibility | Planned | Not started |
| CH-072 | 72 | X | Redis | Planned | Not started |
| CH-073 | 73 | X | Database Monitoring, Security, and Recovery Testing | Planned | Not started |
| CH-074 | 74 | XI | Why Orchestration Exists and Kubernetes Architecture | Planned | Not started |
| CH-075 | 75 | XI | The Control Plane and Nodes | Planned | Not started |
| CH-076 | 76 | XI | Pods, Deployments, and ReplicaSets | Planned | Not started |
| CH-077 | 77 | XI | Services, Ingress, and Gateway API | Planned | Not started |
| CH-078 | 78 | XI | ConfigMaps and Secrets | Planned | Not started |
| CH-079 | 79 | XI | Storage and Persistent Volumes | Planned | Not started |
| CH-080 | 80 | XI | Probes, Resource Requests and Limits, and Scheduling | Planned | Not started |
| CH-081 | 81 | XI | Autoscaling | Planned | Not started |
| CH-082 | 82 | XI | RBAC and Network Policies | Planned | Not started |
| CH-083 | 83 | XI | Helm | Planned | Not started |
| CH-084 | 84 | XI | Cluster Security and Kubernetes Troubleshooting | Planned | Not started |
| CH-085 | 85 | XI | Cluster Upgrades and Production Operations | Planned | Not started |
| CH-086 | 86 | XII | Platform Engineering, Internal Developer Platforms, and Developer Self-Service | Planned | Not started |
| CH-087 | 87 | XII | GitOps Architecture with Argo CD or Flux | Planned | Not started |
| CH-088 | 88 | XII | Environment Promotion, Deployment Templates, and Platform APIs | Planned | Not started |
| CH-089 | 89 | XII | Golden Paths, Policy as Code, and Multi-Tenancy | Planned | Not started |
| CH-090 | 90 | XII | Platform Security, Developer Experience, and Platform Observability | Planned | Not started |
| CH-091 | 91 | XIII | Monitoring and Observability | Planned | Not started |
| CH-092 | 92 | XIII | Metrics, Logs, and Distributed Tracing | Planned | Not started |
| CH-093 | 93 | XIII | Prometheus, Grafana, and Alertmanager | Planned | Not started |
| CH-094 | 94 | XIII | OpenTelemetry and Service Health | Planned | Not started |
| CH-095 | 95 | XIII | SLIs, SLOs, SLAs, and Error Budgets | Planned | Not started |
| CH-096 | 96 | XIII | Incident Response and Postmortems | Planned | Not started |
| CH-097 | 97 | XIII | Capacity Planning, Reliability, Disaster Recovery, and Performance Engineering | Planned | Not started |
| CH-098 | 98 | XIV | Security Engineering Fundamentals and Threat Modelling | Planned | Not started |
| CH-099 | 99 | XIV | IAM, Least Privilege, and Secrets Management | Planned | Not started |
| CH-100 | 100 | XIV | Container Security, Image Scanning, and Dependency Scanning | Planned | Not started |
| CH-101 | 101 | XIV | SAST, DAST, and SBOM | Planned | Not started |
| CH-102 | 102 | XIV | Image Signing, Provenance, Attestations, and Supply-Chain Security | Planned | Not started |
| CH-103 | 103 | XIV | Policy Enforcement, Runtime Security, Audit Logging, and Security Incident Response | Planned | Not started |
| CH-104 | 104 | XV | Distributed Systems, Failure Domains, and Fault Tolerance | Planned | Not started |
| CH-105 | 105 | XV | High Availability, Resilience, Scalability, and Performance | Planned | Not started |
| CH-106 | 106 | XV | Cost Optimisation, Technical Debt, and Operational Excellence | Planned | Not started |
| CH-107 | 107 | XV | Incident Command, Change Management, and Reliability Trade-offs | Planned | Not started |
| CH-108 | 108 | XV | Engineering Leadership and Technical Decision-Making | Planned | Not started |
| CH-109 | 109 | XVI | Requirements Analysis, Architecture Principles, and Architecture Diagrams | Planned | Not started |
| CH-110 | 110 | XVI | Network, Security, Compute, and Storage Architecture | Planned | Not started |
| CH-111 | 111 | XVI | Data, Deployment, and Observability Architecture | Planned | Not started |
| CH-112 | 112 | XVI | Multi-AZ, Multi-Region, and Disaster Recovery Design | Planned | Not started |
| CH-113 | 113 | XVI | Cost Architecture, Architecture Decision Records, and Technology Selection | Planned | Not started |
| CH-114 | 114 | XVI | Risk Analysis, Design Reviews, and Architecture Governance | Planned | Not started |
| CH-115 | 115 | XVII | Application Runtime and Container Failures | Planned | Not started |
| CH-116 | 116 | XVII | Pipeline, Registry, and Artifact Failures | Planned | Not started |
| CH-117 | 117 | XVII | Edge, Network, and Browser-Boundary Failures | Planned | Not started |
| CH-118 | 118 | XVII | Release Strategy, Rollback, and Verification | Planned | Not started |

## 5. Lab register

| ID | Title | Chapter | Status | Notes |
|---|---|---|---|---|
| `BASE-01` | Baseline assessment | — | Drafted, not yet taken | Answer key held by the mentor |
| `LAB-001-01` | Evidence-based value stream map | `CH-001` | Drafted, not yet run | Phase 2 withheld until Phase 1 is accepted |
| `LAB-001-02` | Handoff-chain reconstruction of a real incident | `CH-001` | Drafted, not yet run | Reuses `LAB-001-01` data and an incident from `BASE-01` B4; Phase 2 withheld |
| `LAB-001-03`–`LAB-001-10` | Reserved | `CH-001` | Not written | |

## 6. Project register

| Increment | Project | Status | Gate |
|---|---|---|---|
| PRJ-01 | Linux and Network Operations Environment | Planned | — |
| PRJ-02A | Container Platform (baseline) | Planned | — |
| PRJ-02B | Container platform: database operations | Planned | — |
| PRJ-03 | AWS Infrastructure as Code Platform | Planned | — |
| PRJ-04A | CI/CD Platform (through rollback) | Planned | — |
| PRJ-04B | CI/CD: SBOM, signing, verification | Planned | — |
| PRJ-05A | Kubernetes Platform | Planned | — |
| PRJ-05B | Kubernetes platform: GitOps | Planned | — |
| PRJ-05C | Kubernetes platform: monitoring | Planned | — |
| PRJ-06 | Observability and SRE Platform | Planned | — |
| PRJ-07 | Internal Developer Platform | Planned | — |
| PRJ-08 | Enterprise Cloud Architecture Capstone | Planned | — |

## 7. Portfolio quality and interview readiness

- **Portfolio quality:** no project exists yet, so there is nothing to score. Scoring uses the 20-criterion vector in `projects/PORTFOLIO.md` §4.
- **Interview readiness:** mock interviews are held at each phase gate in `INTERVIEW` mode. None has been held. Each project must pass the nine-question defence in `projects/PORTFOLIO.md` §7.

## 8. AirDive evidence register

| Incident ID | Subject | Evidence received | Redaction checked |
|---|---|---|---|
| *(none yet)* | | | |

No incident evidence has been supplied. No case study can be written until it is. See [`case-studies/README.md`](case-studies/README.md).

## 9. Open decisions and blockers

| Item | Needed from you | Needed by |
|---|---|---|
| **D-005** Laboratory environment: your machine's OS and RAM, the OS of the AirDive hosts, local-versus-cloud split | A short description | Before Chapter 4 |
| **D-009** GitHub repository name and visibility, and approval to create or push | Your instruction | Whenever you want the repository created |
| GitHub integration | The integration is not connected in this chat | Before any repository action |

## 10. Next actions

1. Complete [`BASE-01`](labs/diagnostic/BASE-01-baseline-assessment.md): closed-book first pass, with confidence ratings.
2. Do Phase 1 of [`LAB-001-01`](labs/ch-001/LAB-001-01-value-stream-map.md) and reply with the redacted write-up.
3. Answer the six checkpoint questions at the end of concept 1.1.1.
4. Read concept 1.1.2. After `LAB-001-01`, do Phase 1 of [`LAB-001-02`](labs/ch-001/LAB-001-02-handoff-chain-reconstruction.md) (it reuses your `LAB-001-01` data and an incident from `BASE-01` B4) and answer its six checkpoint questions. Nothing is evaluated until you submit.
5. Optional: log the three incidents you learned most from using the intake template, so that evidence is captured while it still exists.
