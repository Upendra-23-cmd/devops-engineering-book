# References

**Last updated:** 2026-11-16

Only sources that were actually opened are listed. Each carries a **verification level**, because "I saw it cited" is weaker than "I read it".

| Level | Meaning |
|---|---|
| **Primary, read** | The primary page was fetched and read |
| **Primary, excerpt only** | A primary source was seen only as a search-result excerpt; the full text was not opened |
| **Secondary only** | Verified only through secondary descriptions; the original was not opened |

Access dates are given per entry (REF-001 to REF-006: **2026-11-14**; REF-007 and REF-008: **2026-11-16**). Quotation policy: paraphrase; no long quotations (`EDITORIAL_GUIDELINES.md` §9).

## Entries

### REF-001 — DORA software delivery performance metrics
- *A history of DORA's software delivery metrics.* DORA. <https://dora.dev/insights/dora-metrics-history/> (reached from `https://dora.dev/guides/dora-metrics/history`).
- *DORA's software delivery performance metrics.* DORA. <https://dora.dev/guides/dora-metrics/>
- **Used for:** the five-measure model (throughput: change lead time, deployment frequency, failed deployment recovery time; instability: change fail rate, deployment rework rate); the 2024 update that added rework rate; the 2023 renaming of *mean time to restore*; the definition of change lead time as the time from code commit to successful production deployment. Chapter 1 §1.0.1.
- **Verification:** history page — *Primary, read*. Metrics guide — *Primary, excerpt only*.
- **Note on conflicting sources.** Several secondary explainers disagreed about the year in which rework rate was added (2024 versus 2025). The primary DORA page was used. Re-check DORA's pages before drafting §1.2.4, because the model has changed before.

### REF-002 — The 1968 NATO Software Engineering Conference
- Randell, B. *Fifty Years of Software Engineering — or — The View from Garmisch.* arXiv:1805.02742. <https://arxiv.org/pdf/1805.02742>
- The conference reports are archived by Brian Randell at Newcastle University (<http://homepages.cs.ncl.ac.uk/brian.randell/NATO/NATOReports/>). This archive appeared in search results and was **not opened**.
- **Used for:** the place and date of the conference (Garmisch, Germany, October 1968), its sponsorship by the NATO Science Committee, its association with the "software crisis", and a participant's account that the title *software engineering* was chosen deliberately to provoke. Chapter 1 §1.1.1.
- **Verification:** *Primary-adjacent* (a participant's retrospective), *excerpt only*. Read the retrospective in full, and open the archived reports, before the Part I review.

### REF-003 — Royce (1970)
- Royce, W. W. *Managing the Development of Large Software Systems.* Proceedings of IEEE WESCON, August 1970. Pagination differs between sources: reprints show pages 1–9; bibliographic records show pages 328–338 of the proceedings.
- Reprint excerpt: <https://faculty.washington.edu/hazeline/misc/reserve/royce_waterfall.pdf> (seen as a search-result excerpt; automated access to the full file was blocked).
- Secondary, for the attribution of the term "waterfall": *Winston W. Royce*, Wikipedia (<https://en.wikipedia.org/wiki/Winston_W._Royce>), which cites Bell, T. E. and Thayer, T. A., *Software requirements: Are they really a problem?*, 2nd International Conference on Software Engineering, 1976. The 1976 paper was **not opened**.
- **Used for:** that the paper presents a sequential scheme, describes implementing it as a single pass as risky, locates the risk in late testing, and adds further features to reduce risk. The statement that "waterfall" first appeared in 1976 is **hedged in the text** ("one account suggests") because it rests on secondary sources.
- **Verification:** *Primary, excerpt only* for the paper's own statements; *Secondary only* for the 1976 attribution and for the summary of iteration and a pilot. Open the full paper before the chapter is technically reviewed.

### REF-004 — Little's Law
- Little, J. D. C. (1961). *A Proof for the Queuing Formula: L = λW.* Operations Research 9(3): 383–387. DOI 10.1287/opre.9.3.383. Bibliographic record and abstract: <https://econpapers.repec.org/RePEc:inm:oropre:v:9:y:1961:i:3:p:383-387>
- **Used for:** the statement of L = λW and its conditions (stationarity, finite means). Chapter 1 §1.1.1, mechanism 2.
- **Verification:** *Primary, bibliographic record and abstract*; the full text was not opened.

### REF-005 — M/M/1 queue results
- Virtamo, J. *38.3143 Queueing Theory: The M/M/* queue.* Lecture notes, Helsinki University of Technology. <https://www.netlab.tkk.fi/opetus/s38143/luennot/E_mm1jono.pdf>
- **Used for:** mean time in system 1/(μ − λ) = (1/μ) · 1/(1 − ρ). Chapter 1 §1.1.1, mechanism 3.
- **Verification:** *Secondary only* (university lecture notes), *excerpt only*. The result is standard and was additionally checked by the author's own simulation (not a source; the script is unpublished).

### REF-006 — Value stream mapping terms
- Rother, M. and Shook, J. *Learning to See: Value Stream Mapping to Add Value and Eliminate Muda.* Lean Enterprise Institute. The publication year is given as 1998 or 1999 in different citations; confirm against the book's copyright page.
- Secondary summary consulted: <https://resources.rework.com/libraries/process-management/value-stream-mapping> (a vendor article; low authority).
- **Used for:** the terms *lead time*, *process time*, and *process cycle efficiency* (= process time ÷ lead time, equivalent to *flow efficiency* as used in this book).
- **Verification:** *Secondary only.* The book was not opened. Open it before the chapter is technically reviewed.

### REF-007 — Google SRE book, Chapter 1 (Introduction)
- Beyer, B., Jones, C., Petoff, J., and Murphy, N. R. (eds.). *Site Reliability Engineering: How Google Runs Production Systems.* O'Reilly Media, 2016. Chapter 1, *Introduction*, written by Benjamin Treynor Sloss. Web edition: <https://sre.google/sre-book/introduction/> (reached from `https://sre.google/sre-book/`). Accessed **2026-11-16**.
- **Used for:** why development and operations were divided; the direct and indirect costs of the split; the conflict between launching changes and keeping the service stable; launch and change gates and the ways development teams adapt around them; Google SRE's report that roughly 70% of its outages stem from changes to a live system; automation of progressive rollouts, detection, and rollback; the error-budget idea (forward reference to `CH-095`); the statement that the term DevOps emerged in late 2008 (reserved for §1.1.5). Chapter 1 §1.1.2.
- **Verification:** *Primary, read* (the chapter page was fetched and read in full). The figures describe Google's experience as of early 2016 and are not universal constants.
- **Licence:** the web edition is licensed CC BY-NC-ND 4.0. Cite and paraphrase; do not reproduce passages.

### REF-008 — DORA, Streamlining change approval
- *Streamlining change approval.* DORA capability page (the page shows a last-updated date of 30 October 2025). <https://dora.dev/capabilities/streamlining-change-approval/>. Accessed **2026-11-16**.
- The page cites the 2019 *Accelerate State of DevOps Report* (<https://dora.dev/research/2019/dora-report/>), which was seen only as a search-result excerpt and **not opened**.
- **Used for:** the description of change management as a primary risk control and of segregation of duties; DORA's finding that external approval boards have a negative association with delivery performance and no evidence of lower change failure rates; the mechanism of larger, less frequent batches; the listed pitfalls (including responding to problems by adding process); the recommended practices (peer review, automation, treating the development platform as a product, making the normal path usable for emergencies); the revised role of the CAB. Chapter 1 §1.1.2.
- **Verification:** the capability page — *Primary, read*. The 2019 report — *Primary, excerpt only*. For the strength of the evidence, see REF-009: DORA's findings come from survey data and describe associations across organisations.
- **Licence:** DORA site content is licensed CC BY 4.0; attribute and paraphrase.

### REF-009 — DORA research methodology
- *Accelerate State of DevOps Report 2024.* DORA, Google Cloud. <https://services.google.com/fh/files/misc/2024_final_dora_report.pdf> (executive-summary excerpt: data are collected through an annual, worldwide survey of professionals and analysed with statistical methods; the 2024 edition added in-depth interviews).
- *DORA DevOps guidebook, chapter 1.* Google Cloud. <https://services.google.com/fh/files/misc/devops_guidebook_chapter1.pdf> (excerpt: a cross-sectional, theory-based research design; structural equation modelling used from 2015 onwards).
- **Used for:** characterising the strength of DORA's evidence: association in survey data across organisations, not a controlled experiment. Chapter 1 §1.1.2, mechanism 7. Accessed **2026-11-16**.
- **Verification:** *Primary* (DORA and Google Cloud publications), *excerpt only*: seen as search-result excerpts; the documents were not opened in full. Interviews with DORA's lead researcher in secondary newsletters were consulted and not relied on.

## Planned sources (not yet opened; do not cite until verified)

The Agile Manifesto and its history · The NIST definition of cloud computing · Origin of the term "DevOps" (late 2008 to 2009; the SRE book gives late 2008) · *The DevOps Handbook* · *Accelerate* · The Google SRE book beyond Chapter 1 · The 2019 DORA report (the original source of REF-008's findings) · DORA's capability page on working in small batches · Westrum's organisational-culture typology as used in DORA research · Platform-engineering sources.
