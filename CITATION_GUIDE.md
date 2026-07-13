# Citation and Archival Guide

**Purpose:** Explain how to cite LC-OS materials and how OSF, Zenodo, GitHub, and repository metadata relate to each other.

This guide is for readers, reviewers, and researchers who want to cite the LC-OS corpus correctly.

---

## Citation Principle

Cite the most specific object you used.

| If you used... | Cite... |
|---|---|
| A specific paper | That paper's DOI and citation |
| The Mahdi Ledger | The Mahdi Ledger citation |
| The whole research corpus | The repository-level citation |
| Templates or practical tools | The LC-OS Project repository, not this research archive |

---

## OSF and Zenodo Relationship

The papers were first registered through OSF and later also made available through Zenodo for archival and discovery purposes.

Where a paper appears on both OSF and Zenodo with the same DOI, cite the DOI shown in the paper metadata. OSF should be understood as the original registration surface; Zenodo should be understood as an additional archival/discovery surface.

Where a Zenodo record has a distinct Zenodo DOI, that DOI is listed as the Zenodo archive DOI.

The practical rule is simple:

> Use the DOI listed for the paper in `Papers/README.md` or `CITATION.cff`.

---

## Repository-Level Citation

Use the repository-level citation when referencing LC-OS as a complete research corpus rather than one specific paper.

```text
Sood, R. (2025). Lean Collaboration Operating System (LC-OS): A Governance Framework for Long-Horizon Human–AI Collaboration. GitHub. https://github.com/LivingFramework/LC-OS
```

This citation points to the organised archive as a whole: papers, ledger, research architecture, term registry, and corpus maintenance documents.

---

## Paper-Level Citations

For individual papers, prefer the citation listed in:

- [Papers/README.md](Papers/README.md)
- [CITATION.cff](CITATION.cff)

These are the authoritative citation surfaces inside the repository.

---

## GitHub vs DOI Records

GitHub is the navigable research archive.

OSF and Zenodo are archival/citation surfaces.

The recommended use is:

- Use GitHub to navigate the corpus.
- Use DOI records to cite specific papers.
- Use the repository citation only when citing the corpus as a corpus.

---

## `CITATION.cff` Note

`CITATION.cff` exists so GitHub and citation managers can expose citation metadata automatically.

The repository-level citation describes the archive as a whole. Individual paper entries inside `CITATION.cff` describe the scholarly works within the archive.

Because LC-OS is primarily a research corpus rather than executable software, the repository-level citation should be interpreted as a corpus/archive citation, not as a claim that the repository is a software package.

---

## Maintenance Rules

When adding or updating a paper:

1. Add the paper citation to `Papers/README.md`.
2. Add or update the reference in `CITATION.cff`.
3. Update `Research_Architecture/RESEARCH_INDEX.md`.
4. Update any relevant term entries in `Research_Architecture/TERM_REGISTRY.md`.
5. Update synthesis or evolution documents only if the paper changes the corpus-level argument.

Do not create conflicting citation surfaces. If two files disagree, `Papers/README.md` and `CITATION.cff` should be reconciled first.
