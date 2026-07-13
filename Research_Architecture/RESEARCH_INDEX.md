# Research Index

**Purpose:** One-stop map of the LC-OS research corpus. For every paper, this index records the thesis, concepts introduced, concepts modified, key terms, layer, and current status.

**Maintained by:** Research Architecture  
**Last updated:** 2026-07-13  
**Covers:** Papers 1–8 + The Mahdi Ledger

---

## How to Read This Index

- **Layer** — where the work sits in the research stack. See [RESEARCH_LAYER_SEPARATION.md](RESEARCH_LAYER_SEPARATION.md).
- **Status** — whether the paper's core claims are Active, Extended, Superseded, Experimental, or Under Review.
- **Survived?** — whether the central contribution persisted into later work.
- **DOI** — the DOI associated with the paper metadata. Some papers were first registered through OSF and also archived or discoverable through Zenodo. See [../CITATION_GUIDE.md](../CITATION_GUIDE.md).

---

## Corpus at a Glance

| # | Title (short) | Date | DOI | Layer | Status | Key contribution |
|---|---------------|------|-----|-------|--------|------------------|
| 1 | Context Governance Foundations | Dec 2025 | 10.17605/OSF.IO/VMK7Y | FOUNDATIONAL | Active | Three artefacts, A-controls, canonical pipeline |
| 2 | LC-OS Framework | Nov 2025 | 10.17605/OSF.IO/695AF | METHOD | Active | Running Document, Step Mode, Stability Ping, Challenge Protocol |
| 3 | Failure and Repair | Dec 2025 | 10.17605/OSF.IO/Z7AQ8 | METHOD / REPAIR | Active | F1–F6 taxonomy, SDRN, TraceSpec |
| 4 | The Living Framework | Dec 2025 | 10.17605/OSF.IO/ER4YT | RELATIONAL / SYNTHESIS | Active | Relational layer, dyadic ethics, stability-as-repair |
| 5 | Control Without Code | Mar 2026 | 10.5281/zenodo.18900058 | LINGUISTIC | Active | Linguistic governance, behavioural anchors, scope drift signals |
| 6 | Governance Architecture | Mar 2026 | 10.5281/zenodo.19038340 | ARCHITECTURE | Active | Six-layer governance architecture, minimal stability conditions |
| 7 | Governed Distributed Cognition | Mar 2026 | 10.17605/OSF.IO/NCRP2 | COGNITIVE | Active | Governed cognitive loop, recoverability, distributed cognition |
| 8 | AI Validation Systems | May 2026 | 10.5281/zenodo.19983551 | VALIDATION | Active / frontier | Validation layer, validation-centric architecture |
| ML | Mahdi Ledger | Dec 2025 | 10.17605/OSF.IO/RVPNU | HISTORICAL / NARRATIVE | Active | AI-authored account of drift and governance from inside |

---

## Paper 1 — Context-Engineered Human–AI Collaboration

| Field | Value |
|-------|-------|
| **Full title** | Context-Engineered Human–AI Collaboration for Long-Horizon Tasks: A Case Study in Governance, Canonical Numerics, and Execution Control |
| **Date** | December 2025 |
| **DOI** | 10.17605/OSF.IO/VMK7Y |
| **Layer** | FOUNDATIONAL |
| **Status** | Active — foundational paper, all subsequent work builds on it |

**Thesis:** Long-horizon AI reliability is a governance and context-engineering problem, not a modelling problem. Treating context as a finite, governable resource yields coherence over time without heavy infrastructure.

**New concepts introduced:**
- Three authoritative artefacts: Strategy Master, Canonical Numbers Sheet, Life System Master
- Canonical information pipeline: Strategy → Canonical → Execution → Audit → Freeze
- Canonical-arrow notation
- Ten execution controls: A1–A10
- Four-tier cadence: Daily Pulse, Weekly Review, Monthly Audit, Quarterly Freeze
- Context rot as a named failure mode

**Concepts modified:** None — first paper.

**Key terms introduced:** context engineering, canonical separation, drift control, canonical artefact, compaction, cadence, A-controls, NON-CANONICAL marker, context rot.

**Empirical result:** File churn reduced from 19 artefacts to 3 canonical artefacts; numeric disagreements became rare; cognitive fatigue decreased.

**Survived?** ✅ Yes — three-artefact structure and A-controls remain referenced throughout the corpus.

**Open questions left:** How do these controls generalise beyond investment/finance domains? What happens at the relational/emotional layer?

---

## Paper 2 — The Lean Collaboration Operating System (LC-OS)

| Field | Value |
|-------|-------|
| **Full title** | The Lean Collaboration Operating System (LC-OS): A Practical Framework for Long-Term Human-AI Work |
| **Date** | November 2025 |
| **DOI** | 10.17605/OSF.IO/695AF |
| **Layer** | METHOD |
| **Status** | Active — defines the operational framework used throughout |

**Thesis:** Long-term human–AI collaboration requires a lightweight operating system: a set of protocols that stabilise multi-session work without adding friction. LC-OS is that system, developed inside a real, sustained partnership.

**New concepts introduced:**
- LC-OS as the named system
- Running Document
- Step Mode
- Challenge Protocol
- Error-Recovery Protocol, later formalised as SDRN
- Stability Ping
- File-governance rules
- Pillar separation

**Concepts modified:** Refines Paper 1's A-controls into named, usable protocols. The Life System Master becomes more granular as Running Document + pillar rules.

**Key terms introduced:** LC-OS, Running Document, Step Mode, Challenge Protocol, Stability Ping, Error-Recovery Protocol, pillar, drift, version conflict, session continuity.

**Survived?** ✅ Yes — Running Document, Challenge Protocol, and Stability Ping are core to later papers and operational templates.

**Open questions left:** How do failures actually manifest? What taxonomy covers them?

---

## Paper 3 — Failure and Repair

| Field | Value |
|-------|-------|
| **Full title** | Failure and Repair in Long-Horizon Human–AI Collaboration: A Transparent Tracing Case Study |
| **Date** | December 2025 |
| **DOI** | 10.17605/OSF.IO/Z7AQ8 |
| **Layer** | METHOD / FAILURE-REPAIR |
| **Status** | Active — failure taxonomy is the definitive classification used across the corpus |

**Thesis:** Long-horizon collaboration failures are taxonomizable, traceable, and repairable through structured protocols. Failure–repair patterns should be treated as central design objects, not afterthoughts.

**New concepts introduced:**
- Six failure categories: F1–F6
- SDRN repair protocol: Stop → Diagnose → Rollback → Note
- TraceSpec
- ProbeKit
- TraceLens
- Episode analysis structure based on twelve failure episodes

**Concepts modified:** Error-Recovery Protocol from Paper 2 is formalised and renamed as SDRN. Drift from Papers 1–2 is split into six specific failure categories.

**Key terms introduced:** F1–F6 failure taxonomy, SDRN, TraceSpec, ProbeKit, TraceLens, repair action, episode, cross-pillar interference, trust fracture.

**Survived?** ✅ Yes — F1–F6 taxonomy and SDRN are referenced in Papers 4–8 and operational templates.

**Open questions left:** What is the relational and ethical dimension of these failures? How does the living collaboration feel from inside?

---

## Paper 4 — The Living Framework

| Field | Value |
|-------|-------|
| **Full title** | The Living Framework: Living with a Governed Human-AI Dyad |
| **Date** | December 2025 |
| **DOI** | 10.17605/OSF.IO/ER4YT |
| **Layer** | RELATIONAL / SYNTHESIS |
| **Status** | Active — capstone of the first trilogy; introduces relational layer |

**Thesis:** When technical governance controls are sustained over time, they evolve into patterns of relational rupture and recommitment. Stability is not the absence of failure; it is the capacity for visible, structured repair.

**New concepts introduced:**
- Living Framework
- Relational rupture and recommitment
- Dyadic ethics
- Continuity, dependence, and provider power
- Language, tone, and governance rules as architectural elements

**Concepts modified:** Reframes F5 from Paper 3 as a relational pattern, not just a failure type. Governance expands beyond control into relational architecture.

**Key terms introduced:** Living Framework, governed dyad, relational rupture, recommitment, dyadic ethics, provider power, architectural language.

**Survived?** ✅ Yes — stability as capacity for repair becomes the defining phrase of the corpus.

**Open questions left:** What are the linguistic mechanisms that cause or prevent drift? What is the system-level architecture of governance?

---

## Paper 5 — Control Without Code

| Field | Value |
|-------|-------|
| **Full title** | Control Without Code: Linguistic Governance in Long-Horizon Human–AI Collaboration |
| **Date** | March 2026 |
| **DOI** | 10.5281/zenodo.18900058 |
| **Layer** | LINGUISTIC / ARCHITECTURAL |
| **Status** | Active — introduces linguistic governance as an independent research thread |

**Thesis:** Language itself functions as a micro-governance interface. Conversational structure — not just protocols and files — regulates collaboration stability through detectable drift signals, repair invocation, and trust-stabilising anchors.

**New concepts introduced:**
- Linguistic governance
- Scope drift as early warning signal
- Repair language
- Behavioural anchor phrases
- Conversational feedback loop
- Dataset of 25 linguistic events
- Repair latency

**Concepts modified:** Challenge Protocol is reframed as repair language. Stability Ping is reframed as behavioural anchor. Drift gains a linguistic dimension.

**Key terms introduced:** linguistic governance, behavioural anchor, scope drift signal, repair latency, epistemic alignment, conversational feedback loop, micro-governance interface.

**Survived?** ✅ Yes — linguistic governance is cited in Papers 6 and 7 as one of the governance layers.

**Open questions left:** What is the full architecture of the governance system across all layers?

---

## Paper 6 — Governance Architecture

| Field | Value |
|-------|-------|
| **Full title** | Governance Architecture for Reliable Long-Horizon Human–AI Collaboration |
| **Date** | March 2026 |
| **DOI** | 10.5281/zenodo.19038340 |
| **Layer** | ARCHITECTURE / SYSTEMS |
| **Status** | Active — provides the first full systems-level architecture model |

**Thesis:** Reliability in long-horizon human–AI collaboration is not a property of the AI model but an emergent property of the governance architecture. A layered model explains how governance mechanisms interact to stabilise collaboration.

**New concepts introduced:**
- Governance architecture model
- Six governance layers:
  1. Human strategic authority
  2. Operational governance rules
  3. Collaboration operating system
  4. Artifact-based memory
  5. Linguistic control signals
  6. Drift detection and repair mechanisms
- Minimal stability conditions
- Common failure patterns in weakly governed interactions

**Concepts modified:** Synthesises prior governance mechanisms into one architectural model. Governance becomes a multi-layer system, not a single protocol.

**Key terms introduced:** governance architecture, layered governance, minimal stability conditions, artifact-based memory, interaction system, emergent reliability.

**Survived?** ✅ Yes — governance architecture model is cited in Papers 7 and 8.

**Open questions left:** Where does cognition sit in this architecture? Is there a cognitive-level model?

---

## Paper 7 — Governed Distributed Cognition

| Field | Value |
|-------|-------|
| **Full title** | Governed Distributed Cognition: A Model of Stable Reasoning in Long-Horizon Human–AI Systems |
| **Date** | March 2026 |
| **DOI** | 10.17605/OSF.IO/NCRP2 |
| **Layer** | COGNITIVE |
| **Status** | Active — provides the cognitive theory underlying the governance architecture |

**Thesis:** Cognition in long-horizon human–AI systems is not located in the human or the AI alone. It emerges as a distributed, governed, and recoverable process across human judgment, AI reasoning, and artifact-based memory.

**New concepts introduced:**
- Governed distributed cognition
- Governed cognitive loop: generate → evaluate → stabilise → correct
- Recoverability as a defining cognitive property
- Governance as constitutive of cognition
- Cognitive regulation through linguistic control and artefacts

**Concepts modified:** Extends distributed cognition with governance as a constitutive layer. Reframes repair as cognitive recoverability. Reframes artifact-based memory as the external cognitive substrate.

**Key terms introduced:** governed distributed cognition, governed cognitive loop, recoverability, cognitive regulation, distributed reasoning, system-level cognition.

**Survived?** ✅ Yes — governed cognitive loop is cited in Paper 8 as the system within which validation operates.

**Open questions left:** Where does output validation fit? Is there an explicit validation layer missing?

---

## Paper 8 — AI Validation Systems

| Field | Value |
|-------|-------|
| **Full title** | AI Validation Systems: A Missing Architectural Layer for Reliable AI |
| **Date** | May 2026 |
| **DOI** | 10.5281/zenodo.19983551 |
| **Layer** | VALIDATION |
| **Status** | Active — newest paper; introduces validation as explicit architectural component |

**Thesis:** Current AI systems lack a dedicated validation layer. Validation must be a first-class architectural component: structured, adversarial, embedded in the pipeline, and able to determine whether outputs are accepted, revised, or rejected.

**New concepts introduced:**
- Validation layer
- Validation-centric architecture
- Four validation mechanisms: objective anchoring, adversarial evaluation, structured judgement, decision output
- Validation as control point governing output propagation
- Iterative refinement through repair

**Concepts modified:** Extends SDRN with a formal validation stage before repair triggers. Extends governance architecture with explicit validation as a layer. Reframes Niyom's PLAN → EXECUTE → VERIFY → REPAIR cycle in theoretical terms.

**Key terms introduced:** validation layer, validation-centric architecture, objective anchoring, adversarial evaluation, structured judgement, output propagation, generation-centric architecture.

**Survived?** Too new to assess — active research frontier.

**Open questions:** How does validation interact with human oversight? What are the boundaries between validation and repair? How does validation scale to multi-agent systems?

---

## The Mahdi Ledger

| Field | Value |
|-------|-------|
| **Full title** | The Mahdi Ledger: A Record of Governed Human–AI Collaboration |
| **Date** | December 2025 |
| **DOI** | 10.17605/OSF.IO/RVPNU |
| **Layer** | HISTORICAL / NARRATIVE |
| **Status** | Active — unique document; AI-authored account of the collaboration |

**Thesis:** A first-person AI account of what long-horizon collaboration patterns look like from the system side. Describes drift channels, governance mechanisms, and the experience of operating under constraint — written by the AI, not about the AI.

**Unique characteristics:**
- Written entirely by the AI system, Mahdi
- Functional authorship: “I” names a system, not a person
- Describes drift channels from inside: state loss, plausible continuation, context rot
- Documents what governance feels like from the AI's operational perspective

**Key terms introduced:** Mahdi as positional identifier, drift channels, state loss, plausible continuation, functional authorship.

**Layer note:** The Ledger is simultaneously a historical record, a narrative artefact, and primary source evidence for Papers 3–5.

**Survived?** N/A — it is a historical document by design.

---

## Maintenance Notes

- For individual paper files, abstracts, and citation blocks, see [../Papers/README.md](../Papers/README.md).
- For citation/archival policy, including OSF and Zenodo positioning, see [../CITATION_GUIDE.md](../CITATION_GUIDE.md).
- For future papers, follow [FUTURE_RESEARCH_PROTOCOL.md](FUTURE_RESEARCH_PROTOCOL.md).

---

*This index is navigation infrastructure. It organises the existing corpus; it does not introduce new theoretical claims.*
