# Research Layer Separation

**Purpose:** Organises the corpus into distinct layers so readers can navigate
to exactly the kind of content they need — theory, method, tools, or templates.

**Last updated:** 2026-05-25

---

## The Six Layers

```
┌─────────────────────────────────────────────────────────────────────┐
│  LAYER 6: OPERATIONAL                                               │
│  LC-OS-Project: templates, examples, init scripts, checklists       │
├─────────────────────────────────────────────────────────────────────┤
│  LAYER 5: VALIDATION                                                │
│  Paper 8: Validation layer, validation-centric architecture         │
├─────────────────────────────────────────────────────────────────────┤
│  LAYER 4: COGNITIVE                                                 │
│  Paper 7: Governed distributed cognition, cognitive loop            │
├─────────────────────────────────────────────────────────────────────┤
│  LAYER 3: ARCHITECTURAL                                             │
│  Papers 5–6: Linguistic governance, governance architecture         │
├─────────────────────────────────────────────────────────────────────┤
│  LAYER 2: METHOD                                                    │
│  Papers 2–4: LC-OS protocols, failure taxonomy, relational layer    │
├─────────────────────────────────────────────────────────────────────┤
│  LAYER 1: FOUNDATIONAL                                              │
│  Paper 1: Context engineering, A-controls, canonical artefacts      │
├─────────────────────────────────────────────────────────────────────┤
│  HISTORICAL LAYER (runs alongside all others)                       │
│  Mahdi Ledger: AI-authored first-person account                     │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Layer 1: Foundational

**Content:** Paper 1  
**What it contains:** The core argument that reliability is a governance problem.
Three authoritative artefacts. Ten A-controls. The canonical information pipeline.
The four-tier cadence. Empirical evidence from one deployment.

**Who should read this:** Anyone starting with the corpus. This is the entry point.

**Key claims:**
- Context is a finite, governable resource
- Three artefacts are sufficient for baseline governance
- Reliability = process design, not model size

---

## Layer 2: Method

**Content:** Papers 2, 3, 4  
**What it contains:** The named operating system (LC-OS), its protocols (Running
Document, Step Mode, Challenge Protocol, Stability Ping), the failure taxonomy
(F1–F6), the repair protocol (SDRN), and the relational extension.

**Who should read this:** Practitioners implementing LC-OS. Researchers studying
failure patterns in human–AI systems.

**Key claims:**
- LC-OS is the operational instantiation of Layer 1 theory
- Failure follows six predictable categories
- SDRN converts failure into improvement
- Stability is the capacity for repair, not the absence of failure

---

## Layer 3: Architectural

**Content:** Papers 5, 6  
**What it contains:** Linguistic governance (language as micro-governance mechanism)
and the full six-layer governance architecture model.

**Who should read this:** System designers. Researchers building on the framework.
Anyone asking "why does this work?" rather than "how do I use it?"

**Key claims:**
- Conversational structure is itself a governance mechanism
- Governance has six distinct, interacting layers
- Reliability is emergent across these layers — not reducible to any one

---

## Layer 4: Cognitive

**Content:** Paper 7  
**What it contains:** The cognitive theory of long-horizon human–AI systems.
Distributed cognition, governed cognitive loop, recoverability.

**Who should read this:** Researchers in human–computer interaction, cognitive
science, or AI theory. Anyone asking "what kind of cognitive system is this?"

**Key claims:**
- Cognition in human–AI systems is distributed across human, AI, and artefacts
- Governance is constitutive of cognition, not just a constraint
- Recoverability is the key cognitive property that governance preserves

---

## Layer 5: Validation

**Content:** Paper 8  
**What it contains:** The argument for validation as a missing architectural layer.
Validation-centric architecture, four validation mechanisms, validation as control point.

**Who should read this:** AI system architects. Researchers studying AI reliability.
Anyone building systems where output quality is critical.

**Key claims:**
- Current AI systems lack a dedicated validation layer
- Validation must be embedded in the pipeline, not bolted on
- Reliability requires validation-centric, not generation-centric, architecture

---

## Historical Layer

**Content:** The Mahdi Ledger  
**What it contains:** The AI's first-person account of the collaboration. Drift
channels described from inside the system. Governance as experienced by the governed.

**Who should read this:** Anyone interested in AI perspective-taking, narrative
accounts of AI collaboration, or primary source evidence for Papers 3–5.

**Key characteristics:**
- Written entirely by the AI system ("Mahdi"), not by the human researcher
- Functional authorship: "I" names a system function, not a person
- Unique in the corpus: the only document describing the collaboration from the AI side

---

## Operational Layer

**Content:** LC-OS-Project repository  
**What it contains:** All operational outputs — templates, examples, init scripts,
checklists, the Practitioners Guide. The practitioner implementation of the research.

**Relationship to research layers:** The operational layer is not part of the
research corpus. It is the practitioner output of that corpus.

| Research Layer | Operational output |
|----------------|--------------------|
| Foundational (Paper 1) | Strategy Master template, Canonical Numbers template |
| Method (Papers 2–4) | Running Document, Stability Ping, Challenge Protocol, Failure Log, SDRN |
| Architectural (Papers 5–6) | Session-start protocols, scope rules |
| Cognitive (Paper 7) | (No direct template — theoretical foundation for all) |
| Validation (Paper 8) | (Niyom VERIFY stage — separate engineering project) |

**Important:** LC-OS-Project is operational output, not research. Changes to
LC-OS-Project do not require updating research papers. Research findings may
update operational templates, but not the reverse.

---

## How to Use This Layer Map

**Reading a paper:** Check its layer. Foundational layer papers require no prior
reading. Method layer papers assume Paper 1. Architecture layer assumes Papers 1–4.
Cognitive layer assumes Papers 1–6. Validation layer assumes Papers 1–7.

**Building on the research:** Identify which layer your contribution targets.
New operational tools → Operational Layer (LC-OS-Project). New failure patterns →
Method Layer. New governance mechanisms → Architectural Layer.

**Teaching the corpus:** Start at Layer 1. Add layers as needed. The Mahdi Ledger
can be introduced anywhere — it enriches any layer.
