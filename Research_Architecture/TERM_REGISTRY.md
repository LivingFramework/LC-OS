# Term Registry

**Purpose:** Single source of truth for terminology across the LC-OS corpus.
Every significant term used in the research is defined here, with its origin,
current status, and notes on usage.

**Rule:** When writing about LC-OS research, use terms as defined here.
If a term is Deprecated, use the Candidate Replacement instead.
If a term is under Review, use it but note the ambiguity.

**Last updated:** 2026-05-25

---

## How to Read This Registry

| Column | Meaning |
|--------|---------|
| **Term** | The term as used in the corpus |
| **Definition** | Meaning within the LC-OS corpus (may differ from general usage) |
| **Origin** | Paper where term was introduced |
| **Status** | Active / Experimental / Deprecated / Merged / Under Review |
| **Notes** | Usage notes, common confusions, related terms |
| **Candidate replacement** | Alternative term if under review or deprecated |

---

## Status Definitions

| Status | Meaning |
|--------|---------|
| **Active** | In current use; meaning is stable |
| **Experimental** | Used in one paper; not yet validated across the corpus |
| **Deprecated** | No longer preferred; use candidate replacement |
| **Merged** | Absorbed into a broader term |
| **Under Review** | Actively debated; do not treat as settled |

---

## Core Terms

### Canonical Artefact (also: Authoritative Artefact, Authoritative File)
| | |
|--|--|
| **Definition** | A designated file that holds the single source of truth for one domain of information. There are three canonical artefacts: Strategy Master (textual truth), Canonical Numbers Sheet/Canonical Numbers (numeric truth), Running Document (session/cadence truth). |
| **Origin** | Paper 1 |
| **Status** | Active |
| **Notes** | "Authoritative file" is used interchangeably. "Canonical artefact" is the more formal term. In operational practice (LC-OS-Project), often just called "the three files." |
| **Candidate replacement** | N/A |

---

### Canonical Numbers Sheet (also: Canonical Numbers)
| | |
|--|--|
| **Definition** | The single authoritative source for all numerical data in a collaboration. Any number not in this file is NON-CANONICAL and cannot drive decisions. |
| **Origin** | Paper 1 |
| **Status** | Active |
| **Notes** | Shortened to "Canonical Numbers" in LC-OS-Project templates. The Sheet suffix is a legacy from the original spreadsheet implementation. |
| **Candidate replacement** | N/A |

---

### Context Engineering
| | |
|--|--|
| **Definition** | The deliberate design of information state that conditions a model at inference time — what sources are trusted, what is authoritative, what must be re-verified. Distinct from prompt engineering (which tunes phrasing). |
| **Origin** | Paper 1 |
| **Status** | Active |
| **Notes** | Paper 1 frames the entire research as a context engineering problem. Subsequent papers expand the scope but context engineering remains the foundational frame. |
| **Candidate replacement** | N/A |

---

### Context Rot
| | |
|--|--|
| **Definition** | The degradation of AI collaboration quality over time as small inconsistencies accumulate, context expands uncontrolled, and the model loses coherent grounding in authoritative state. |
| **Origin** | Paper 1 |
| **Status** | Active |
| **Notes** | The named failure mode that motivates the entire research program. Related to F1 (Context & Memory Drift) but broader — context rot is the structural risk; F1 is a specific episode type. |
| **Candidate replacement** | N/A |

---

### Drift
| | |
|--|--|
| **Definition** | The gradual, often invisible departure of AI reasoning, outputs, or decisions from authoritative state. Can be numerical (F3), contextual (F1), linguistic (Paper 5), or relational (F5). |
| **Origin** | Paper 2 (named); Paper 1 (implicit as "context rot") |
| **Status** | Active |
| **Notes** | The corpus's unifying failure concept. When used without qualification, refers to general collaboration degradation. For precision, use the F1–F6 category. |
| **Candidate replacement** | N/A |

---

### F1 — Context & Memory Drift
| | |
|--|--|
| **Definition** | Failure category: AI loses accurate context across sessions or within a session; decisions are made on outdated or reconstructed information. |
| **Origin** | Paper 3 |
| **Status** | Active |
| **Notes** | Most common failure type. Primary prevention: Running Document shared at session start. |
| **Candidate replacement** | N/A |

---

### F2 — File & Version Divergence
| | |
|--|--|
| **Definition** | Failure category: Multiple versions of a file exist; it is unclear which is current; edits are applied to wrong versions. |
| **Origin** | Paper 3 |
| **Status** | Active |
| **Notes** | Prevented by single-source-of-truth discipline (A2) and file registry (A3). |
| **Candidate replacement** | N/A |

---

### F3 — Numerical Reasoning Errors
| | |
|--|--|
| **Definition** | Failure category: AI recalculates, estimates, or invents numerical values rather than referencing the Canonical Numbers file. |
| **Origin** | Paper 3 |
| **Status** | Active |
| **Notes** | Prevented by A2 (Single Source of Truth for numbers). One of the most consequential failure types in high-stakes domains. |
| **Candidate replacement** | N/A |

---

### F4 — Governance & Boundary Violations
| | |
|--|--|
| **Definition** | Failure category: AI or human operates outside agreed scope, ignores established rules, or crosses explicit constraints. |
| **Origin** | Paper 3 |
| **Status** | Active |
| **Notes** | Prevented by explicit scope definition in Strategy Master and Challenge Protocol. Includes scope creep, pillar boundary violations, and rule abandonment. |
| **Candidate replacement** | N/A |

---

### F5 — Emotional / Trust Fractures
| | |
|--|--|
| **Definition** | Failure category: The relational trust between human and AI degrades; the human stops believing the AI's outputs are honest or reliable. |
| **Origin** | Paper 3 |
| **Status** | Active |
| **Notes** | Extended in Paper 4 into a full relational theory (rupture and recommitment). Related to sycophancy — AI telling the human what they want to hear rather than what is true. |
| **Candidate replacement** | N/A |

---

### F6 — Cross-Pillar Interference
| | |
|--|--|
| **Definition** | Failure category: Context, decisions, or emotional load from one life/work domain bleeds into another, causing contamination of reasoning or priorities. |
| **Origin** | Paper 3 |
| **Status** | Active |
| **Notes** | Prevented by pillar separation rules in the Running Document. Particularly relevant in personal productivity use cases. |
| **Candidate replacement** | N/A |

---

### Governance
| | |
|--|--|
| **Definition** | Within the LC-OS corpus: the structured mechanisms that regulate, constrain, and repair human–AI collaboration to maintain reliability over time. Encompasses protocols, artefacts, linguistic signals, and relational norms. |
| **Origin** | Paper 1 (as A-controls); fully theorised in Paper 6 |
| **Status** | ⚠️ Under Review |
| **Notes** | See special review section below. |
| **Candidate replacement** | See special review |

---

### Governed Cognitive Loop
| | |
|--|--|
| **Definition** | The recurrent process through which reasoning is generated, evaluated, stabilised, and corrected in a long-horizon human–AI system: generate → evaluate → stabilise → correct. |
| **Origin** | Paper 7 |
| **Status** | Active |
| **Notes** | The cognitive-level model of how the governance architecture functions at the reasoning layer. |
| **Candidate replacement** | N/A |

---

### LC-OS (Lean Collaboration Operating System)
| | |
|--|--|
| **Definition** | The named framework for long-horizon human–AI collaboration: a minimal set of protocols, artefacts, and rules that stabilise multi-session work. |
| **Origin** | Paper 2 |
| **Status** | Active |
| **Notes** | The name of the entire research program and practitioner toolkit. "Lean" is intentional — the system is minimal by design. |
| **Candidate replacement** | N/A |

---

### Living Framework
| | |
|--|--|
| **Definition** | The governance structure understood as a living, relational entity — one that evolves through rupture and recommitment, not just through protocol updates. |
| **Origin** | Paper 4 |
| **Status** | Active |
| **Notes** | Also the name of the GitHub organisation (LivingFramework). The concept captures that governance in long-horizon collaboration is not static — it adapts through the collaboration's own history. |
| **Candidate replacement** | N/A |

---

### Minimal Stability Conditions
| | |
|--|--|
| **Definition** | The minimum governance mechanisms required for sustained long-horizon human–AI collaboration. Below these conditions, collaboration cannot remain stable regardless of model capability. |
| **Origin** | Paper 6 |
| **Status** | Active |
| **Notes** | Not fully enumerated in the corpus — this is a research-frontier concept. The operational approximation is: Running Document + Canonical Numbers + explicit scope. |
| **Candidate replacement** | N/A |

---

### NON-CANONICAL
| | |
|--|--|
| **Definition** | A marker applied to any numerical value that does not appear in the Canonical Numbers file. NON-CANONICAL values cannot drive decisions. |
| **Origin** | Paper 1 |
| **Status** | Active |
| **Notes** | A specific, enforceable designation — not a vague quality judgment. If a number isn't in the canonical file, it is NON-CANONICAL regardless of how plausible it sounds. |
| **Candidate replacement** | N/A |

---

### Pillar
| | |
|--|--|
| **Definition** | A distinct life or work domain within a collaboration that must be kept separate to prevent cross-pillar interference (F6). Examples: career, finance, health, a specific client project. |
| **Origin** | Paper 2 |
| **Status** | Active |
| **Notes** | Particularly relevant in personal productivity use cases. Pillar boundaries are defined in the Strategy Master. |
| **Candidate replacement** | N/A |

---

### Recoverability
| | |
|--|--|
| **Definition** | The property of a cognitive system (human–AI pair + artefacts) that enables it to return to coherent, governed reasoning after a failure or drift episode. |
| **Origin** | Paper 7 |
| **Status** | Active |
| **Notes** | Formalises what repair (Papers 3–5) achieves at the cognitive level. A system with high recoverability can sustain long-horizon work; a system without it degrades and cannot self-correct. |
| **Candidate replacement** | N/A |

---

### Running Document
| | |
|--|--|
| **Definition** | The persistent, session-level authoritative artefact that captures decisions, rules, corrections, open questions, and session notes. Shared with the AI at the start of every session. Functions as the collaboration's external memory. |
| **Origin** | Paper 2 |
| **Status** | Active |
| **Notes** | The most operationally important artefact. Equivalent to a ship's log for the collaboration. Replaces reliance on AI session memory. |
| **Candidate replacement** | N/A |

---

### SDRN (Stop → Diagnose → Rollback → Note)
| | |
|--|--|
| **Definition** | The four-step repair protocol for collaboration failures: Stop the current task, Diagnose what went wrong and why, Rollback to the last correct state, Note the failure in the failure log. |
| **Origin** | Paper 3 (formalises Error-Recovery Protocol from Paper 2) |
| **Status** | Active |
| **Notes** | The operational repair procedure. "Note" is critical — without logging, the same failure recurs. |
| **Candidate replacement** | N/A |

---

### Stability Ping
| | |
|--|--|
| **Definition** | A periodic, brief alignment check between human and AI: are we still working from the same understanding? Any drift? One improvement before continuing? |
| **Origin** | Paper 2 |
| **Status** | Active |
| **Notes** | Operational trigger: after major milestones, after long gaps, or when something feels "off." Not a formal audit — a quick check. |
| **Candidate replacement** | N/A |

---

### Strategy Master
| | |
|--|--|
| **Definition** | The canonical artefact holding textual truth: principles, policies, scope, and decision logic that remain stable across sessions. Not a working document — rarely updated. |
| **Origin** | Paper 1 |
| **Status** | Active |
| **Notes** | One of the three canonical artefacts. Distinguished from Running Document by stability: Strategy Master changes rarely; Running Document changes every session. |
| **Candidate replacement** | N/A |

---

### TraceSpec
| | |
|--|--|
| **Definition** | The minimal schema for logging failure episodes: trigger, symptom, potential damage, repair action, resulting change. |
| **Origin** | Paper 3 |
| **Status** | Active |
| **Notes** | The structured format behind the Failure Log template in LC-OS-Project. ProbeKit and TraceLens are companion tools. |
| **Candidate replacement** | N/A |

---

### Validation Layer
| | |
|--|--|
| **Definition** | A dedicated architectural component that evaluates AI-generated outputs against objectives, constraints, and potential failure conditions before those outputs are accepted and propagated. |
| **Origin** | Paper 8 |
| **Status** | Experimental (one paper; research frontier) |
| **Notes** | The newest concept in the corpus. Paper 8 argues this layer is currently missing from most AI systems. Niyom's VERIFY stage is an operational instantiation of this concept. |
| **Candidate replacement** | N/A |

---

## ⚠️ Special Review: "Governance"

### The Problem

The term "governance" is used throughout the corpus with shifting scope:

| Paper | How "governance" is used |
|-------|--------------------------|
| Paper 1 | A-controls; execution gates; file discipline |
| Paper 2 | Protocols; operating rules |
| Paper 4 | Architectural; relational; tonal |
| Paper 5 | Linguistic; embedded in dialogue |
| Paper 6 | Full six-layer system |
| Paper 7 | Constitutive of cognition |

Internally, this breadth is coherent — each paper adds a dimension.

Externally, "governance" is increasingly read as **policy/regulation/compliance**
(AI governance in the policy sense: EU AI Act, Responsible AI frameworks, etc.).
This creates a risk: readers arrive expecting policy/regulatory discussion and find
a system-level architecture paper. The word may be causing misrouting.

### Migration Analysis (Do NOT rename yet — analysis only)

| Candidate | Covers | Does not cover | Risk |
|-----------|--------|----------------|------|
| **Cognitive Control** | Papers 7–8 well | Relational layer (Paper 4) | Too narrow |
| **Reliability Layer** | Papers 1, 6, 8 well | Linguistic, relational dimensions | Too narrow |
| **Control Architecture** | Papers 5, 6, 7 well | Operational protocols (Paper 2) | Sounds technical-only |
| **Stability Layer** | Papers 2, 4 well | Validation dimension (Paper 8) | Too passive |
| **Coordination Layer** | Multi-agent context | Not right for human-AI dyad | Wrong register |
| **Collaboration Architecture** | Good for Papers 4–7 | Misses enforcement/control aspect | Too soft |
| **Supervisory Structure** | Papers 1, 6 well | Linguistic, relational | Too hierarchical |

### Recommendation

Do not rename. "Governance" works within the corpus because readers of the
corpus understand it in context. If external confusion becomes a documented
problem (e.g., wrong citations, misreadings in reviews), revisit this analysis.

The UNIFIED_SYNTHESIS should clarify the internal meaning of governance in its
opening section to pre-empt misreading.

---

*"A term without a registry becomes a Rorschach test."*
