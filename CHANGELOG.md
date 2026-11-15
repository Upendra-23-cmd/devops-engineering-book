# Changelog

Format: newest first. Dates are ISO 8601 (UTC).

## 0.1.0 — 2026-11-14

### Added
- Repository scaffold following the file organisation in Part 12 of the master prompt.
- `TABLE_OF_CONTENTS.md`: 17 parts, 118 chapters, 291 sections. Generated from a single data structure; the generator asserted that every curriculum topic maps to exactly one section and that curriculum order is preserved within each part (Part XVII, whose subjects the master prompt calls "potential", is grouped by failure theme).
- `BOOK_PLAN.md`: starting position, programme architecture, eight-phase roadmap with gates, learning loop, laboratory and cost policy, assessment policy, tooling status, decision log (D-001 to D-011), risks.
- `EDITORIAL_GUIDELINES.md`: identifiers, the 24-component chapter template, the six-part concept template, laboratory rules and hint ladder, failure-injection safety rules, evidence and verification rules, review workflow.
- `PROGRESS.md`: six separate trackers, claimed-versus-verified register, five-dimension matrix, 118-row chapter register.
- `projects/PORTFOLIO.md`: eight projects delivered as twelve increments, the 20-point quality standard, evidence rules, lifecycle gates, defence checklist.
- Templates: chapter, lab (21 fields), project specification, AirDive incident intake.
- `chapters/part-01-devops-foundations/ch-001-…`: front matter, chapter foundations, and concept 1.1.1. Status **Planned** (drafting in progress).
- `labs/ch-001/LAB-001-01-…`: value stream map lab (assessment mode). Status **Drafted, not yet run**.
- `labs/diagnostic/BASE-01-…`: baseline assessment (16 scenario questions plus architecture recall). Answer key not stored.
- `diagrams/FIG-001`; inline `FIG-002` and `FIG-003` in Chapter 1.

### Verified
- The five-metric DORA model and its 2024 update, against DORA's own history page.
- Little's Law (1961 paper's bibliographic record and abstract).
- The M/M/1 time-in-system relationship (university lecture notes, plus the author's simulation: 1.99, 5.10, and 10.03 times service time at utilisation 0.5, 0.8, and 0.9, against theoretical 2, 5, and 10).
- Arithmetic in every worked example in Chapter 1 and in the BASE-01 subnet question (computed, not estimated).

### Not verified (see `REFERENCES.md` for each source's level)
- Royce (1970): the full paper was not opened; statements rest on a reprint excerpt and secondary accounts. The "waterfall" 1976 attribution is hedged in the text.
- The 1968 NATO conference: a participant's retrospective was seen as an excerpt only.
- Value stream mapping terms: secondary sources only.
- Mermaid diagrams were not rendered in a Mermaid renderer.
- No lab has been executed.

### Known limitations
- No GitHub repository exists; the GitHub integration was not connected when this scaffold was produced.
- No AirDive evidence has been supplied, so no case study exists.
- Planning effort figures in `BOOK_PLAN.md` §5 are assumptions.
