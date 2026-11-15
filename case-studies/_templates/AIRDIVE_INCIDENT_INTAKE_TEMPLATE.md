---
incident_id: INC-AD-NNN
case_study: CS-NN            # subject from case-studies/README.md, if one applies
date_range_utc: "YYYY-MM-DD HH:MM to YYYY-MM-DD HH:MM"
systems: []                  # use placeholders, not real hostnames
severity: ""                 # impact in your own words; no invented scale
redaction_checked: false
---

# INC-AD-NNN — <short title>

> **Rules.** Facts need evidence. Memory-only statements go under *Recollection (unverified)*. No secrets, tokens, private keys, customer data, internal hostnames, or internal IP addresses. Evidence gathering is read-only.

## 1. Evidence inventory

| ID | Type (log, diff, build, screenshot, metric) | Source and location | Timestamp (UTC) | Redacted? |
|---|---|---|---|---|
| E1 | | | | |

## 2. Timeline (UTC)

| Time | Event | Evidence ID |
|---|---|---|
| | | E? |

## 3. Verified facts
Each statement cites at least one evidence ID.

- F1: … (E?)

## 4. Recollection (unverified)
What you remember that no evidence currently supports.

- R1: …

## 5. Hypotheses
For each: confidence (low/medium/high), what evidence supports it, what would falsify it, and the next diagnostic.

| ID | Hypothesis | Supporting evidence | Falsified by | Next diagnostic |
|---|---|---|---|---|
| H1 | | | | |

## 6. Root cause
State only what the evidence supports. If it is not established, write **Not established**, with the best hypothesis and what is missing.

## 7. Actions actually taken
What was done during the incident, in order, with timestamps where known.

## 8. Proposed solutions (not yet implemented)
Each proposal: expected effect, risk, how its effect will be verified, and the control it becomes (runbook, alert, test, gate, architecture change).

## 9. Open questions
