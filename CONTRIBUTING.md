# Contributing to LC-OS

**Purpose:** Define how this repository should be maintained so the LC-OS research archive remains clear, stable, and trustworthy.

LC-OS is a research corpus. It contains published papers, an AI-authored ledger, citation metadata, and research architecture. It is not the place for operational templates, implementation scripts, or practitioner quick-start tooling; those belong in the companion LC-OS Project repository.

---

## Repository Boundary

| Belongs here | Belongs elsewhere |
|-------------|------------------|
| Published papers | Operational templates |
| Research architecture | Implementation scripts |
| Citation metadata | Daily-use checklists |
| Research index and term registry | Practitioner examples |
| Archive and reader guidance | Tooling prototypes |

Operational material should go to `LC-OS-Project` unless it is included only as evidence or citation context for the research corpus.

---

## Contribution Rules

1. **Do not silently rewrite published research.**
   Published PDFs and archival records should be treated as fixed scholarly artefacts.

2. **Use navigation documents for clarification.**
   If a reader-facing explanation needs improvement, update the README, Reader Guide, Citation Guide, Research Architecture files, or Archive Policy rather than altering published papers.

3. **Keep metadata aligned.**
   When paper metadata changes, check all relevant surfaces:
   - `README.md`
   - `Papers/README.md`
   - `Research_Architecture/RESEARCH_INDEX.md`
   - `CITATION_GUIDE.md`
   - `CITATION.cff`

4. **Follow the Future Research Protocol for new research.**
   New papers or substantial theoretical additions should follow `Research_Architecture/FUTURE_RESEARCH_PROTOCOL.md`.

5. **Preserve the research/project boundary.**
   New tools, templates, automation, or practitioner material should normally be added to the companion project repository, not this archive.

6. **Prefer small, auditable changes.**
   Make focused changes with clear commit messages. Avoid large mixed edits that combine theory, metadata, navigation, and formatting in one change.

---

## Maintenance Checklist

Before merging a documentation or metadata update, verify:

- Links resolve internally.
- DOI fields match the current citation guide and paper metadata.
- Reader-facing claims do not overstate what the papers establish.
- The research archive remains distinct from the operational toolkit.
- The change is documented in `CHANGELOG.md` if it materially changes repo navigation, citation metadata, or archive structure.

---

## Publication Integrity

Corrections to published work should be handled through errata, notes, future papers, or metadata updates. Published PDFs should not be replaced simply to smooth wording after release.

The archive should make the research easier to understand without blurring the historical record of how the corpus developed.
