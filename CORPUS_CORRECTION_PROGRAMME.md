# LC-OS Corpus Correction Programme

Status: active audit; no published PDF has been altered  
Established: 11 August 2026

## Purpose

This file records the existence and governing rules of the LC-OS corpus correction programme. The programme replaces the proposed Convergence Companion as the priority workstream.

The immediate objective is to audit all eight LC-OS papers and then publish corrected, clearly versioned manuscripts where the evidence requires revision. Paper 1 will be rebuilt first after the complete corpus audit because it is the foundation for the later series.

## Authoritative detailed records

The detailed, row-level audit is maintained in the Awen repository on branch `lc-os-convergence-evidence-audit`, under:

`projects/lc-os-convergence-companion/`

The controlling files are:

- `CORPUS-CORRECTION-REGISTER.csv` — every material correction, its severity, evidence, impact, and required remediation.
- `LCOS-CLAIM-REGISTER.csv` — exact claims, source locations, permitted paraphrases, prohibited strengthening, and verification status.
- `CONTRADICTION-REGISTER.csv` — conflicts within papers and between frozen papers, repository summaries, and later drafts.
- `SOURCE-MANIFEST.csv` — canonical URLs, versions, dates, and file hashes.
- `SOURCE-QUALITY-ASSESSMENT.md` — paper-level methodological and evidential assessment.
- `LIMITATIONS-AND-EXCLUSIONS.md` — claims that must not be made.
- `DECISION-LOG.md` and `session-logs/` — audit decisions and session handoffs.

The Awen register is the single source of truth. This LC-OS file is an index and policy notice, not a duplicate correction ledger.

## Current audit position

Completed full-paper audits:

- Paper 1 — 5 correction entries.
- Paper 2 — 8 correction entries.
- Paper 3 — 14 correction entries.
- Paper 4 — 13 correction entries.

Current total: 40 material correction entries.

Next work, after owner authorization:

1. Audit Papers 5–8.
2. Reconcile cross-paper terminology, evidence, chronology, and dependencies.
3. Rebuild Paper 1 accurately as the corrected foundation.
4. Subject the revised Paper 1 to source verification, calculation checks, adversarial review, reference validation, and full rendered-document inspection.
5. Publish a transparent new version and change log without erasing the historical record.
6. Revise later papers in dependency order.

## Non-negotiable correction rules

- Preserve every original DOI-linked or frozen publication.
- Never silently overwrite historical evidence or terminology.
- Distinguish factual correction, clarification, reanalysis, and genuinely new evidence.
- Do not reconstruct missing data from memory.
- Narrow or remove any claim whose evidence cannot be verified.
- Match claim strength exactly to the available evidence.
- Verify quotations, citations, DOI metadata, dates, protocol sequences, tables, figures, calculations, and availability statements.
- Record every material change in a version-specific change log.
- Do not use a later correction to backdate priority or strengthen the historical record.
- Do not release a revised paper until it passes an adversarial final review and complete render inspection.

## Present boundary

The Convergence Companion is paused indefinitely. No external convergence, novelty, independence, priority, lead-time, or comparative-timeline claim should be published until the corpus correction programme is complete and separately reviewed.
