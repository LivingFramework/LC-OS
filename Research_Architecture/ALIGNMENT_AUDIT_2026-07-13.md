# LC-OS Research Corpus Alignment Audit

**Date:** 2026-07-13  
**Scope:** LC-OS repository research archive, paper metadata, Zenodo/OSF references, and Research Architecture navigation layer  
**Status:** Maintenance audit — does not introduce new theoretical claims

---

## Purpose

This audit checks whether the public repository presents the LC-OS research corpus coherently across:

- Root `README.md`
- `Papers/README.md`
- `CITATION.cff`
- `LICENSE.md`
- `Research_Architecture/` navigation files

The goal is not to rewrite the research. The goal is to align repository metadata, citation surfaces, and navigation infrastructure so the corpus remains internally consistent and externally citable.

---

## Current Corpus Shape

The repository already has a strong research-archive structure:

1. Root README explains the core LC-OS thesis and positions the repository as a research archive.
2. `Papers/README.md` gives paper-level abstracts, files, DOI/citation information, and reading order.
3. `CITATION.cff` gives repository-level citation metadata and paper-level references.
4. `Research_Architecture/` provides corpus navigation infrastructure:
   - `RESEARCH_INDEX.md`
   - `RESEARCH_EVOLUTION_MAP.md`
   - `TERM_REGISTRY.md`
   - `UNIFIED_SYNTHESIS.md`
   - `RESEARCH_LAYER_SEPARATION.md`
   - `OPERATIONALIZATION_AUDIT.md`
   - `FUTURE_RESEARCH_PROTOCOL.md`
5. `Mahdi_Ledger/` is positioned as a primary transparency artefact and companion record.

This is the right architecture for a research corpus. The main risks are now metadata drift and citation drift, not conceptual incoherence.

---

## Alignment Findings

### 1. DOI drift in `RESEARCH_INDEX.md`

`Papers/README.md` and `CITATION.cff` contain DOI information for Papers 5, 6, and 8, but `Research_Architecture/RESEARCH_INDEX.md` still marks some of them as missing.

#### Required corrections

| Paper | Current issue | Correct DOI |
|------|---------------|-------------|
| Paper 5 — Control Without Code | `RESEARCH_INDEX.md` says `DOI: Not yet listed` | `10.5281/zenodo.18900058` |
| Paper 6 — Governance Architecture | `RESEARCH_INDEX.md` says `DOI: Not yet listed` | `10.5281/zenodo.19038340` |
| Paper 8 — AI Validation Systems | `RESEARCH_INDEX.md` says `DOI: Not yet listed` | `10.5281/zenodo.19983551` |

#### Recommended action

Update `Research_Architecture/RESEARCH_INDEX.md` so DOI fields match the paper README and citation file.

---

### 2. Last-updated drift in Research Architecture

`RESEARCH_INDEX.md` is marked as last updated `2026-05-25`, but the repository now includes later publication metadata for Paper 8 and Zenodo-linked entries.

#### Recommended action

After DOI corrections, update the `Last updated` field to the maintenance date of the correction.

Suggested value:

```md
**Last updated:** 2026-07-13
```

---

### 3. Repository-level citation type may understate the corpus

`CITATION.cff` currently uses:

```yaml
type: software
```

LC-OS is partly a framework and partly a research archive. Since this repository is explicitly described as the research archive for papers, ledger, and architecture documents, `software` may not be the best fit.

#### Options

| Option | Meaning | Recommendation |
|-------|---------|----------------|
| Keep `type: software` | Treat LC-OS as a software/framework artefact | Acceptable if GitHub citation should identify the operational framework |
| Change to `type: dataset` | Treat repo as corpus/archive | Possible, but may be misleading because papers are the primary artefacts |
| Change to `type: collection` | Treat repo as curated scholarly collection | Best conceptual fit if accepted by CFF tooling |

#### Recommended action

Check CFF schema compatibility before changing. If `collection` is valid for your target citation tooling, use it. Otherwise keep `software` and add a clarifying `abstract` sentence: this repository is the research archive and citation gateway for the LC-OS corpus.

---

### 4. OSF vs Zenodo canonicality needs one explicit rule

The corpus currently uses both OSF and Zenodo:

- Papers 1–4 and 7 list OSF DOIs as canonical and Zenodo as mirrors.
- Papers 5, 6, and 8 list Zenodo as the main DOI source.
- The root README points directly to Zenodo record URLs for all papers.

This is understandable, but a new reader may not know whether to cite OSF or Zenodo when both exist.

#### Recommended action

Add a short canonicality rule to `Papers/README.md`, for example:

```md
## DOI Canonicality Rule

Where both OSF and Zenodo records exist, cite the DOI marked "Canonical" in the paper entry. Zenodo links are included as archival mirrors unless no OSF DOI is listed.
```

This prevents citation ambiguity without changing any underlying publication record.

---

### 5. Research/operational boundary is clear, but root README could surface it earlier

`FUTURE_RESEARCH_PROTOCOL.md` makes a clean distinction:

- Research corpus → ideas, models, frameworks, empirical findings
- LC-OS-Project → tools, templates, examples, automation

The root README mentions the companion LC-OS Project repository, but the boundary could be made slightly more explicit near the top.

#### Recommended action

In the root README, under “What This Repository Contains,” add one sentence:

```md
This repository preserves the scholarly corpus; implementation templates and operational tooling live in LC-OS-Project.
```

This will reduce confusion for practitioners landing on the repo looking for templates.

---

### 6. Good existing alignment to preserve

The following areas are already strong and should not be over-edited:

- The root README clearly states the core thesis: long-horizon reliability is a governance problem, not a model-capability problem.
- The eight-paper synthesis is coherent and readable.
- The `Research_Architecture/README.md` correctly states that the folder is navigation infrastructure, not new research.
- The `FUTURE_RESEARCH_PROTOCOL.md` is well aligned with the corpus-governance logic of LC-OS itself.
- The license is clear: CC BY 4.0.

---

## Minimal Patch Set

For immediate alignment, make only these changes:

1. Update Paper 5 DOI in `Research_Architecture/RESEARCH_INDEX.md`.
2. Update Paper 6 DOI in `Research_Architecture/RESEARCH_INDEX.md`.
3. Update Paper 8 DOI in `Research_Architecture/RESEARCH_INDEX.md`.
4. Update `RESEARCH_INDEX.md` last-updated date.
5. Add a DOI canonicality rule to `Papers/README.md`.
6. Add one research-vs-project boundary sentence to the root README.

Do **not** change theoretical wording, concepts, layer assignments, or paper summaries in this pass.

---

## Suggested Follow-Up Patch

After the minimal patch set, consider a second maintenance PR for citation polish:

1. Review whether `CITATION.cff` should remain `type: software` or become a corpus/collection-style type supported by CFF tooling.
2. Add repository-level `doi` only if there is a single canonical DOI for the repository as a whole.
3. Keep individual paper DOIs in `references`.
4. Add `preferred-citation` if you want GitHub’s citation widget to point users to a specific paper or corpus-level citation.

---

## Governance Note

This audit should be treated as maintenance under LC-OS governance:

- It does not add new claims.
- It corrects metadata drift.
- It preserves the research/operations boundary.
- It strengthens citation reliability.
- It keeps the corpus externally legible without altering the research substance.

In LC-OS terms: this is a file-governance and citation-governance repair, not a research contribution.
