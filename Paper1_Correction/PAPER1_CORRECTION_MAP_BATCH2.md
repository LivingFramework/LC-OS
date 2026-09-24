# Paper 1 Correction Map — Batch 2

**Status:** Working correction record.  
**Scope:** Related Work and Methods/Control Stack only. This document specifies minimum corrections; it is not a replacement manuscript.

## Related Work

| ID | Original location and problem | Minimum correction | Why |
|---|---|---|---|
| P1-CM-014 | Related Work: broad statement that “few studies” formalise governance, provenance, or numeric reproducibility. | Narrow to a non-quantified framing statement, or remove. | No systematic review supports “few studies.” |
| P1-CM-015 | Related Work: technical equations, thresholds, and effect estimates presented as factual background (for example retrieval degradation, reasoning variance, interference, factual-fidelity loss, entropy bounds, and coordination overhead). | Remove unsupported equations, numerical thresholds, and claimed empirical laws. Keep only cited, qualitative descriptions where the cited source directly supports them. | The paper does not establish these figures and the citations do not support all of the mathematical precision. |
| P1-CM-016 | Related Work: phrases claiming deterministic or reproducible operations as achieved properties (“reproducible lookup,” “deterministic regeneration,” “finite-state process,” “reproducibility parity”). | Change to “documented lookup/checkpoint procedure” or equivalent conditional language. | The available record does not establish deterministic model reasoning or reproducibility parity. |
| P1-CM-017 | RAG subsection: “0 unresolved ID collisions across N = 842 retrieval events.” | Remove. | No event log or denominator is available. |
| P1-CM-018 | Memory subsection: “Human audits confirmed zero semantic drift over 12 cycles (<0.5% edit distance).” | Remove the quantitative result. Retain only that compaction notes were used as part of the described approach. | No audit dataset, source/digest pairs, metric definition, or reproducible comparison is available. |
| P1-CM-019 | Provenance subsection: immutable conversational Merkle-chain, “Verification latency <20ms (N=1,024),” and “reproducibility parity.” | Retain only the design idea of recording provenance where records exist; remove the hash-chain assertion, latency figure, sample size, and parity claim. | The public record does not contain the claimed operational logs or benchmark. |
| P1-CM-020 | Human–AI Teaming subsection: claimed balanced coupling and sustainable cognitive load after 50 sessions. | Retain human-confirmation as a proposed safeguard; remove claimed trust bounds and cognitive-load result. | The measurement and evidence are unavailable; the AI cannot be treated as an independently rated human participant. |
| P1-CM-021 | Related Work synthesis: “model-agnostic,” “any transformer or agentic loop can adopt this control stack without retraining.” | Replace with “the proposed practices may require adaptation and prospective testing across systems.” | Portability and model-agnosticism were not tested. |

## Methods and Control Stack

| ID | Original location and problem | Minimum correction | Why |
|---|---|---|---|
| P1-CM-022 | Architecture: the three artefacts are described as a “minimal cognitive stack.” | Keep as a description of the case design; delete “minimal” unless expressly framed as the authors’ design choice. | No comparative basis establishes minimality. |
| P1-CM-023 | Cadence and Decision Boundary: “mitigates context rot,” “prevents silent drift,” and “preserves reproducibility.” | Change each to “is intended to reduce…” or “is intended to support…”. | These are prospective design aims, not verified effects. |
| P1-CM-024 | Control Stack table: it reuses A1–A10 for a second, incompatible set of control names. | Preserve the historical table only with the global collision disclosure from Batch 1, or remove the table if it cannot be presented without making control-specific claims. Do not introduce a new namespace. | The source has two incompatible A1–A10 mappings; choosing one would falsely resolve the record. |
| P1-CM-025 | Worked examples, pseudocode, extended example, formal semantics, and key syntax are presented as the historical system, including named assets, thresholds, and operational outcomes. | Remove from corrected Paper 1 unless a particular item can be directly authenticated as a contemporaneous design artefact. No replacement technical specification is to be added. | These sections transform the paper into a new technical guide and contain unauthenticated specifics. |
| P1-CM-026 | Methods: “algorithmic gate,” “deterministic reasoning,” and assertions that a procedure “ensures procedural determinism.” | Replace only where needed with “documented check” / “proposed guard”; do not claim deterministic model behaviour. | The distinction is necessary for accuracy. |
| P1-CM-027 | Error Taxonomy: “Error frequency … decreased >90% across 60 sessions.” | Remove. | The event records and denominator are unavailable. |
| P1-CM-028 | Human Factors: “maintains … while avoiding fatigue” and five-minute pause “measurably reduces error variance by ≈15%.” | Recast as a proposed pause safeguard; remove measured-effect wording. | No valid outcome data or defined variance analysis exists. |
| P1-CM-029 | Security & Privacy: “ensures compliance with baseline GDPR principles.” | Replace with “privacy and compliance requirements require context-specific assessment; this paper does not provide legal certification.” | A design description cannot certify GDPR compliance. |
| P1-CM-030 | Implementation Blueprint: tiers and “Tier 1 yields most of the reliability benefit.” | Remove the tier-benefit claim. Retain only a short, clearly prospective implementation illustration if needed for the original paper’s purpose. | No tier comparison or benefit evidence exists. |

## Batch 2 acceptance test

1. No technical formula, performance figure, benchmark, log count, or threshold remains unless directly supported by the cited source or authenticated record.
2. The A1–A10 collision is disclosed, never silently repaired.
3. The paper does not acquire a new specification, pseudocode appendix, or technical-guide character.
4. Architecture statements remain descriptions or proposals, never evidence of effectiveness, portability, or legal compliance.
