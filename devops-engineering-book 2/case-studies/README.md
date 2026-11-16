# Case Studies (Part XVII)

Case studies come from **real AirDive incidents and infrastructure history**. This repository holds none yet: the master prompt names the subjects, but no incident evidence has been supplied. A case study is written only from evidence you provide.

## Rules

1. **Facts need evidence.** A fact has a source (log line, commit SHA, build number, configuration diff, timestamp, screenshot) recorded in the intake record.
2. **Three separate sections in every case study:** *Verified facts*, *Hypotheses*, *Proposed solutions*. Nothing moves from hypothesis to fact without evidence.
3. **Recollection is allowed but labelled.** Anything that rests on memory alone is tagged **Recollection (unverified)**.
4. **Redact before you share.** No secrets, tokens, private keys, customer data, internal hostnames, or internal IP addresses in chat, commits, or evidence files. Replace them with stable placeholders (for example, `HOST-A`) and keep a private mapping.
5. **Read-only evidence gathering.** Collecting evidence from AirDive must not change anything. Failure injection uses the reference application, never AirDive production.
6. **Every case study ends in a control**: a runbook, an alert, a test, a pipeline gate, or an architectural change, each with a way to verify it works.

## How to log an incident

Copy [`_templates/AIRDIVE_INCIDENT_INTAKE_TEMPLATE.md`](_templates/AIRDIVE_INCIDENT_INTAKE_TEMPLATE.md) to `INC-AD-<nnn>-<slug>.md`, fill it in as soon as the incident is fresh (before the evidence expires), then use `CASE STUDY` mode to turn it into a documented case study. Evidence ages quickly: container logs rotate, CI build logs expire, and memory fades.

## Subject register

| ID | Subject | Chapter | Evidence received |
|---|---|---|---|
| CS-01 | Node.js ESM runtime errors | CH-115 | No |
| CS-02 | Docker restart loops | CH-115 | No |
| CS-03 | Unhealthy frontend containers | CH-115 | No |
| CS-04 | Docker storage pressure | CH-115 | No |
| CS-05 | Jenkins pipeline failures | CH-116 | No |
| CS-06 | GHCR authentication | CH-116 | No |
| CS-07 | Image architecture mismatches | CH-116 | No |
| CS-08 | Nginx configuration problems | CH-117 | No |
| CS-09 | TLS certificate permissions | CH-117 | No |
| CS-10 | Health-check mismatches | CH-115 | No |
| CS-11 | CORS failures | CH-117 | No |
| CS-12 | DNS resolution issues | CH-117 | No |
| CS-13 | Compose interpolation failures | CH-116 | No |
| CS-14 | Blue-green deployment | CH-118 | No |
| CS-15 | Canary releases | CH-118 | No |
| CS-16 | Rollback | CH-118 | No |
| CS-17 | Deployment verification | CH-118 | No |
| CS-18 | CI quality gates | CH-116 | No |
