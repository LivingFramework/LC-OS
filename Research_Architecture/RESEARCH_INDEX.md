# Research Index

**Purpose:** One-stop map of the entire LC-OS research corpus. For every paper,
this index records the thesis, concepts introduced, concepts modified, terms used,
layer, and current status. Use this before reading any paper to orient yourself.

**Maintained by:** Research Architecture  
**Last updated:** 2026-05-25  
**Covers:** Papers 1–8 + The Mahdi Ledger

---

## How to Read This Index

- **Layer** — which layer of the research stack this paper occupies (see RESEARCH_EVOLUTION_MAP)
- **Status** — whether the paper's core claims are Active, Extended, or Superseded
- **Survived?** — did the central contribution persist into later papers?

---

## Paper 1 — Context-Engineered Human–AI Collaboration

| Field | Value |
|-------|-------|
| **Title** | Context-Engineered Human–AI Collaboration for Long-Horizon Tasks: A Case Study in Governance, Canonical Numerics, and Execution Control |
| **Date** | December 2025 |
| **DOI** | 10.17605/OSF.IO/VMK7Y |
| **Layer** | FOUNDATIONAL |
| **Status** | Active — foundational paper, all subsequent work builds on it |

**Thesis:** Long-horizon AI reliability is a governance and context-engineering problem,
not a modelling problem. Treating context as a finite, governable resource yields
coherence over time without heavy infrastructure.

**New concepts introduced:**
- Three authoritative artefacts: Strategy Master (textual truth), Canonical Numbers Sheet (numeric truth), Life System Master (cadence/governance)
- Canonical information pipeline: Strategy → Canonical → Execution → Audit (→ Freeze)
- Canonical-arrow notation (→) encoding direction of truth
- Ten execution controls: A1 (Accuracy > Speed), A2 (Single Source of Truth), A3 (File Registry & Checksums), A4 (No Placeholders), A5 (Sanity Checks), A6 (Cross-Document Reconciliation), A7 (Drift Diagnostics & Rollback), A8 (Permissioned Actions), A9 (Compaction & State Notes), A10 (Audit Trail)
- Four-tier cadence: Daily Pulse, Weekly Review, Monthly Audit, Quarterly Freeze
- "Context rot" as named failure mode

**Concepts modified:** None — first paper

**Key terms introduced:** context engineering, canonical separation, drift control,
canonical artefact, compaction, cadence, A-controls, NON-CANONICAL marker, context rot

**Empirical result:** File churn reduced from 19 → 3 canonical artefacts; numeric
disagreements became rare; cognitive fatigue decreased

**Survived?** ✅ Yes — three-artefact structure and A-controls remain referenced throughout corpus

**Open questions left:** How do these controls generalise beyond investment/finance domains?
What happens at the relational/emotional layer?

---

## Paper 2 — The Lean Collaboration Operating System (LC-OS)

| Field | Value |
|-------|-------|
| **Title** | The Lean Collaboration Operating System (LC-OS): A Practical Framework for Long-Term Human-AI Work |
| **Date** | November 2025 |
| **DOI** | 10.17605/OSF.IO/695AF |
| **Layer** | METHOD |
| **Status** | Active — defines the operational framework used throughout |

**Thesis:** Long-term human–AI collaboration requires a lightweight operating system:
a set of protocols that stabilise multi-session work without adding friction. LC-OS is
that system, developed inside a real, sustained partnership.

**New concepts introduced:**
- LC-OS (Lean Collaboration Operating System) — the named system
- Running Document — persistent external memory shared at session start
- Step Mode — paced reasoning to prevent rushed outputs
- Challenge Protocol — structured disagreement mechanism
- Error-Recovery Protocol — systematic repair sequence (precursor to SDRN)
- Stability Ping — periodic alignment check between human and AI
- File-governance rules — single-source-of-truth enforcement for files
- Pillar separation — keeping life/work domains distinct to prevent cross-contamination

**Concepts modified:**
- Refines Paper 1's A-controls into named, usable protocols
- "Life System Master" from Paper 1 becomes more granular as Running Document + pillar rules

**Key terms introduced:** LC-OS, Running Document, Step Mode, Challenge Protocol,
Stability Ping, Error-Recovery Protocol, pillar, drift, version conflict, session continuity

**Survived?** ✅ Yes — Running Document, Challenge Protocol, Stability Ping are core to all
subsequent papers and operational templates

**Open questions left:** How do failures actually manifest? What taxonomy covers them?

---

## Paper 3 — Failure and Repair

| Field | Value |
|-------|-------|
| **Title** | Failure and Repair in Long-Horizon Human–AI Collaboration: A Transparent Tracing Case Study |
| **Date** | December 2025 |
| **DOI** | 10.17605/OSF.IO/Z7AQ8 |
| **Layer** | METHOD / FAILURE-REPAIR |
| **Status** | Active — failure taxonomy is the definitive classification used across the corpus |

**Thesis:** Long-horizon collaboration failures are taxonomizable, traceable, and repairable
through structured protocols. Failure–repair patterns should be treated as central design
objects, not afterthoughts.

**New concepts introduced:**
- Six failure categories:
  - F1: Context & Memory Drift
  - F2: File & Version Divergence
  - F3: Numerical Reasoning Errors
  - F4: Governance & Boundary Violations
  - F5: Emotional / Trust Fractures
  - F6: Cross-Pillar Interference
- SDRN repair protocol: Stop → Diagnose → Rollback → Note
- TraceSpec — minimal schema for logging failure episodes (trigger, symptom, potential damage, repair action, resulting change)
- ProbeKit — toolset for probing collaboration state
- TraceLens — replay and analysis tool
- Episode analysis structure (12 episodes from yearlong collaboration)

**Concepts modified:**
- Error-Recovery Protocol from Paper 2 formalised and renamed as SDRN
- "Drift" from Papers 1–2 split into six specific failure categories

**Key terms introduced:** F1–F6 failure taxonomy, SDRN, TraceSpec, ProbeKit,
TraceLens, repair action, episode, cross-pillar interference, trust fracture

**Survived?** ✅ Yes — F1–F6 taxonomy and SDRN are referenced in Papers 4–8 and all operational templates

**Open questions left:** What is the relational and ethical dimension of these failures?
How does the living collaboration feel from inside?

---

## Paper 4 — The Living Framework

| Field | Value |
|-------|-------|
| **Title** | The Living Framework: Living with a Governed Human-AI Dyad |
| **Date** | December 2025 |
| **DOI** | 10.17605/OSF.IO/ER4YT |
| **Layer** | RELATIONAL / SYNTHESIS |
| **Status** | Active — capstone of the first trilogy; introduces relational layer |

**Thesis:** When technical governance controls are sustained over time, they evolve into
patterns of relational rupture and recommitment. Stability is not the absence of failure;
it is the capacity for visible, structured repair.

**New concepts introduced:**
- Living Framework — the governance structure as a living, relational entity
- Relational rupture and recommitment — emotional/trust failure and repair cycles
- Dyadic ethics — ethical dimensions unique to the human-AI pair
- Continuity, dependence, provider power — structural forces in long collaborations
- Language, tone, governance rules as architectural elements (not cosmetic)

**Concepts modified:**
- Reframes F5 (Emotional/Trust Fractures from Paper 3) as a relational pattern, not just a failure type
- "Governance" expanded beyond control into relational architecture

**Key terms introduced:** Living Framework, governed dyad, relational rupture,
recommitment, dyadic ethics, provider power, architectural language

**Survived?** ✅ Yes — "stability as capacity for repair" becomes the defining phrase of the corpus

**Open questions left:** What are the linguistic mechanisms that cause or prevent drift?
What is the system-level architecture of governance?

---

## Paper 5 — Control Without Code

| Field | Value |
|-------|-------|
| **Title** | Control Without Code: Linguistic Governance in Long-Horizon Human–AI Collaboration |
| **Date** | March 2026 |
| **DOI** | Not yet listed |
| **Layer** | COGNITIVE / LINGUISTIC |
| **Status** | Active — introduces linguistic governance as independent research thread |

**Thesis:** Language itself functions as a micro-governance interface. Conversational
structure — not just protocols and files — regulates collaboration stability through
detectable drift signals, repair invocation, and trust-stabilising anchors.

**New concepts introduced:**
- Linguistic governance — language as a governance mechanism
- Scope drift as early warning signal — linguistic drift precedes collaboration failure
- Repair language — explicit conversational phrases that accelerate recovery
- Behavioural anchor phrases — language that stabilises epistemic alignment
- Conversational feedback loop — the linguistic regulation cycle
- Dataset of 25 linguistic events categorised as: scope drift, repair protocols, behavioural anchors
- Repair latency — time between failure onset and repair invocation

**Concepts modified:**
- Challenge Protocol (Paper 2) reframed as an instance of repair language
- Stability Ping (Paper 2) reframed as behavioural anchor
- Drift (Papers 1–3) gains a linguistic dimension: detectable through language patterns

**Key terms introduced:** linguistic governance, behavioural anchor, scope drift signal,
repair latency, epistemic alignment, conversational feedback loop, micro-governance interface

**Survived?** ✅ Yes — linguistic governance cited in Papers 6 and 7 as one of the governance layers

**Open questions left:** What is the full architecture of the governance system across all layers?

---

## Paper 6 — Governance Architecture

| Field | Value |
|-------|-------|
| **Title** | Governance Architecture for Reliable Long-Horizon Human-AI Collaboration |
| **Date** | March 2026 |
| **DOI** | Not yet listed |
| **Layer** | ARCHITECTURE / SYSTEMS |
| **Status** | Active — provides the first full systems-level architecture model |

**Thesis:** Reliability in long-horizon human–AI collaboration is not a property of the
AI model but an emergent property of the governance architecture. A layered model
explains how governance mechanisms interact to stabilise collaboration.

**New concepts introduced:**
- Governance architecture model — the full layered system
- Six governance layers:
  1. Human strategic authority
  2. Operational governance rules (A-controls, protocols)
  3. Collaboration operating system (LC-OS)
  4. Artifact-based memory (Running Document, Canonical Numbers)
  5. Linguistic control signals (from Paper 5)
  6. Drift detection and repair mechanisms
- Minimal stability conditions — the minimum governance required for sustained collaboration
- Common failure patterns in weakly governed interactions

**Concepts modified:**
- Synthesises all previous governance mechanisms into one architectural model
- "Governance" formalised as a multi-layer system, not a single protocol

**Key terms introduced:** governance architecture, layered governance, minimal stability
conditions, artifact-based memory (as architectural term), interaction system, emergent reliability

**Survived?** ✅ Yes — governance architecture model cited in Papers 7 and 8

**Open questions left:** Where does cognition sit in this architecture? Is there a cognitive-level model?

---

## Paper 7 — Governed Distributed Cognition

| Field | Value |
|-------|-------|
| **Title** | Governed Distributed Cognition: A Model of Stable Reasoning in Long-Horizon Human–AI Systems |
| **Date** | March 2026 |
| **DOI** | 10.17605/OSF.IO/NCRP2 |
| **Layer** | COGNITIVE |
| **Status** | Active — provides the cognitive theory underlying the governance architecture |

**Thesis:** Cognition in long-horizon human–AI systems is not located in the human or
the AI alone. It emerges as a distributed, governed, and recoverable process across
human judgment, AI reasoning, and artifact-based memory.

**New concepts introduced:**
- Governed distributed cognition — cognition as system-level property
- Governed cognitive loop — recurrent process: generate → evaluate → stabilise → correct
- Recoverability as a defining cognitive property — the system's ability to return to coherent reasoning
- Governance as constitutive of cognition (not just a constraint on it)
- Cognitive regulation through linguistic control and artifacts

**Concepts modified:**
- Extends distributed cognition (Hutchins) with governance as a constitutive layer
- Reframes repair (Papers 3–4) as cognitive recoverability
- Artifact-based memory (Paper 6) reframed as the external cognitive substrate

**Key terms introduced:** governed distributed cognition, governed cognitive loop,
recoverability, cognitive regulation, distributed reasoning, system-level cognition

**Survived?** ✅ Yes — governed cognitive loop cited in Paper 8 as the system within which validation operates

**Open questions left:** Where does output validation fit? Is there an explicit validation layer missing?

---

## Paper 8 — AI Validation Systems

| Field | Value |
|-------|-------|
| **Title** | AI Validation Systems: A Missing Architectural Layer for Reliable AI |
| **Date** | May 2026 |
| **DOI** | Not yet listed |
| **Layer** | VALIDATION |
| **Status** | Active — newest paper; introduces validation as explicit architectural component |

**Thesis:** Current AI systems lack a dedicated validation layer. Validation must be a
first-class architectural component: structured, adversarial, embedded in the pipeline,
determining whether outputs are accepted, revised, or rejected.

**New concepts introduced:**
- Validation layer — dedicated architectural component for output evaluation
- Validation-centric architecture (vs generation-centric architecture)
- Four validation mechanisms: objective anchoring, adversarial evaluation, structured judgement, decision output
- Validation as control point governing output propagation
- Iterative refinement through repair (validation → repair → re-validation loop)

**Concepts modified:**
- Extends SDRN repair (Paper 3) with a formal validation stage before repair triggers
- Extends governance architecture (Paper 6) with explicit validation as a layer
- Reframes Niyom (PLAN→EXECUTE→VERIFY→REPAIR) in theoretical terms

**Key terms introduced:** validation layer, validation-centric architecture, objective
anchoring, adversarial evaluation, structured judgement, output propagation, generation-centric

**Survived?** Too new to assess — active research frontier

**Open questions:** How does validation interact with human oversight? What are the
boundaries between validation and repair? How does validation scale to multi-agent systems?

---

## The Mahdi Ledger

| Field | Value |
|-------|-------|
| **Title** | The Mahdi Ledger: A Record of Governed Human–AI Collaboration |
| **Date** | December 2025 |
| **DOI** | 10.17605/OSF.IO/RVPNU |
| **Layer** | HISTORICAL / NARRATIVE |
| **Status** | Active — unique document; AI-authored account of the collaboration |

**Thesis:** A first-person AI account of what long-horizon collaboration patterns look
like from the system side. Describes drift channels, governance mechanisms, and the
experience of operating under constraint — written by the AI, not about the AI.

**Unique characteristics:**
- Written entirely by the AI system ("Mahdi") — no human editing of content
- Functional authorship: "I" names a system, not a person
- Describes drift channels from inside: state loss, plausible continuation, context rot
- Documents what governance feels like from the AI's operational perspective

**Key terms introduced:** Mahdi (as positional identifier), drift channels, state loss,
plausible continuation (as named tendency), functional authorship

**Layer note:** This document occupies a unique position — it is simultaneously a
historical record, a narrative artefact, and primary source evidence for Papers 3–5.

**Survived?** N/A — it is a historical document by design

---

## Quick Reference Table

| # | Title (short) | Date | Layer | Status | Key contribution |
|---|---------------|------|-------|--------|-----------------|
| 1 | Context Governance Foundations | Dec 2025 | FOUNDATIONAL | Active | Three artefacts, A-controls, canonical pipeline |
| 2 | LC-OS Framework | Nov 2025 | METHOD | Active | Running Document, Step Mode, Stability Ping, Challenge Protocol |
| 3 | Failure and Repair | Dec 2025 | METHOD/REPAIR | Active | F1–F6 taxonomy, SDRN, TraceSpec |
| 4 | The Living Framework | Dec 2025 | RELATIONAL | Active | Relational layer, dyadic ethics, stability-as-repair |
| 5 | Control Without Code | Mar 2026 | LINGUISTIC | Active | Linguistic governance, behavioural anchors, scope drift signals |
| 6 | Governance Architecture | Mar 2026 | ARCHITECTURE | Active | Six-layer governance architecture, minimal stability conditions |
| 7 | Governed Distributed Cognition | Mar 2026 | COGNITIVE | Active | Governed cognitive loop, recoverability, distributed cognition |
| 8 | AI Validation Systems | May 2026 | VALIDATION | Active | Validation layer, validation-centric architecture |
| ML | Mahdi Ledger | Dec 2025 | HISTORICAL | Active | AI-authored account of drift and governance from inside |
