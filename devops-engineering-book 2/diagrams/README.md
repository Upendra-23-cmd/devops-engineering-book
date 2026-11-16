# Diagrams

Diagrams are written as **Mermaid** text so that they are version-controlled and reviewable in pull requests. GitHub renders `mermaid` fenced blocks in Markdown.

## Conventions

- Chapter-specific diagrams are written **inline** in the chapter. Diagrams shared by several documents live here as `FIG-<nnn>-<slug>.md`.
- Every diagram has an ID, a caption, and a *last reviewed* date.
- Quote node labels (`A["Label"]`) to avoid parser problems with punctuation.
- No secrets, real hostnames, real IP addresses, or customer data in any diagram.
- A diagram that cannot be rendered by GitHub's Mermaid support is simplified rather than replaced by an image, unless an editable visual canvas materially improves it. In that case the Mermaid or text source is still kept here.

## Registry

| ID | Title | File | Last reviewed |
|---|---|---|---|
| FIG-001 | Programme phases and project gates | [`FIG-001-programme-phases.md`](FIG-001-programme-phases.md) | 2026-11-14 |
| FIG-002 | Plan-driven delivery pipeline with queues (Chapter 1) | Inline in [`CH-001`](../chapters/part-01-devops-foundations/ch-001-from-silos-to-devops.md) | 2026-11-14 |
| FIG-003 | A generic delivery system with feedback loops (Chapter 1) | Inline in [`CH-001`](../chapters/part-01-devops-foundations/ch-001-from-silos-to-devops.md) | 2026-11-14 |
| FIG-004 | The control spiral: gates, batch size, and adaptation (Chapter 1, §1.1.2) | Inline in [`CH-001`](../chapters/part-01-devops-foundations/ch-001-from-silos-to-devops.md) | 2026-11-16 |

> **Note.** Rendering has not been checked in a Mermaid renderer in the environment where this scaffold was produced. Open each diagram on GitHub (or in a Mermaid-aware viewer) and report any that fail to render.
