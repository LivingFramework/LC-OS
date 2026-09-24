# Context Engineered Human AI Collaboration for Long Horizon Tasks

## A correction draft based on the November 2025 Paper 1

**Status:** Working correction draft - not for publication.  
**Purpose:** This draft applies the minimum corrections mapped in `PAPER1_CORRECTION_MAP.md` to the Executive Summary, Abstract, and Introduction of the published Paper 1. Unchanged portions preserve the original purpose and wording where that wording remains supportable.

**Published record:** OSF preprint, DOI https://doi.org/10.17605/OSF.IO/VMK7Y  
**Author:** Rishi Sood  
**Original publication date:** November 2025

## Executive Summary

This paper presents a practical governance blueprint for supporting long-horizon collaboration between a human strategist and an AI system through deliberate context engineering. Rather than optimizing prompts in isolation, it describes a way to structure state across sessions - files, numbers, and cadence - so reasoning can be checked and audited over time.

The approach is anchored in three authoritative artefacts that separate concerns and are intended to reduce drift: Strategy Master (textual truth), Canonical Numbers Sheet (numeric truth), and Life System Master (cadence and governance). Information flows in a documented sequence: Strategy -> Canonical Numbers -> Execution -> Audit -> Freeze.

The published paper describes ten execution controls (A1-A10):

- A1 Accuracy over Speed - prioritise verification over throughput.
- A2 Single Source of Truth - numbers come only from Canonical.
- A3 File Registry and Checksums - one live file; versions traceable.
- A4 No Placeholders in Outputs - finals should not contain speculative or incomplete content.
- A5 Sanity Checks and Unit Tests - verify before publication.
- A6 Cross Document Reconciliation - Strategy and Canonical should match.
- A7 Drift Diagnostics and Rollback - detect, revert, and note cause.
- A8 Permissioned Actions and Approvals - gated changes and explicit approval.
- A9 Compaction and State Notes - summarise long history.
- A10 Audit Trail and Release Process - freeze, log, and archive.

**Historical terminology note.** The published paper uses A1-A10 inconsistently in later sections. This correction preserves that historical inconsistency rather than silently choosing one mapping. It makes no control-specific outcome attribution.

The original paper reported reductions in file churn, numeric disagreement, recovery time, and qualitative load, as well as a gift-capture outcome. The underlying logs, denominators, definitions, and source records are not available. Accordingly, this correction does not present those reports as verified findings.

LLMs can encounter context loss, ambiguous numerics, and rushed iteration. Treating context as a finite, governed resource - with a small working set, verifiable numbers, and frozen checkpoints - is intended to support coherence in settings where correctness and provenance matter.

The original one-week adoption sequence is retained later only as an illustrative workflow. It is not presented as a validated deployment protocol.

**Bottom line.** The paper presents process design as a proposed way to support long-horizon reliability. It does not establish that the proposed controls are effective or superior to model-scale, longer-context, or alternative approaches.

## Abstract

This paper describes a structured governance framework for supporting long-horizon collaboration between humans and large language models through deliberate context engineering. It describes one human-AI collaboration focused on maintaining accuracy, auditability, and coherence across extended reasoning cycles.

At the centre of the framework are three authoritative artefacts that separate layers of truth: Strategy Master (textual truth), Canonical Numbers Sheet (numeric truth), and Life System Master (cadence and governance). These artefacts are connected through a documented information sequence - Strategy -> Canonical -> Execution -> Audit -> Freeze - intended to reduce ambiguity.

The paper describes ten execution controls that specify operational safeguards such as accuracy over speed, single sources of truth, cross-document reconciliation, drift diagnostics, and audit trail management. These safeguards are intended to support more consistent long-horizon collaboration.

The original paper reported empirical outcomes from the collaboration. Those outcome estimates cannot be verified from the available records. This single human-AI case also cannot establish whether reliability depends more on process design than on model scale, parameter count, or context-window size.

By treating context as a finite, governable resource and combining minimal tooling with disciplined cadence, the paper offers a traceability-oriented approach that may be adapted and prospectively evaluated in smaller workflows where correctness, provenance, and long-term coherence matter.

## 1 Introduction

Large language models can process long contexts, but sustaining dependable work across days or weeks remains difficult. Minor inconsistencies in sources, ambiguous numerics, and ad-hoc decisions can compound into drift. Human collaborators may accept provisional facts as permanent, then lose track of their origin. The result can be a brittle workflow that appears effective in short excerpts but does not remain dependable over time.

This paper frames long-horizon collaboration as a governance and context-engineering problem. Its central design choice is to keep working memory small, provenance explicit, and action gates simple and repeatable. Rather than assuming that longer prompts or larger context windows will prevent errors, it proposes surrounding processes intended to limit how easily mistakes propagate.

The method has three components.

### 1.1 Canonical separation of text and numerics

The paper describes a two-file separation between logic and data: the Strategy Master holds narrative reasoning, operating rules, and procedural logic; the Canonical Numbers Sheet contains numeric values treated as authoritative for the workflow. Numerical claims absent from the canonical sheet are marked NON-CANONICAL and should not drive decisions.

This two-file separation is one layer within the three-artefact arrangement described above; the Life System Master holds cadence and audit procedures.

### 1.2 Control stack

The published paper describes ten execution controls (A1-A10) intended to govern behaviour at critical points:

| ID | Control | Core function |
|---|---|---|
| A1 | Accuracy over Speed | Prioritise verification over throughput. |
| A2 | Single Source of Truth | Use canonical lookup for numeric values. |
| A3 | File Registry and Checksums | Record version traceability. |
| A4 | No Placeholders in Outputs | Avoid speculative or incomplete final content. |
| A5 | Sanity Checks and Unit Tests | Check numerics and logic before publication. |
| A6 | Cross Document Reconciliation | Check Strategy and Canonical for consistency. |
| A7 | Drift Diagnostics and Rollback | Detect anomalies and record their cause. |
| A8 | Permissioned Actions and Approvals | Gate material changes through explicit consent. |
| A9 | Compaction and State Notes | Summarise long histories into concise digests. |
| A10 | Audit Trail and Release Process | Freeze, log, and archive artefacts. |

Together, these controls specify documented checkpoints within a human-AI workflow. They do not make model reasoning deterministic.

### 1.3 Cadence and audit rhythm

The paper describes a temporal cycle of daily pulse, weekly review, monthly audit, and quarterly freeze. This cycle is intended to support review and reduce over-iteration without requiring extensive infrastructure.

This paper presents an applied design description rather than a controlled experiment or benchmark. Its primary case concerns an investment-strategy environment, while similar workflow risks may arise in research programmes, legal case management, product-incident response, and knowledge operations. The proposed structure may support reliability, but that proposition requires prospective evaluation.

**Purpose and contribution.** The contribution of this work is to describe long-horizon human-AI collaboration as a governance and context-engineering problem, and to document the file architecture and lightweight control stack developed in one active collaboration. The paper does not claim to validate effectiveness, reproducibility, or comparative performance.

The remainder of the corrected paper retains the original subject areas while distinguishing historical descriptions from claims requiring prospective evaluation. It reviews relevant context-engineering and agentic-systems literature; describes the architecture and its limits; records the evidentiary limitations of the original outcome claims; and outlines ethical and practical considerations without claiming certification or demonstrated effectiveness.
