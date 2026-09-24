# Paper 1 Correction Map — Batch 3

**Status:** Working correction record.  
**Scope:** Results through Appendices. This document identifies necessary corrections only; it does not author a new paper.

## Results and Discussion

| ID | Original location and problem | Minimum correction | Why |
|---|---|---|---|
| P1-CM-031 | Setup: approximately 60 sessions, June–October 2025, and four measurement methods. It also says all work was manual but assigns an “Automatic A1 log parse.” | Replace with a brief historical-context statement. State that the public record does not contain a session register, definitions, denominators, or the claimed logs; do not present a dataset or measurement procedure. | The collection procedure is internally inconsistent and the supporting records are unavailable. |
| P1-CM-032 | Setup: “behavioural validation” and “reproducible reliability.” | Change to a design description developed in one human–AI collaboration, suitable for prospective evaluation. | The available record cannot validate efficacy or reproducibility. |
| P1-CM-033 | Quantitative Outcomes: every reported outcome (file churn, numeric errors, latency, qualitative load, gift capture). | Remove the complete outcome list and the statement that constraints outperform larger context windows. Add one concise limitation/disclosure that historical outcome estimates cannot be verified from available records. | The quantitative claims lack the necessary underlying data; file-churn figures also conflict internally. |
| P1-CM-034 | Qualitative Observations: error correlations, 27% E5 rate, 180-token average, >98% retention, and >4.5/5 human-and-AI trust rating. | Remove numerical and causal claims. Retain only the described safeguards as historical examples or prospective practices. | No supporting records, instruments, or valid AI-participant measure exist. |
| P1-CM-035 | Practitioner Guidance: “Most drift disappears,” “prevents entropy accumulation,” and similar result language. | Retain only as conditional suggestions: “may be considered” / “is intended to support.” | The steps were not empirically proven by this record. |
| P1-CM-036 | Synthesis: twelve audit cycles, 91% and 68% improvements, 30,000-token threshold, <2% loss, and causal/model-scale conclusion. | Remove all figures and causal conclusion. State that the paper reports a proposed architecture whose effectiveness requires prospective testing. | The evidence is unavailable or internally inconsistent; comparative conclusion was not studied. |
| P1-CM-037 | Table 2 — A-Control Effectiveness Summary. | Remove the full table. Do not replace it with a new evaluation table. | It combines conflicting A1–A10 labels with unsupported control-specific effects and confidence ratings. |

## Limitations, Adoption, Ethics, and Conclusion

| ID | Original location and problem | Minimum correction | Why |
|---|---|---|---|
| P1-CM-038 | Limitations: “control stack substantially improves,” performance beyond 60k tokens, “error suppression collapses,” and durable gains. | Retain limitations but remove performance conclusions and specific threshold. Describe limits in non-quantified terms and say effectiveness remains unverified. | Corrects overclaim while preserving the paper’s cautionary function. |
| P1-CM-039 | Process scope: “invariant design principles are portable.” | Change to “the practices have not been tested beyond this setting.” | Portability is untested. |
| P1-CM-040 | Metrics: “numeric drift and file-churn reductions are clear.” | Replace with “the paper’s reported historical outcomes cannot be independently checked from the available materials.” | This is the central evidence correction. |
| P1-CM-041 | Adoption Playbook: one-week roll-out and named A-controls. | Retain only as a clearly labelled illustrative workflow, if needed to preserve Paper 1’s original structure; remove mandatory or outcome-guaranteeing wording. Add the A1–A10 historical-collision disclosure where the labels appear. | The paper may describe a workflow, but cannot claim this is a validated deployment protocol. |
| P1-CM-042 | Expected Benefits: blank/unspecified reduction, fatigue improvement, zero breaches, and full reproducibility. | Remove the full subsection. | It promises outcomes with no valid evidence. |
| P1-CM-043 | Ethics: “every control … ensures” safeguards; claims of storage/deletion practice, immutable/redactable logs, chain-of-custody, continuous oversight, demonstrable psychological effects, and replayable decisions. | Retain a modest ethical-position section. Change absolute or factual operational claims to design intentions, and delete any statement not supported by available artefacts. Do not claim legal, privacy, or ethical compliance. | The paper does not document sufficient evidence for these guarantees. |
| P1-CM-044 | Conclusion: “demonstrates,” “achieved,” quantitative benefits, same-model comparison, generalisation, and “three artefacts and ten controls suffice.” | Rewrite only the conclusion sentences needed to say: Paper 1 documents a proposed architecture from one collaboration; it does not establish effectiveness, model comparison, generalisability, or reproducibility. Preserve the concise final design proposition. | The conclusion must not restore claims retired elsewhere. |

## Authorship, availability, references, and appendices

| ID | Original location and problem | Minimum correction | Why |
|---|---|---|---|
| P1-CM-045 | Author Contributions: it credits ChatGPT as a joint contributor, says it “implemented” controls, and says both contributors reviewed and approved the manuscript. | Replace with an accurate AI-assistance disclosure. Rishi Sood remains the sole human author and project lead; disclose use of ChatGPT for assistance without asserting AI authorship, independent review, or approval. | AI cannot be an accountable co-author or approver; the existing statement overstates human review as well. |
| P1-CM-046 | Data and Materials Availability: promises artefacts, logs, and supplementary materials that are not available. | Replace with a frank unavailable-materials statement naming the missing records and explaining that the correction does not reconstruct them. | Materials promised by Paper 1 cannot currently support its outcome claims. |
| P1-CM-047 | References: a mixture of primary literature, blogs, and entries requiring source verification. | Do not add references merely to support new claims. Retain only sources that are correctly identified and directly support the limited remaining text; record any removal separately. | A corrected paper needs accurate citations, not a larger bibliography. |
| P1-CM-048 | Appendix A pseudocode; Appendix B outcome logs; Appendices C–J examples, registries, templates, checklists, and claimed replication package. | Remove any appendix that asserts unauthenticated code, logs, outcomes, material availability, or reproducibility. Do not replace them with newly created templates or expanded technical content. If a short appendix list is retained, it must state only what is historically published and what is unavailable. | These appendices contain missing-evidence claims and were a major source of the abandoned 83-page expansion. |
| P1-CM-049 | Figures 1–2 describe A-control relationships and gates despite the unresolved A1–A10 collision. | Retain the general three-artefact flow figure only if its wording is narrowed to a proposed/design flow. Remove or quarantine the control-stack figure unless it can be made accurate without silently resolving the label collision. | Avoids a visual assertion that contradicts the text. |

## Batch 3 acceptance test

1. No Results table, appendix, or conclusion claims efficacy, statistical/quantitative improvement, causation, reproducibility, or generalisability without authenticated evidence.
2. All missing materials are disclosed plainly; none are promised as available.
3. The correction removes unsupported material; it does not replace it with new theory, templates, pseudocode, frameworks, or literature.
4. The corrected paper remains recognisably Paper 1, with its original design purpose intact.
