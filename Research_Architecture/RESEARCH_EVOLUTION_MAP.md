# Research Evolution Map

**Purpose:** The history of thought across the LC-OS research corpus. Tracks how
concepts were born, merged, renamed, deprecated, and evolved from Paper 1 through Paper 8.

**Read this when:** You want to understand *why* the corpus is structured as it is,
or need to trace where a concept came from and how it changed.

**Last updated:** 2026-05-25

---

## The Research Arc (One Paragraph)

The corpus began as a governance blueprint for a specific problem: how to keep
AI collaboration reliable across many sessions (Paper 1). It quickly became clear
that reliability required a named operating system (Paper 2), and that operating
systems fail in predictable ways (Paper 3). The relational and human dimensions of
those failures demanded their own treatment (Paper 4). With the practical system
established, the research turned inward: how does *language itself* govern the
collaboration (Paper 5)? What is the *architecture* of the full governance system
(Paper 6)? What does *cognition* look like in such a system (Paper 7)? And finally:
is there a validation layer missing from all of this (Paper 8)?

The arc moves from **practice → system → failure → relationship → language →
architecture → cognition → validation**. Each paper adds a layer. Nothing is discarded.

---

## Concept Lineage

### Concept: Canonical Artefacts / Authoritative Files

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Born | Paper 1 | Three artefacts: Strategy Master, Canonical Numbers Sheet, Life System Master | Active |
| Refined | Paper 2 | Life System Master split into Running Document + pillar governance rules | Active |
| Extended | Paper 6 | Renamed "artifact-based memory" in architectural model | Active |
| Extended | Paper 7 | Reframed as "external cognitive substrate" in distributed cognition model | Active |

**Current status:** Active. The three-artefact structure (Strategy Master, Canonical Numbers, Running Document) is the operational core of LC-OS-Project.

---

### Concept: Drift

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Born | Paper 1 | "Context rot" — unnamed drift in long contexts | Active |
| Named | Paper 2 | "Drift" as explicit concept; Stability Ping as detection mechanism | Active |
| Taxonomised | Paper 3 | Drift split into six failure categories (F1–F6) | Active |
| Linguistic dimension | Paper 5 | "Scope drift" detectable through language patterns | Active |
| Architectural dimension | Paper 6 | Drift as system-level failure; "drift detection" as governance layer | Active |
| Cognitive dimension | Paper 7 | Drift as loss of cognitive recoverability | Active |

**Current status:** Active. "Drift" is the unifying failure concept across the corpus.
Most concrete as F1 (Context & Memory Drift) in operational use.

---

### Concept: Repair

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Born | Paper 2 | "Error-Recovery Protocol" — informal repair sequence | Active |
| Formalised | Paper 3 | SDRN: Stop → Diagnose → Rollback → Note; TraceSpec schema | Active |
| Relational dimension | Paper 4 | Repair as "recommitment" — emotional/relational layer | Active |
| Linguistic dimension | Paper 5 | "Repair language" as explicit governance mechanism | Active |
| Cognitive dimension | Paper 7 | Repair as restoring cognitive recoverability | Active |
| Validation integration | Paper 8 | Repair triggered by validation failure; repair → re-validation loop | Active |

**Current status:** Active. SDRN is the operational repair protocol. Repair is now
understood as: technical (SDRN) + relational (recommitment) + linguistic (repair language)
+ cognitive (recoverability restoration) + validation-triggered.

---

### Concept: Governance

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Born | Paper 1 | A-controls (A1–A10) as governance mechanisms | Active |
| Extended | Paper 2 | LC-OS protocols as lightweight governance layer | Active |
| Relational | Paper 4 | Governance as architectural, not just procedural | Active |
| Linguistic | Paper 5 | Language as micro-governance interface | Active |
| Architecturalised | Paper 6 | Full six-layer governance architecture model | Active |
| Constitutive | Paper 7 | Governance as constitutive of cognition, not just constraint on it | Active |

**Current status:** Active — but under terminology review. See TERM_REGISTRY for
the "governance" special review section.

---

### Concept: Running Document

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Implicit | Paper 1 | Life System Master contains session cadence; no explicit "running document" | — |
| Born | Paper 2 | Running Document as named persistent memory mechanism | Active |
| Evidence | Paper 3 | Running Document cited as one of the controls that contained failure damage | Active |
| Architectural | Paper 6 | Running Document classified as artifact-based memory layer | Active |
| Cognitive | Paper 7 | Running Document as external cognitive substrate | Active |

**Current status:** Active. The Running Document is the single most referenced operational
artefact across the corpus. It appears in every paper from 2 onward.

---

### Concept: Stability / Stability Ping

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Born | Paper 2 | Stability Ping as periodic alignment check | Active |
| Defined relationally | Paper 4 | "Stability is not the absence of failure; it is the capacity for visible, structured repair" — corpus-defining phrase | Active |
| Linguistic | Paper 5 | Behavioural anchor phrases as stability mechanisms | Active |
| Architectural | Paper 6 | Minimal stability conditions defined | Active |

**Current status:** Active. Stability Ping remains an operational tool. The relational
definition of stability (Paper 4) became the corpus's philosophical anchor.

---

### Concept: Failure Taxonomy (F1–F6)

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Born | Paper 3 | Six categories: F1 Context Drift, F2 File Divergence, F3 Numerical Errors, F4 Boundary Violations, F5 Trust Fractures, F6 Cross-Pillar | Active |
| Extended | Paper 4 | F5 (Trust Fractures) expanded into relational theory | Active |
| Referenced | Papers 5–8 | F1, F4, F5 referenced as the failure types linguistic governance and architecture address | Active |

**Current status:** Active. F1–F6 is the stable failure classification system used in
all operational templates, examples, and failure logs across LC-OS-Project.

---

### Concept: Linguistic Governance

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Born | Paper 5 | Language as micro-governance mechanism; scope drift signals, repair language, behavioural anchors | Active |
| Integrated | Paper 6 | Linguistic control signals as one of six governance layers | Active |
| Integrated | Paper 7 | Linguistic controls as part of cognitive regulation | Active |

**Current status:** Active. Explains *why* certain phrases in the operational templates
(Challenge Protocol, Stability Ping trigger phrases) work at a governance level.

---

### Concept: Validation

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Implicit | Papers 1–3 | Audit, sanity checks, cross-document reconciliation — validation present but unnamed as layer | — |
| Implicit | Papers 6–7 | Governance and cognitive loop include evaluation steps | — |
| Named as missing layer | Paper 8 | Validation formalised as explicit architectural component; validation-centric architecture introduced | Active |

**Current status:** Active frontier. Paper 8 is the newest contribution. Validation is
the current research edge — the layer that was always implicit but never formalised
until Paper 8.

---

### Concept: Distributed Cognition / Governed Cognitive Loop

| Stage | Paper | Form | Status |
|-------|-------|------|--------|
| Born | Paper 7 | Governed distributed cognition; governed cognitive loop; recoverability | Active |

**Current status:** Active. Provides the cognitive theory underlying the governance
architecture. Bridges computer science governance (Papers 1–6) with cognitive science.

---

## Chronological View: When Ideas Arrived

```
Nov 2025  ──────── Paper 2: LC-OS, Running Document, Step Mode, Stability Ping
Dec 2025  ──────── Paper 1: Context engineering, A-controls, Canonical artefacts
          ──────── Paper 3: F1–F6 taxonomy, SDRN, TraceSpec
          ──────── Paper 4: Living Framework, relational layer, stability-as-repair
          ──────── Mahdi Ledger: AI-authored account of collaboration from inside
Mar 2026  ──────── Paper 5: Linguistic governance, behavioural anchors
          ──────── Paper 6: Governance architecture, six layers, minimal stability conditions
          ──────── Paper 7: Governed distributed cognition, cognitive loop, recoverability
May 2026  ──────── Paper 8: Validation layer, validation-centric architecture
```

Note: Paper 2 was published before Paper 1 despite Paper 1 covering earlier work.
The publication sequence does not reflect the conceptual sequence.

---

## Conceptual Dependency Map

```
Paper 1 (Foundations)
    └──► Paper 2 (LC-OS Operating System)
              └──► Paper 3 (Failure & Repair Taxonomy)
                        └──► Paper 4 (Living Framework / Relational Layer)
                                  └──► Paper 5 (Linguistic Governance)
                                             └──► Paper 6 (Governance Architecture)
                                                       └──► Paper 7 (Governed Cognition)
                                                                 └──► Paper 8 (Validation Layer)
Mahdi Ledger ──► (Primary evidence for Papers 3, 4, 5)
```

Each paper extends the one before it. No paper invalidates a prior paper.
The corpus is cumulative, not revisionary.

---

## What Has Not Changed

These concepts have remained stable from introduction to present:

- The three-artefact structure (Strategy Master, Canonical Numbers, Running Document)
- The F1–F6 failure taxonomy
- The SDRN repair protocol
- The definition of stability: "not the absence of failure but the capacity for visible, structured repair"
- The core claim: reliability is a governance property, not a model property

---

## What Has Evolved

- "Governance" — grew from A-controls (Paper 1) → protocols (Paper 2) → relational architecture (Paper 4) → linguistic mechanism (Paper 5) → six-layer system (Paper 6) → constitutive of cognition (Paper 7)
- "Repair" — grew from Error-Recovery (Paper 2) → SDRN (Paper 3) → recommitment (Paper 4) → linguistic repair (Paper 5) → validation-triggered repair (Paper 8)
- "Drift" — grew from context rot (Paper 1) → named failure (Paper 2) → six categories (Paper 3) → linguistic detection (Paper 5) → cognitive recoverability loss (Paper 7)

---

## What Ended / Was Deprecated

No concepts have been deprecated. The corpus is additive. Older formulations were
refined and extended, not replaced. The A-controls from Paper 1, for example, are
now understood as instances of the governance architecture from Paper 6 — they were
not wrong, just more specific than the later model.
