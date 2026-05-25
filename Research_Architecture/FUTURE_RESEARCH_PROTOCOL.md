# Future Research Protocol

**Purpose:** A governance framework for how future research papers enter the LC-OS corpus.
No isolated papers going forward — all new research enters the system.

**Effective from:** 2026-05-25  
**Applies to:** All future papers under the LC-OS / Living Framework research program

---

## The Problem This Protocol Solves

The corpus grew organically across Papers 1–8. Each paper was valuable. But because
they arrived without a common entry protocol, the corpus now requires significant
navigation infrastructure (this Research Architecture folder) to make coherent.

Going forward, each new paper should be positioned within the corpus *before* it is
written, not after. This protocol provides that positioning.

---

## Step 1: Paper Classification

Before beginning a new paper, answer this question:

**What type of contribution is this?**

| Type | Description | Example |
|------|-------------|---------|
| **New idea** | Introduces a concept not present in existing corpus | Paper 5 (linguistic governance) |
| **Extension** | Develops an existing concept further | Paper 4 extending Paper 3's F5 |
| **Correction** | Identifies and corrects an error or incompleteness in a prior paper | — |
| **Rename** | Proposes renaming a term based on the TERM_REGISTRY review process | — |
| **Merge** | Synthesises two or more existing concepts into a unified model | Paper 6 (architecture synthesis) |
| **Retirement** | Argues that a concept is no longer valid and should be deprecated | — |
| **Operationalization** | Translates a research finding into an operational tool | Note: this goes to LC-OS-Project, not to the research corpus |

---

## Step 2: Layer Assignment

Assign the new paper to one of the six research layers (see RESEARCH_LAYER_SEPARATION.md).

If the paper spans multiple layers, identify the *primary* layer and note the secondary
layers it touches.

---

## Step 3: Dependency Mapping

List the prior papers the new paper builds on. Be explicit:
- "This paper assumes familiarity with Paper X"
- "This paper corrects Claim Y from Paper Z"
- "This paper extends Concept W introduced in Paper V"

---

## Step 4: Term Registration

Before submission, audit all new terms introduced in the paper.

For each new term:
1. Check TERM_REGISTRY — does the term already exist under a different name?
2. If new: add it to TERM_REGISTRY in EXPERIMENTAL status
3. If it renames an existing term: follow the TERM_REGISTRY rename process
4. If it merges two existing terms: update both entries and add the merged term

---

## Step 5: RESEARCH_INDEX Entry

After submission, add an entry to RESEARCH_INDEX.md using the standard template:
- Title, date, DOI, layer, status
- Thesis
- New concepts introduced
- Concepts modified
- Key terms (link to TERM_REGISTRY)
- Survived? (leave as "Too new to assess" initially)
- Open questions

---

## Step 6: RESEARCH_EVOLUTION_MAP Update

After publication, update RESEARCH_EVOLUTION_MAP.md:
- Add the paper to the chronological view
- Update any concept lineage rows that the paper extends
- Update the conceptual dependency map

---

## Step 7: UNIFIED_SYNTHESIS Update

After publication, update UNIFIED_SYNTHESIS.md:
- Add the paper to Section 2 (Evolution of Thought) as a new stage if it represents
  a genuinely new direction
- Update Section 3 (Current Worldview) if any claims have changed
- Update Section 7 (Open Research Questions) — close questions the paper answers,
  add questions the paper opens

---

## What This Protocol Prevents

| Without protocol | With protocol |
|-----------------|---------------|
| Papers add terms without checking existing corpus vocabulary | All new terms checked against TERM_REGISTRY first |
| Papers introduce concepts without connecting them to prior work | Dependency mapping required before writing |
| Corpus grows without a map of how papers relate | RESEARCH_INDEX and EVOLUTION_MAP updated on each paper |
| New readers cannot navigate without reading everything | UNIFIED_SYNTHESIS kept current |
| Same concept gets named differently across papers | TERM_REGISTRY governs naming |

---

## Operationalization is Not Research

A recurring risk: practitioners ask "can you write a paper about the init script /
the examples / the Niyom integration?"

The answer is no — not as LC-OS research papers. Operational work (templates, scripts,
tools, workflows) belongs in LC-OS-Project, not in the research corpus.

A paper is appropriate when it introduces, extends, corrects, or synthesises a *concept*.
A practitioner guide, a tool, or a worked example is appropriate for LC-OS-Project.

The boundary:
- **Research corpus** → ideas, models, frameworks, empirical findings
- **LC-OS-Project** → tools, templates, examples, automation

When in doubt: would this paper be citable in another researcher's work on human–AI
collaboration theory? If yes → research corpus. If no → LC-OS-Project.

---

## Minimum Viable Protocol

If the full protocol is too much for a given paper, at minimum:
1. Classify the paper type
2. Assign a layer
3. Add a TERM_REGISTRY entry for every new term
4. Update RESEARCH_INDEX after publication

The EVOLUTION_MAP and SYNTHESIS updates can follow on a quarterly cadence rather
than per-paper if volume increases.

---

*No isolated papers going forward. Research enters the system.*
