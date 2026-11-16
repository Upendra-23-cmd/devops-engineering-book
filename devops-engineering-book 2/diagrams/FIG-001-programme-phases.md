# FIG-001 — Programme phases and project gates

```mermaid
flowchart TD
    A["Phase A: Foundations (Parts I-III, Ch 1-22)"] --> B["Phase B: Delivery foundations (Parts IV-V, Ch 23-36)"]
    B --> C["Phase C: Cloud and Infrastructure as Code (Parts VI-VII, Ch 37-54)"]
    C --> D["Phase D: Delivery systems, edge, and data (Parts VIII-X, Ch 55-73)"]
    D --> E["Phase E: Orchestration and platform (Parts XI-XII, Ch 74-90)"]
    E --> F["Phase F: Reliability and security (Parts XIII-XIV, Ch 91-103)"]
    F --> G["Phase G: Senior and architect (Parts XV-XVI, Ch 104-114)"]
    G --> H["Phase H: Case studies and graduation (Part XVII, Ch 115-118)"]
    H --> GRAD["Final evaluation: architecture challenge, live troubleshooting, portfolio defence"]

    A -.-> PRJ01["PRJ-01 Linux and network operations"]
    B -.-> PRJ02A["PRJ-02A Container platform"]
    C -.-> PRJ03["PRJ-03 AWS Infrastructure as Code platform"]
    D -.-> PRJ04A["PRJ-04A CI/CD through verified rollback"]
    D -.-> PRJ02B["PRJ-02B Database operations hardening"]
    E -.-> PRJ05A["PRJ-05A Kubernetes platform"]
    E -.-> PRJ05B["PRJ-05B GitOps"]
    F -.-> PRJ06["PRJ-06 Observability and SRE platform"]
    F -.-> PRJ05C["PRJ-05C Monitoring"]
    F -.-> PRJ04B["PRJ-04B SBOM, signing, verification"]
    F -.-> PRJ07["PRJ-07 Internal developer platform"]
    G -.-> PRJ08["PRJ-08 Cloud architecture capstone"]

    classDef project fill:#eef6ff,stroke:#3b6ea5;
    class PRJ01,PRJ02A,PRJ03,PRJ04A,PRJ02B,PRJ05A,PRJ05B,PRJ06,PRJ05C,PRJ04B,PRJ07,PRJ08 project;
```

*Caption.* Solid arrows show book order. Dotted arrows show the phase in which a project increment completes. Increments are explained in [`../projects/PORTFOLIO.md`](../projects/PORTFOLIO.md).

*Source of record:* this file. *Last reviewed:* 2026-11-14.
