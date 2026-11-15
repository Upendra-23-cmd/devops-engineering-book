---
id: BASE-01
title: Baseline assessment (placement and verification of claimed skills)
status: Drafted
version: 0.1.0
last_updated: 2026-11-14
mode: Assessment (answer key is held by the mentor and is not stored here)
---

# BASE-01 — Baseline assessment

**Purpose.** The master prompt lists what you have worked with, but working on a system is not the same as understanding it. This assessment replaces assumption with evidence. It decides where the first challenge labs start and which of your claimed skills can be marked *verified*.

**This is not a pass/fail test.** A confident wrong answer and an honest "I don't know" are both useful; a guess presented as certainty is the only unhelpful answer.

## Rules

1. **Closed-book first pass.** Answer from memory, without documentation, search, or AI assistance. Do this pass in one or two sittings (about 90–120 minutes in total).
2. **Optional second pass.** You may then look things up and revise. Mark any revised answer **[2P]** so the first-pass answer is not lost.
3. **Short answers.** Three to eight sentences or a short list per question. Include the exact command or setting where the question asks for one.
4. **Rate your confidence** for every answer from 1 (guessing) to 5 (certain), and state the **source** of the answer: *experience* (you have done or seen it), *study* (read or watched), or *guess*.
5. **No production access is needed.** Do not run anything against AirDive production for this assessment. Do not paste secrets, tokens, private keys, customer data, internal hostnames, or internal IP addresses.
6. Answer format: copy the table at the end, or reply in chat with `Q<n>: answer / confidence / source`.

Each question is tagged with the dimensions it probes: **D1** conceptual understanding, **D2** independent implementation, **D3** troubleshooting and root-cause analysis, **D4** production operations and reliability, **D5** architecture and engineering judgement.

---

## Part A — Scenario questions

**Q1 (D3).** A container started by Docker Compose keeps restarting. You have shell access to the host, but the container exits too quickly to open a shell inside it. List the first five diagnostic actions you would take, in order. For each, give the exact command or UI action, what you expect it to reveal, and what result would make you choose a different next step.

**Q2 (D1).** Explain the difference between (a) a container whose main process exits and (b) a running container whose health check is failing. For each, describe how it appears in `docker ps` or `docker compose ps`, what Docker does about it by default, and how it interacts with a `restart:` policy and with `depends_on` using `condition: service_healthy`.

**Q3 (D1).** Trace what happens, in order, from a user typing `https://app.example.com/dashboard` into a browser until the first byte of the HTML response arrives. Assume public DNS, an Nginx reverse proxy on an EC2 instance, and a Node.js container behind it. Cover each protocol layer you rely on, where each connection terminates, and what can fail at each step.

**Q4 (D1, D2).** (a) How many IPv4 addresses are in `10.0.4.0/22`, and what are the first and last addresses of the range? (b) A cloud subnet using such a block does not give you every address for your instances. Name the provider you are describing, say what is reserved, and say why.

**Q5 (D2, D3).** An application running as user ID 1000, inside a container or on a host, cannot read `/etc/ssl/private/app.key`, which is owned by `root:ssl-cert` with mode `0640`. List at least three different ways to restore access and state the security trade-off of each. Which would you choose for a production Nginx container, and why?

**Q6 (D1, D3).** A Node.js container ignores `docker stop` for ten seconds and is then killed. Give two plausible causes. Explain how the shell form versus the exec form of `CMD`, and PID 1 behaviour, contribute. State how you would fix each cause.

**Q7 (D1, D2).** Explain what an image layer is and how Docker's build cache decides whether to reuse one. A Dockerfile copies the whole source tree and then runs `npm ci`. Say what is wrong with that ordering and give the corrected ordering for a Node.js application.

**Q8 (D1, D3).** Your build pipeline runs on an amd64 agent, and your production hosts are arm64 (Graviton). Describe what happens if you push and run an image built only for amd64 on those hosts. Say how you would detect the mismatch before deploying and give two ways to produce an image that works on both architectures.

**Q9 (D1, D4).** Explain the roles of the Jenkins controller and of agents. Why is running builds on the controller considered poor practice? What risks does it create for credentials and for availability?

**Q10 (D5, D4).** Compare blue-green and canary deployments: what each protects against, what each costs, and how rollback works in each. Then explain what happens to both strategies when a release includes a database schema change that is not backward compatible, and describe one technique that makes such a change safe.

**Q11 (D1, D3).** A teammate force-pushes a rebased shared branch, and your local work now conflicts with the remote history. Explain why rebasing shared history is hazardous, how you would recover your own commits using local Git data, and which branch-protection setting would have prevented the force-push.

**Q12 (D1, D5).** In AWS IAM, what is the difference between an identity-based policy and a resource-based policy? Describe how a request is evaluated when there is an explicit deny, an allow, and no matching statement. Give an example in which a role has `s3:GetObject` allowed but the request is still denied.

**Q13 (D2, D3).** A browser shows no certificate warning, but `curl` reports `unable to get local issuer certificate` when calling the same HTTPS endpoint. What is the most likely cause? How would you confirm it with OpenSSL (say what output you would look for)? How would you fix it on an Nginx server?

**Q14 (D1, D4).** What is the difference between a logical backup (`pg_dump`) and a physical base backup of PostgreSQL? What must be configured in advance to perform point-in-time recovery? What must a restore test prove before you can say your backups work?

**Q15 (D3).** A Linux server reports `No space left on device` when creating files, but `df -h` shows 40% of space free. State your leading hypothesis, how you would confirm it, and two ways to find the cause.

**Q16 (D4, D5).** Define SLI, SLO, SLA, and error budget. For a login API, propose one SLI, one SLO with a time window, and the resulting error budget. State what the team should do when the budget is exhausted.

---

## Part B — Architecture recall (AirDive)

Do this from memory first. Mark every statement **V** (verified: you have a log, diff, or configuration that shows it), **B** (believed: no evidence to hand), or **U** (unknown). Use placeholders such as `HOST-A` instead of real hostnames or addresses.

**B1.** Draw, as a Mermaid diagram or plain text, the **production request path** of one AirDive service, from client to every data store. Mark each hop with its port and protocol, and say where TLS terminates.

**B2.** Draw the **delivery path** from commit to running container. Say where each secret and each piece of configuration comes from.

**B3.** List every **stateful component** (databases, caches, volumes, buckets). For each, say whether a backup exists, when a restore was last *tested* (not merely taken), and what the result was.

**B4.** Name the **three incidents that taught you the most**. For each: the symptom in one sentence, the root cause as you currently believe it, and an evidence tag (V, B, or U). These become candidates for the case-study register.

**B5.** List at least **five things you do not know** about your own system.

---

## Answer sheet

| Q | Answer | Confidence (1–5) | Source (experience / study / guess) |
|---|---|---|---|
| Q1 | | | |
| Q2 | | | |
| Q3 | | | |
| Q4 | | | |
| Q5 | | | |
| Q6 | | | |
| Q7 | | | |
| Q8 | | | |
| Q9 | | | |
| Q10 | | | |
| Q11 | | | |
| Q12 | | | |
| Q13 | | | |
| Q14 | | | |
| Q15 | | | |
| Q16 | | | |

## What happens next

The mentor scores each answer on the dimensions it probes, compares your confidence with your accuracy (calibration matters as much as correctness), updates the *claimed versus verified* register in [`PROGRESS.md`](../../PROGRESS.md), and chooses where the first challenge labs start. The answer key is not stored in this repository.
