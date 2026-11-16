# Publication

**Status:** Deferred. Nothing is exported until chapters have passed technical and editorial review.

## Principles
- Markdown is the source of truth. A PDF (or any other format) is **generated** from reviewed Markdown and is never edited by hand.
- Export preserves: heading hierarchy, code formatting, diagrams, captions, references, tables, page numbering, and the table of contents.
- Export is performed in `EXPORT` mode and only for chapters whose status is *Editorially reviewed* or *Finalised*.

## Plan
1. Freeze chapter numbering (printed numbers are derived from book order; cross-references use permanent IDs until then).
2. Resolve every `CH-nnn` cross-reference to its printed number.
3. Render Mermaid diagrams to images **for print only**; the Mermaid source remains in the repository.
4. Generate the PDF; check headings, code blocks, tables, and references against the Markdown.
5. Record the export (date, commit, tool versions) in `CHANGELOG.md`.
