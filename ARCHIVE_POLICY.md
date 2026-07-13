# Archive Policy

**Purpose:** Define how the LC-OS research archive preserves scholarly integrity while allowing reader-facing documentation and metadata to improve over time.

LC-OS is a living research corpus, but not every part of the corpus should change in the same way. Published papers, archival records, navigation documents, and operational outputs have different stability rules.

---

## Stability Classes

| Class | Examples | Update rule |
|------|----------|-------------|
| Published research records | Paper PDFs, Mahdi Ledger publication files | Treat as fixed records after publication |
| Metadata | DOI fields, citation tables, release dates, links | Correct when inaccurate or incomplete |
| Navigation documents | README, Reader Guide, Citation Guide, Research Architecture guides | Improve as the corpus becomes easier to explain |
| Operational outputs | Templates, scripts, field tools | Maintain in `LC-OS-Project`, not this repository |

---

## Published Papers

Published papers should not be silently rewritten after release.

If a paper needs correction after publication, use one of these mechanisms:

1. Add an erratum or correction note.
2. Clarify the point in a navigation or synthesis document.
3. Address the issue in a future paper.
4. Correct citation or metadata fields where the research record itself is not being changed.

This protects the historical integrity of the corpus.

---

## Metadata Corrections

Metadata can and should be corrected when inaccurate.

Examples:

- DOI fields marked as missing when a DOI now exists.
- Broken or outdated links.
- Mismatched paper titles.
- Confusing OSF/Zenodo positioning.
- Inconsistent citation guidance across files.

Metadata corrections should be made consistently across all affected files.

---

## Navigation and Explanation

Reader-facing documents may evolve.

These include:

- `README.md`
- `READER_GUIDE.md`
- `CITATION_GUIDE.md`
- `Research_Architecture/README.md`
- `Research_Architecture/RESEARCH_INDEX.md`
- `Research_Architecture/UNIFIED_SYNTHESIS.md`
- `Research_Architecture/TERM_REGISTRY.md`

The purpose of these files is to help readers understand the corpus without altering the published research record.

---

## Research / Project Boundary

This repository holds the research archive. Operational templates, examples, scripts, and implementation tooling belong in `LC-OS-Project` unless they are included as cited evidence or research context.

Changes in the operational project may be informed by this research archive. They do not automatically require changes to the published research papers.

---

## Archive Principle

The archive should become clearer over time without pretending the research history was cleaner than it was.

Good maintenance preserves both:

- reader clarity, and
- historical traceability.
