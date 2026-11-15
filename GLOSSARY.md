# Glossary

**Last updated:** 2026-11-14 · Entries are added chapter by chapter. Each entry names the place where the term is introduced.

| Term | Definition | Introduced |
|---|---|---|
| **Batch (release)** | A group of changes released together. Not the same as *batch processing* in computing, where jobs are submitted and run later without interaction. | CH-001 §1.1.1 |
| **Batch size** | How much change goes into one release. | CH-001 §1.1.1 |
| **Change lead time** | In DORA's model, the time from a code commit to a successful production deployment [REF-001]. Distinct from the broader *lead time* below, whose start and end points you define for your own measurement. | CH-001 §1.0.1 |
| **CI/CD** | Continuous integration and continuous delivery (or deployment): practices that build and test every change automatically and keep software releasable. Defined fully in `CH-003`. | CH-001 (forward reference) |
| **Deployment frequency** | How often changes reach production. One of DORA's throughput measures. | CH-001 §1.0.1 |
| **DevOps** | *Provisional definition:* a set of cultural and technical practices that aim to shorten the time from change to production while keeping the system reliable, by sharing ownership between development and operations. Definitions vary; §1.2 discusses them. | CH-001 §1.0.1 |
| **DORA** | DevOps Research and Assessment: a research programme on software delivery performance. | CH-001 §1.0.1 |
| **Flow efficiency** | Process time ÷ lead time. Value stream mapping literature also calls it *process cycle efficiency*. | CH-001 §1.1.1 |
| **Handoff** | Transfer of work between people, teams, or functions. | CH-001 §1.1.1 |
| **Lead time** | Elapsed time from the start of an item (as you define it) to its delivery to users. | CH-001 §1.1.1 |
| **Little's Law** | For a stable system, average number of items in the system = average arrival rate × average time in the system (L = λW). For delivery: average lead time = average WIP ÷ average throughput. | CH-001 §1.1.1 |
| **M/M/1 queue** | The simplest standard queueing model: one server, random (Poisson) arrivals, and exponentially distributed service times. | CH-001 §1.1.1 |
| **Plan-driven development** | Work organised into phases completed largely in order, with sign-off between phases; often called "waterfall". | CH-001 §1.1.1 |
| **Process time** | Time an item is actively being worked on. | CH-001 §1.1.1 |
| **Queue** | Work waiting for a resource: a person, an environment, an approval, or a release window. | CH-001 §1.1.1 |
| **SRE (site reliability engineering)** | An approach to operating services that treats operations as a software-engineering problem. Defined in §1.1.5 and Part XIII (planned). | CH-001 (forward reference) |
| **Software crisis** | The term associated with the 1968 NATO conference for the concern that large software systems were late, over budget, and unreliable. | CH-001 §1.1.1 |
| **Throughput** | Items completed per unit of time. | CH-001 §1.1.1 |
| **Utilisation (ρ)** | The fraction of time a resource is busy. | CH-001 §1.1.1 |
| **Value stream map** | A diagram of the steps and waiting between a request and its delivery, with the time spent in each. | CH-001 §1.1.1 |
| **Waterfall (term)** | The label later attached to the simplified, single-pass sequential lifecycle. | CH-001 §1.1.1 |
| **Work in progress (WIP)** | Items started but not finished. | CH-001 §1.1.1 |
