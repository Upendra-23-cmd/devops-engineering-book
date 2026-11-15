# Table of Contents

**Book:** The Practical DevOps Engineer  
**Subtitle:** From Linux Fundamentals to Enterprise Cloud Infrastructure, Platform Engineering, and DevOps Architecture  
**Manuscript version:** 0.1.0 · **Generated:** 2026-11-14

This is the book-level contents: Part → Chapter → Section. Every section corresponds to exactly one topic in the master curriculum, and every curriculum topic appears exactly once (checked by script when this file was generated). Concept-level (x.y.z) contents are produced chapter by chapter; Chapter 1's is in its chapter file.

## How to read this file

- **Identifiers.** Each chapter has a permanent ID (`CH-001` and so on). The printed chapter number follows book order and may change before the publication freeze, so cross-reference by ID.
- **Lab themes** are indicative. They are finalised when the chapter is written and validated, and every concept in a chapter receives its own laboratory.
- **Status** of each chapter is tracked in [`PROGRESS.md`](PROGRESS.md), not here.
- **Curriculum order is preserved** inside each part. Where a concept needs one that appears later, the chapter forward-references it rather than reordering the curriculum.
- **Phases** (A–H) group parts into milestones; they are defined in [`BOOK_PLAN.md`](BOOK_PLAN.md).

## Front matter (planned)

- Preface: who this book is for and what it will and will not claim
- How to use this book: the learning loop and the hint ladder
- Safety, cost, and ethics in laboratories
- The reference application and the laboratory environment
- Notation, conventions, and version baselines

## Contents at a glance

| Part | Title | Phase | Chapters | Sections |
|---|---|---|---|---|
| I | DevOps Engineering Foundations | A | 1–3 (3) | 9 |
| II | Linux and Systems Engineering | A | 4–13 (10) | 17 |
| III | Networking and Internet Infrastructure | A | 14–22 (9) | 16 |
| IV | Git, GitHub and Engineering Workflows | B | 23–28 (6) | 12 |
| V | Docker and Container Engineering | B | 29–36 (8) | 18 |
| VI | AWS and Cloud Architecture | C | 37–46 (10) | 22 |
| VII | Infrastructure as Code and Configuration Management | C | 47–54 (8) | 20 |
| VIII | CI/CD and Release Engineering | D | 55–61 (7) | 20 |
| IX | Nginx, Edge Infrastructure and TLS | D | 62–66 (5) | 15 |
| X | Databases and Stateful Infrastructure | D | 67–73 (7) | 15 |
| XI | Kubernetes and Container Orchestration | E | 74–85 (12) | 24 |
| XII | GitOps and Platform Engineering | E | 86–90 (5) | 14 |
| XIII | Observability and Site Reliability Engineering | F | 91–97 (7) | 20 |
| XIV | DevSecOps and Software Supply Chain Security | F | 98–103 (6) | 17 |
| XV | Senior DevOps Engineering | G | 104–108 (5) | 15 |
| XVI | Cloud and DevOps Architecture | G | 109–114 (6) | 19 |
| XVII | Real-World AirDive Engineering Case Studies | H | 115–118 (4) | 18 |
| | **Total** | | **118 chapters** | **291 sections** |

---

## Part I — DevOps Engineering Foundations

**Phase A — Foundations.**  
**Practical outcome (proposed; not specified in the master curriculum):** A measured, evidence-backed model of one real delivery path (lead time, constraints, improvement hypotheses) plus a documented model of its environments and architecture.  
**Projects:** No flagship project. Part practical review PR-P01 closes the part.  
**Part practical review:** `PR-P01`

### Chapter 1 — From Silos to DevOps: Evolution, Principles, and Culture `CH-001`

- 1.1 Evolution of software engineering and operations
- 1.2 DevOps principles and culture

*Lab themes (indicative):* Evidence-based value stream map of a real delivery path; batch-size experiment with git bisect; blameless rewrite of a real incident; delivery metrics from real history.

### Chapter 2 — The Software Lifecycle, Production Systems, and Environment Strategy `CH-002`

- 2.1 Software development lifecycle
- 2.2 Infrastructure and production environments
- 2.3 Application architecture fundamentals
- 2.4 Development, testing, staging, and production

*Lab themes (indicative):* Trace a request through the reference stack; environment parity audit; architecture-from-evidence of a real service.

### Chapter 3 — Automation, CI/CD Foundations, and the DevOps Engineer's Role `CH-003`

- 3.1 CI/CD and automation fundamentals
- 3.2 DevOps engineering responsibilities
- 3.3 Senior engineering and architectural thinking

*Lab themes (indicative):* Automate one manual release step and measure the effect; ownership and on-call readiness map; written trade-off decision memo.

---

## Part II — Linux and Systems Engineering

**Phase A — Foundations.**  
**Major practical outcome (from the master curriculum):** build, secure, monitor, break, troubleshoot, and recover a Linux application server.  
**Projects:** Feeds PRJ-01 (completes after Part III).  
**Part practical review:** `PR-P02`

### Chapter 4 — Linux Architecture: Kernel, User Space, and the Filesystem Hierarchy `CH-004`

- 4.1 Linux architecture
- 4.2 Kernel and user space
- 4.3 Filesystem hierarchy

*Lab themes (indicative):* Trace system calls; map the filesystem hierarchy on a live host; observe the kernel/user-space boundary.

### Chapter 5 — Linux Users, Groups, Permissions, Ownership, and ACLs `CH-005`

- 5.1 Users and groups
- 5.2 Permissions, ownership, ACLs

*Lab themes (indicative):* Repair a service that fails on ownership; design a least-privilege group model; ACL repair.

### Chapter 6 — Processes, Signals, and systemd Services `CH-006`

- 6.1 Processes and signals
- 6.2 systemd and services

*Lab themes (indicative):* Process lifecycle and signal handling; write, harden, and deliberately break a systemd unit.

### Chapter 7 — Package Management and Shell Scripting `CH-007`

- 7.1 Package management
- 7.2 Shell scripting

*Lab themes (indicative):* Repair broken package state in a disposable VM; write an idempotent provisioning script with error handling and tests.

### Chapter 8 — CPU and Memory `CH-008`

- 8.1 CPU and memory

*Lab themes (indicative):* Distinguish CPU saturation from memory pressure; reproduce and diagnose an out-of-memory kill.

### Chapter 9 — Disk, Storage, and Filesystems `CH-009`

- 9.1 Disk and storage
- 9.2 Filesystems

*Lab themes (indicative):* Disk-full and inode-exhaustion incidents on a disposable loop device; filesystem resize and recovery.

### Chapter 10 — Logs and journald `CH-010`

- 10.1 Logs and journald

*Lab themes (indicative):* Reconstruct an incident timeline from the journal; log-rotation failure.

### Chapter 11 — Linux Networking `CH-011`

- 11.1 Linux networking

*Lab themes (indicative):* Inspect interfaces, routes, and sockets; isolate a connectivity fault using network namespaces.

### Chapter 12 — SSH, Server Security, and Linux Hardening `CH-012`

- 12.1 SSH and server security
- 12.2 Linux hardening

*Lab themes (indicative):* Harden sshd and verify it; lock-out recovery in a disposable VM; audit against a hardening checklist.

### Chapter 13 — Production Server Administration `CH-013`

- 13.1 Production server administration

*Lab themes (indicative):* Integrated lab: build, monitor, break, and recover the Part II application server.

---

## Part III — Networking and Internet Infrastructure

**Phase A — Foundations.**  
**Major practical outcome (from the master curriculum):** design and troubleshoot a multi-tier application network.  
**Projects:** Completes PRJ-01: Production-Ready Linux and Network Operations Environment.  
**Part practical review:** `PR-P03`

### Chapter 14 — OSI, TCP/IP, and IP Addressing `CH-014`

- 14.1 OSI and TCP/IP
- 14.2 IP addressing

*Lab themes (indicative):* Annotated packet-capture walk-through; build an address plan.

### Chapter 15 — Subnetting and Routing `CH-015`

- 15.1 Subnetting
- 15.2 Routing

*Lab themes (indicative):* Design a subnet plan; diagnose a routing-table fault.

### Chapter 16 — TCP and UDP `CH-016`

- 16.1 TCP and UDP

*Lab themes (indicative):* Capture handshake and teardown; diagnose resets and timeouts.

### Chapter 17 — DNS `CH-017`

- 17.1 DNS

*Lab themes (indicative):* Run a resolver in a sandbox; break resolution and diagnose it from evidence.

### Chapter 18 — HTTP, HTTPS, and TLS `CH-018`

- 18.1 HTTP and HTTPS
- 18.2 TLS

*Lab themes (indicative):* Inspect a handshake and certificate chain; expired and incomplete-chain certificate incidents.

### Chapter 19 — Ports, Sockets, Firewalls, and NAT `CH-019`

- 19.1 Ports and sockets
- 19.2 Firewalls
- 19.3 NAT

*Lab themes (indicative):* Blocked-port incident; build a stateful firewall policy; NAT in a lab network namespace.

### Chapter 20 — Reverse Proxies and Load Balancing `CH-020`

- 20.1 Reverse proxies
- 20.2 Load balancing

*Lab themes (indicative):* Nginx reverse proxy to two backends; failover test.

### Chapter 21 — Network Troubleshooting `CH-021`

- 21.1 Network troubleshooting

*Lab themes (indicative):* Layered troubleshooting playbook; multi-fault network incident worked from evidence.

### Chapter 22 — Cloud Networking and Network Security `CH-022`

- 22.1 Cloud networking
- 22.2 Network security

*Lab themes (indicative):* Map on-premises network primitives to cloud equivalents; threat-model a network.

---

## Part IV — Git, GitHub and Engineering Workflows

**Phase B — Delivery foundations.**  
**Major practical outcome (from the master curriculum):** establish a professional software delivery repository with reviews, automated checks, release management, and documentation.  
**Projects:** The repository standard produced here is reused by every later project; PRJ-04A builds directly on it.  
**Part practical review:** `PR-P04`

### Chapter 23 — Git Internals `CH-023`

- 23.1 Git internals

*Lab themes (indicative):* Inspect objects with plumbing commands; recover lost commits.

### Chapter 24 — Branching, Merging, Rebase, and Conflict Resolution `CH-024`

- 24.1 Branching and merging
- 24.2 Rebase and conflict resolution

*Lab themes (indicative):* Conflict-resolution scenarios; a rebase gone wrong and its recovery.

### Chapter 25 — Pull Requests, Code Review, and Branch Protection `CH-025`

- 25.1 Pull requests
- 25.2 Code review
- 25.3 Branch protection

*Lab themes (indicative):* Configure a protected branch with required checks; review a defective pull request.

### Chapter 26 — Release Tags and Versioning `CH-026`

- 26.1 Release tags
- 26.2 Versioning

*Lab themes (indicative):* Versioning policy and release tagging; broken-tag incident.

### Chapter 27 — GitHub Actions `CH-027`

- 27.1 GitHub Actions

*Lab themes (indicative):* Build a CI workflow; troubleshoot a failing workflow; harden workflow permissions.

### Chapter 28 — GitOps Foundations, Repository Security, and Engineering Collaboration `CH-028`

- 28.1 GitOps foundations
- 28.2 Repository security
- 28.3 Engineering collaboration

*Lab themes (indicative):* Secret-leak response; declarative repository layout; collaboration protocol.

---

## Part V — Docker and Container Engineering

**Phase B — Delivery foundations.**  
**Major practical outcome (from the master curriculum):** build and operate a secure multi-container application platform.  
**Projects:** Completes PRJ-02A: Enterprise-Style Container Platform (baseline).  
**Part practical review:** `PR-P05`

### Chapter 29 — Virtualisation, Containers, Namespaces, and cgroups `CH-029`

- 29.1 Virtualisation and containers
- 29.2 Namespaces and cgroups

*Lab themes (indicative):* Build a container by hand from kernel primitives; resource-limit experiment.

### Chapter 30 — Docker Engine, Images, and Layers `CH-030`

- 30.1 Docker Engine
- 30.2 Images and layers

*Lab themes (indicative):* Inspect image layers; storage-driver behaviour and disk pressure.

### Chapter 31 — Dockerfiles, BuildKit and Caching, and Multi-Stage Builds `CH-031`

- 31.1 Dockerfiles
- 31.2 BuildKit and caching
- 31.3 Multi-stage builds

*Lab themes (indicative):* Optimise a slow, bloated build; cache-invalidation incident.

### Chapter 32 — Container Networking and Volumes `CH-032`

- 32.1 Container networking
- 32.2 Volumes

*Lab themes (indicative):* Bridge-network debugging; volume permission failure; data-persistence test.

### Chapter 33 — Docker Compose, Health Checks, and Resource Management `CH-033`

- 33.1 Compose
- 33.2 Health checks
- 33.3 Resource management

*Lab themes (indicative):* Dependency ordering; broken health check; memory-limit kill.

### Chapter 34 — Container Security `CH-034`

- 34.1 Security

*Lab themes (indicative):* Harden a container (non-root, read-only filesystem, capabilities); attack-surface review.

### Chapter 35 — Registries, Image Tagging, and ARM64/AMD64 `CH-035`

- 35.1 Registries
- 35.2 Image tagging
- 35.3 ARM64 and AMD64

*Lab themes (indicative):* Registry authentication failure; multi-architecture build and manifest; tagging policy.

### Chapter 36 — Container Debugging and Production Container Operations `CH-036`

- 36.1 Container debugging
- 36.2 Production container operations

*Lab themes (indicative):* Debug a restart loop without interactive access; production runbook drill.

---

## Part VI — AWS and Cloud Architecture

**Phase C — Cloud and Infrastructure as Code.**  
**Major practical outcome (from the master curriculum):** design and implement a secure multi-tier cloud architecture.  
**Projects:** Feeds PRJ-03 (completes after Part VII).  
**Part practical review:** `PR-P06`

### Chapter 37 — Cloud Computing and AWS Global Infrastructure `CH-037`

- 37.1 Cloud computing
- 37.2 AWS global infrastructure

*Lab themes (indicative):* Map failure domains (Region, Availability Zone); set budget and quota guardrails before any billable lab.

### Chapter 38 — AWS IAM `CH-038`

- 38.1 IAM

*Lab themes (indicative):* Least-privilege policy design; investigate an access-denied failure using policy evaluation logic.

### Chapter 39 — VPC, Subnets, and Route Tables `CH-039`

- 39.1 VPC
- 39.2 Subnets
- 39.3 Route tables

*Lab themes (indicative):* Build a VPC from scratch; routing fault diagnosis.

### Chapter 40 — Internet Gateways, NAT Gateways, Security Groups, and Network ACLs `CH-040`

- 40.1 Internet gateways
- 40.2 NAT gateways
- 40.3 Security groups
- 40.4 Network ACLs

*Lab themes (indicative):* Private-subnet egress; isolate a fault between security groups and network ACLs; NAT cost analysis.

### Chapter 41 — EC2 and EBS `CH-041`

- 41.1 EC2
- 41.2 EBS

*Lab themes (indicative):* Launch and harden an Arm-based instance; snapshot and restore a volume; volume-full incident.

### Chapter 42 — S3 `CH-042`

- 42.1 S3

*Lab themes (indicative):* Bucket policy and encryption; detect and fix accidental public access; lifecycle rules.

### Chapter 43 — Load Balancers and Auto Scaling `CH-043`

- 43.1 Load balancers
- 43.2 Auto Scaling

*Lab themes (indicative):* Load balancer with target health; scale-out under load; failed health check.

### Chapter 44 — Route 53, CloudFront, and ACM `CH-044`

- 44.1 Route 53
- 44.2 CloudFront
- 44.3 ACM

*Lab themes (indicative):* DNS failover record; certificate validation failure; CDN caching incident.

### Chapter 45 — CloudWatch and AWS Cost Management `CH-045`

- 45.1 CloudWatch
- 45.2 AWS cost management

*Lab themes (indicative):* Metrics, alarms, and logs; budget alarms; cost-anomaly investigation.

### Chapter 46 — High Availability and Disaster Recovery `CH-046`

- 46.1 High availability
- 46.2 Disaster recovery

*Lab themes (indicative):* Multi-AZ failover drill; backup and restore test measuring recovery time and recovery point.

---

## Part VII — Infrastructure as Code and Configuration Management

**Phase C — Cloud and Infrastructure as Code.**  
**Major practical outcome (from the master curriculum):** provision and configure repeatable environments from version-controlled code.  
**Projects:** Completes PRJ-03: AWS Infrastructure as Code Platform.  
**Part practical review:** `PR-P07`

### Chapter 47 — Infrastructure as Code Principles and Terraform Architecture `CH-047`

- 47.1 Infrastructure as Code principles
- 47.2 Terraform architecture

*Lab themes (indicative):* Plan/apply lifecycle on a disposable target; inspect the dependency graph.

### Chapter 48 — Providers, Resources, Data Sources, Variables, and Outputs `CH-048`

- 48.1 Providers
- 48.2 Resources and data sources
- 48.3 Variables and outputs

*Lab themes (indicative):* Build a small stack; diagnose validation and provider errors.

### Chapter 49 — Terraform State and Remote State `CH-049`

- 49.1 State
- 49.2 Remote state

*Lab themes (indicative):* State lock and corruption incident; migrate to remote state.

### Chapter 50 — Modules, Workspaces, and Environment Separation `CH-050`

- 50.1 Modules
- 50.2 Workspaces and environment separation

*Lab themes (indicative):* Refactor into modules; compare environment-separation strategies.

### Chapter 51 — Import, Drift, Terraform Testing, and Terraform Security `CH-051`

- 51.1 Import and drift
- 51.2 Terraform testing
- 51.3 Terraform security

*Lab themes (indicative):* Detect and remediate drift; write tests; scan and fix insecure configuration.

### Chapter 52 — Ansible Architecture, Inventories, and Playbooks `CH-052`

- 52.1 Ansible architecture
- 52.2 Inventories
- 52.3 Playbooks

*Lab themes (indicative):* Idempotent playbook; inventory fault.

### Chapter 53 — Roles, Configuration Drift, Idempotency, and Secret Handling `CH-053`

- 53.1 Roles
- 53.2 Configuration drift
- 53.3 Idempotency
- 53.4 Secret handling

*Lab themes (indicative):* Role refactor; drift detection; secret-leak drill.

### Chapter 54 — Infrastructure Automation Pipelines `CH-054`

- 54.1 Infrastructure automation pipelines

*Lab themes (indicative):* Plan-on-pull-request and apply-on-merge pipeline with approvals; recovery from a failed apply.

---

## Part VIII — CI/CD and Release Engineering

**Phase D — Delivery systems, edge, and data.**  
**Major practical outcome (from the master curriculum):** build a complete secure CI/CD delivery system with verified deployments and automated rollback.  
**Projects:** Completes PRJ-04A: Secure Enterprise CI/CD Platform (pipeline through verified rollback).  
**Part practical review:** `PR-P08`

### Chapter 55 — CI/CD Principles and Jenkins Architecture `CH-055`

- 55.1 CI/CD principles
- 55.2 Jenkins architecture
- 55.3 Agents and controllers

*Lab themes (indicative):* Controller and agent setup; executor starvation incident.

### Chapter 56 — Pipeline Design, Jenkinsfiles, and Build Automation `CH-056`

- 56.1 Pipeline design
- 56.2 Jenkinsfiles
- 56.3 Build automation

*Lab themes (indicative):* Declarative pipeline; failing-stage triage; reproducible builds.

### Chapter 57 — Testing, Code Quality, and Security Scanning `CH-057`

- 57.1 Testing
- 57.2 Code quality
- 57.3 Security scanning

*Lab themes (indicative):* Quality gates; flaky-test investigation; failed scan gate.

### Chapter 58 — Image Creation, Registry Publishing, and Artifact Management `CH-058`

- 58.1 Image creation
- 58.2 Registry publishing
- 58.3 Artifact management

*Lab themes (indicative):* Build, publish, and promote; registry authentication failure; artifact traceability.

### Chapter 59 — Deployment Automation and Immutable Releases `CH-059`

- 59.1 Deployment automation
- 59.2 Immutable releases

*Lab themes (indicative):* Scripted deployment; immutable tagging; configuration drift between releases.

### Chapter 60 — Blue-Green, Canary, and Progressive Delivery `CH-060`

- 60.1 Blue-green deployments
- 60.2 Canary releases
- 60.3 Progressive delivery

*Lab themes (indicative):* Blue-green cutover with verification; canary analysis; containing a bad release.

### Chapter 61 — Rollback, Pipeline Security, and Release Governance `CH-061`

- 61.1 Rollback
- 61.2 Pipeline security
- 61.3 Release governance

*Lab themes (indicative):* Automated rollback drill; pipeline credential-leak drill; change-approval policy.

---

## Part IX — Nginx, Edge Infrastructure and TLS

**Phase D — Delivery systems, edge, and data.**  
**Major practical outcome (from the master curriculum):** operate a secure, highly available web edge for multiple application services.  
**Projects:** Adds edge depth to earlier projects; no flagship project completes here.  
**Part practical review:** `PR-P09`

### Chapter 62 — Web Server Architecture and Nginx Internals `CH-062`

- 62.1 Web server architecture
- 62.2 Nginx internals

*Lab themes (indicative):* Worker and event-loop behaviour under load; configuration contexts.

### Chapter 63 — Reverse Proxies, Upstreams, Load Balancing, and HTTP Routing `CH-063`

- 63.1 Reverse proxies
- 63.2 Upstreams
- 63.3 Load balancing
- 63.4 HTTP routing

*Lab themes (indicative):* Multi-service routing; upstream failure behaviour; diagnose 502 and 504 responses from evidence.

### Chapter 64 — Headers, TLS, Certificates, and Renewal `CH-064`

- 64.1 Headers
- 64.2 TLS
- 64.3 Certificates
- 64.4 Renewal

*Lab themes (indicative):* Security headers; automated issuance and renewal; renewal-failure drill.

### Chapter 65 — Unprivileged Containers, File Permissions, and Configuration Validation `CH-065`

- 65.1 Unprivileged containers
- 65.2 File permissions
- 65.3 Configuration validation

*Lab themes (indicative):* Run the proxy unprivileged; certificate file-permission failure; configuration test in CI.

### Chapter 66 — Proxy Troubleshooting and Secure Edge Design `CH-066`

- 66.1 Proxy troubleshooting
- 66.2 Secure edge design

*Lab themes (indicative):* Edge incident playbook; design review of an edge architecture.

---

## Part X — Databases and Stateful Infrastructure

**Phase D — Delivery systems, edge, and data.**  
**Major practical outcome (from the master curriculum):** operate a stateful application environment with tested backup and restoration procedures.  
**Projects:** Completes PRJ-02B: database-operations hardening of the container platform.  
**Part practical review:** `PR-P10`

### Chapter 67 — Database Fundamentals and PostgreSQL Architecture `CH-067`

- 67.1 Database fundamentals
- 67.2 PostgreSQL architecture

*Lab themes (indicative):* Inspect server processes, write-ahead log, and on-disk layout.

### Chapter 68 — Transactions, Indexes, and Connection Pooling `CH-068`

- 68.1 Transactions
- 68.2 Indexes
- 68.3 Connections and pooling

*Lab themes (indicative):* Reproduce isolation anomalies; plan-driven indexing; connection-exhaustion incident.

### Chapter 69 — Persistent Storage and Replication `CH-069`

- 69.1 Persistent storage
- 69.2 Replication

*Lab themes (indicative):* Volume-loss recovery; streaming replication and failover drill.

### Chapter 70 — Backups and Point-in-Time Recovery `CH-070`

- 70.1 Backups
- 70.2 Point-in-time recovery

*Lab themes (indicative):* Logical versus physical backup; recover to a chosen point in time.

### Chapter 71 — Migrations and Schema Compatibility `CH-071`

- 71.1 Migrations
- 71.2 Schema compatibility

*Lab themes (indicative):* Expand-and-contract migration; incompatible migration during a blue-green release.

### Chapter 72 — Redis `CH-072`

- 72.1 Redis

*Lab themes (indicative):* Persistence modes; eviction and memory incident.

### Chapter 73 — Database Monitoring, Security, and Recovery Testing `CH-073`

- 73.1 Database monitoring
- 73.2 Database security
- 73.3 Recovery testing

*Lab themes (indicative):* Slow-query and replica-lag alerts; least-privilege roles; full recovery exercise measuring recovery time and recovery point.

---

## Part XI — Kubernetes and Container Orchestration

**Phase E — Orchestration and platform.**  
**Major practical outcome (from the master curriculum):** deploy, secure, troubleshoot, and operate a Kubernetes-based application platform.  
**Projects:** Completes PRJ-05A: Kubernetes Production Application Platform (cluster, workloads, security, failure drills).  
**Part practical review:** `PR-P11`

### Chapter 74 — Why Orchestration Exists and Kubernetes Architecture `CH-074`

- 74.1 Why orchestration exists
- 74.2 Kubernetes architecture

*Lab themes (indicative):* Build a cluster; trace one request through the API server and controllers.

### Chapter 75 — The Control Plane and Nodes `CH-075`

- 75.1 Control plane
- 75.2 Nodes

*Lab themes (indicative):* Control-plane component failure; node NotReady diagnosis.

### Chapter 76 — Pods, Deployments, and ReplicaSets `CH-076`

- 76.1 Pods
- 76.2 Deployments
- 76.3 ReplicaSets

*Lab themes (indicative):* CrashLoopBackOff and image-pull failures; rolling update and rollback.

### Chapter 77 — Services, Ingress, and Gateway API `CH-077`

- 77.1 Services
- 77.2 Ingress and Gateway API

*Lab themes (indicative):* Selector-mismatch incident; ingress routing fault.

### Chapter 78 — ConfigMaps and Secrets `CH-078`

- 78.1 ConfigMaps
- 78.2 Secrets

*Lab themes (indicative):* Configuration rollout; secret-exposure review.

### Chapter 79 — Storage and Persistent Volumes `CH-079`

- 79.1 Storage
- 79.2 Persistent volumes

*Lab themes (indicative):* Claim stuck in Pending; data persistence across rescheduling.

### Chapter 80 — Probes, Resource Requests and Limits, and Scheduling `CH-080`

- 80.1 Probes
- 80.2 Resource requests and limits
- 80.3 Scheduling

*Lab themes (indicative):* Probe misconfiguration; out-of-memory kills and CPU throttling; unschedulable pod.

### Chapter 81 — Autoscaling `CH-081`

- 81.1 Autoscaling

*Lab themes (indicative):* Horizontal autoscaling under load; autoscaler misbehaviour.

### Chapter 82 — RBAC and Network Policies `CH-082`

- 82.1 RBAC
- 82.2 Network policies

*Lab themes (indicative):* Least-privilege role design; a network policy that silently blocks traffic.

### Chapter 83 — Helm `CH-083`

- 83.1 Helm

*Lab themes (indicative):* Chart authoring; failed upgrade and rollback.

### Chapter 84 — Cluster Security and Kubernetes Troubleshooting `CH-084`

- 84.1 Cluster security
- 84.2 Kubernetes troubleshooting

*Lab themes (indicative):* Pod-level hardening; multi-fault incident worked from evidence.

### Chapter 85 — Cluster Upgrades and Production Operations `CH-085`

- 85.1 Cluster upgrades
- 85.2 Production operations

*Lab themes (indicative):* Version-skew-aware upgrade rehearsal; operational runbooks.

---

## Part XII — GitOps and Platform Engineering

**Phase E — Orchestration and platform.**  
**Major practical outcome (from the master curriculum):** create a reusable internal developer platform that makes application delivery consistent and repeatable.  
**Projects:** Completes PRJ-05B: GitOps increment of the Kubernetes platform.  
**Part practical review:** `PR-P12`

### Chapter 86 — Platform Engineering, Internal Developer Platforms, and Developer Self-Service `CH-086`

- 86.1 Platform engineering fundamentals
- 86.2 Internal developer platforms
- 86.3 Developer self-service

*Lab themes (indicative):* Derive platform requirements from user needs; design a self-service workflow.

### Chapter 87 — GitOps Architecture with Argo CD or Flux `CH-087`

- 87.1 GitOps architecture
- 87.2 Argo CD or Flux

*Lab themes (indicative):* Install and reconcile; drift correction; broken-sync incident.

### Chapter 88 — Environment Promotion, Deployment Templates, and Platform APIs `CH-088`

- 88.1 Environment promotion
- 88.2 Reusable deployment templates
- 88.3 Platform APIs

*Lab themes (indicative):* Promotion pipeline; reusable template; API contract.

### Chapter 89 — Golden Paths, Policy as Code, and Multi-Tenancy `CH-089`

- 89.1 Golden paths
- 89.2 Policy as code
- 89.3 Multi-tenancy

*Lab themes (indicative):* Golden path for a new service; policy-violation drill; tenant-isolation test.

### Chapter 90 — Platform Security, Developer Experience, and Platform Observability `CH-090`

- 90.1 Platform security
- 90.2 Developer experience
- 90.3 Platform observability

*Lab themes (indicative):* Platform threat model; measure developer experience; platform service-level objectives.

---

## Part XIII — Observability and Site Reliability Engineering

**Phase F — Reliability and security.**  
**Major practical outcome (from the master curriculum):** build an observability platform, define service objectives, generate incidents, and demonstrate recovery.  
**Projects:** Completes PRJ-06: Observability and SRE Platform, and PRJ-05C: monitoring increment of the Kubernetes platform.  
**Part practical review:** `PR-P13`

### Chapter 91 — Monitoring and Observability `CH-091`

- 91.1 Monitoring
- 91.2 Observability

*Lab themes (indicative):* Instrument a service; blind-spot analysis.

### Chapter 92 — Metrics, Logs, and Distributed Tracing `CH-092`

- 92.1 Metrics
- 92.2 Logs
- 92.3 Distributed tracing

*Lab themes (indicative):* Request, error, and duration metrics; structured logs; trace a slow request.

### Chapter 93 — Prometheus, Grafana, and Alertmanager `CH-093`

- 93.1 Prometheus
- 93.2 Grafana
- 93.3 Alertmanager

*Lab themes (indicative):* Scrape and alert; alert-noise reduction; missing-telemetry incident.

### Chapter 94 — OpenTelemetry and Service Health `CH-094`

- 94.1 OpenTelemetry
- 94.2 Service health

*Lab themes (indicative):* Instrument with OpenTelemetry; define a service health model.

### Chapter 95 — SLIs, SLOs, SLAs, and Error Budgets `CH-095`

- 95.1 SLIs
- 95.2 SLOs
- 95.3 SLAs
- 95.4 Error budgets

*Lab themes (indicative):* Derive objectives from data; burn-rate alerts; error-budget policy.

### Chapter 96 — Incident Response and Postmortems `CH-096`

- 96.1 Incident response
- 96.2 Postmortems

*Lab themes (indicative):* Run an incident with defined roles; write a blameless postmortem.

### Chapter 97 — Capacity Planning, Reliability, Disaster Recovery, and Performance Engineering `CH-097`

- 97.1 Capacity planning
- 97.2 Reliability
- 97.3 Disaster recovery
- 97.4 Performance engineering

*Lab themes (indicative):* Load test and capacity model; disaster-recovery drill; bottleneck hunt.

---

## Part XIV — DevSecOps and Software Supply Chain Security

**Phase F — Reliability and security.**  
**Major practical outcome (from the master curriculum):** establish a secure software delivery pipeline with verifiable security controls.  
**Projects:** Completes PRJ-04B (SBOM, signing, verification) and PRJ-07: Internal Developer Platform.  
**Part practical review:** `PR-P14`

### Chapter 98 — Security Engineering Fundamentals and Threat Modelling `CH-098`

- 98.1 Security engineering fundamentals
- 98.2 Threat modelling

*Lab themes (indicative):* Threat-model a service from a data-flow diagram.

### Chapter 99 — IAM, Least Privilege, and Secrets Management `CH-099`

- 99.1 IAM
- 99.2 Least privilege
- 99.3 Secrets management

*Lab themes (indicative):* Remediate an over-privileged role; secret-rotation drill.

### Chapter 100 — Container Security, Image Scanning, and Dependency Scanning `CH-100`

- 100.1 Container security
- 100.2 Image scanning
- 100.3 Dependency scanning

*Lab themes (indicative):* Triage scan findings; vulnerable-dependency gate.

### Chapter 101 — SAST, DAST, and SBOM `CH-101`

- 101.1 SAST and DAST
- 101.2 SBOM

*Lab themes (indicative):* Static and dynamic testing in a pipeline; generate and query an SBOM.

### Chapter 102 — Image Signing, Provenance, Attestations, and Supply-Chain Security `CH-102`

- 102.1 Image signing
- 102.2 Provenance and attestations
- 102.3 Supply-chain security

*Lab themes (indicative):* Sign and verify images; reject an unsigned artifact; provenance check.

### Chapter 103 — Policy Enforcement, Runtime Security, Audit Logging, and Security Incident Response `CH-103`

- 103.1 Policy enforcement
- 103.2 Runtime security
- 103.3 Audit logging
- 103.4 Security incident response

*Lab themes (indicative):* Admission policy; runtime detection drill; audit-trail investigation; security incident exercise.

---

## Part XV — Senior DevOps Engineering

**Phase G — Senior and architect.**  
**Major practical outcome (from the master curriculum):** operate and improve a complex multi-service platform under realistic failure conditions.  
**Projects:** No flagship project completes here; the part feeds PRJ-08.  
**Part practical review:** `PR-P15`

### Chapter 104 — Distributed Systems, Failure Domains, and Fault Tolerance `CH-104`

- 104.1 Distributed systems
- 104.2 Failure domains
- 104.3 Fault tolerance

*Lab themes (indicative):* Partial-failure experiments with timeouts and retries; failure-domain mapping.

### Chapter 105 — High Availability, Resilience, Scalability, and Performance `CH-105`

- 105.1 High availability
- 105.2 Resilience
- 105.3 Scalability
- 105.4 Performance

*Lab themes (indicative):* Fault-injection experiments; capacity tests; retry-storm incident.

### Chapter 106 — Cost Optimisation, Technical Debt, and Operational Excellence `CH-106`

- 106.1 Cost optimisation
- 106.2 Technical debt
- 106.3 Operational excellence

*Lab themes (indicative):* Cost review; technical-debt register; operational readiness review.

### Chapter 107 — Incident Command, Change Management, and Reliability Trade-offs `CH-107`

- 107.1 Incident command
- 107.2 Change management
- 107.3 Reliability trade-offs

*Lab themes (indicative):* Incident commander simulation; change request with risk assessment; trade-off memo.

### Chapter 108 — Engineering Leadership and Technical Decision-Making `CH-108`

- 108.1 Engineering leadership
- 108.2 Technical decision-making

*Lab themes (indicative):* Decision-record exercise; code-review mentoring simulation; stakeholder communication.

---

## Part XVI — Cloud and DevOps Architecture

**Phase G — Senior and architect.**  
**Major practical outcome (from the master curriculum):** design, implement, defend, and document a complete enterprise-style cloud platform.  
**Projects:** Completes PRJ-08: Enterprise Cloud Architecture Capstone.  
**Part practical review:** `PR-P16`

### Chapter 109 — Requirements Analysis, Architecture Principles, and Architecture Diagrams `CH-109`

- 109.1 Requirements analysis
- 109.2 Architecture principles
- 109.3 Architecture diagrams

*Lab themes (indicative):* Elicit requirements from an ambiguous brief; context, container, and component diagrams.

### Chapter 110 — Network, Security, Compute, and Storage Architecture `CH-110`

- 110.1 Network architecture
- 110.2 Security architecture
- 110.3 Compute architecture
- 110.4 Storage architecture

*Lab themes (indicative):* Layer-by-layer design review; trade-off matrix.

### Chapter 111 — Data, Deployment, and Observability Architecture `CH-111`

- 111.1 Data architecture
- 111.2 Deployment architecture
- 111.3 Observability architecture

*Lab themes (indicative):* Data architecture against recovery objectives; deployment and observability architecture.

### Chapter 112 — Multi-AZ, Multi-Region, and Disaster Recovery Design `CH-112`

- 112.1 Multi-AZ design
- 112.2 Multi-region design
- 112.3 Disaster recovery

*Lab themes (indicative):* Multi-AZ design with a failure test; disaster-recovery strategy comparison with cost.

### Chapter 113 — Cost Architecture, Architecture Decision Records, and Technology Selection `CH-113`

- 113.1 Cost architecture
- 113.2 Architecture Decision Records
- 113.3 Technology selection

*Lab themes (indicative):* Cost model; write decision records; technology-selection matrix.

### Chapter 114 — Risk Analysis, Design Reviews, and Architecture Governance `CH-114`

- 114.1 Risk analysis
- 114.2 Design reviews
- 114.3 Architecture governance

*Lab themes (indicative):* Risk register; run a design review; governance model.

---

## Part XVII — Real-World AirDive Engineering Case Studies

**Phase H — Case studies and graduation.**  
**Practical outcome (proposed; not specified in the master curriculum):** evidence-based case studies in which verified facts, hypotheses, and proposed solutions are strictly separated, each converted into a runbook or control.  
**Projects:** Case studies are harvested as the matching technical parts are completed and compiled here. Every case study requires evidence supplied by the learner; none is written from assumption.  
**Part practical review:** `PR-P17`

### Chapter 115 — Application Runtime and Container Failures `CH-115`

- 115.1 `CS-01` Node.js ESM runtime errors
- 115.2 `CS-02` Docker restart loops
- 115.3 `CS-03` Unhealthy frontend containers
- 115.4 `CS-04` Docker storage pressure
- 115.5 `CS-10` Health-check mismatches

*Lab themes (indicative):* Evidence-based reconstruction, root-cause analysis, runbook, and prevention control for each case.

### Chapter 116 — Pipeline, Registry, and Artifact Failures `CH-116`

- 116.1 `CS-05` Jenkins pipeline failures
- 116.2 `CS-06` GHCR authentication
- 116.3 `CS-07` Image architecture mismatches
- 116.4 `CS-13` Compose interpolation failures
- 116.5 `CS-18` CI quality gates

*Lab themes (indicative):* Same method; focus on build and delivery-path failures.

### Chapter 117 — Edge, Network, and Browser-Boundary Failures `CH-117`

- 117.1 `CS-08` Nginx configuration problems
- 117.2 `CS-09` TLS certificate permissions
- 117.3 `CS-11` CORS failures
- 117.4 `CS-12` DNS resolution issues

*Lab themes (indicative):* Same method; focus on proxy, certificate, DNS, and cross-origin failures.

### Chapter 118 — Release Strategy, Rollback, and Verification `CH-118`

- 118.1 `CS-14` Blue-green deployment
- 118.2 `CS-15` Canary releases
- 118.3 `CS-16` Rollback
- 118.4 `CS-17` Deployment verification

*Lab themes (indicative):* Same method; focus on release strategy and recovery.

---

## Back matter (planned)

- **Appendix A** — Laboratory environment setup and safety checklist
- **Appendix B** — Engineering templates: Architecture Decision Record, runbook, postmortem, change request, design review, threat model
- **Appendix C** — Command and configuration reference (version-tagged and sourced)
- **Appendix D** — Interview question bank and answer frameworks
- **Appendix E** — Cost and cleanup checklists
- **Appendix F** — Reference architecture catalogue
- Glossary · References · Index
