# Operationalization Audit

**Purpose:** Review the LC-OS-Project practitioner toolkit and classify each artefact
by its current form and potential for automation. This is a classification exercise —
not an implementation plan.

**Scope:** All templates and documents in the LC-OS-Project repository.  
**Last updated:** 2026-05-25

---

## Audit Framework

For each artefact, we ask:

| Question | Options |
|----------|---------|
| Current form | Manual template / Worked example / Script / Checklist |
| Automation candidate? | Schema / Script / Plugin / Runtime / None |
| Effort to automate | Low / Medium / High |
| Value of automating | Low / Medium / High |
| Priority | Now / Later / Never |

**Definitions:**
- **Schema** — can be expressed as a data schema (YAML/JSON) for structured storage
- **Script** — can be automated as a CLI script (e.g., init, validate, update)
- **Plugin** — could become an AI tool plugin or MCP server
- **Runtime** — requires real-time execution during collaboration (e.g., Niyom's VERIFY)

---

## Audit Results

### scripts/init-project.js
| Field | Value |
|-------|-------|
| Current form | Script (Node.js) |
| Automation candidate | Script — already automated ✅ |
| Notes | Bootstraps a new LC-OS project. Consider: `npx lc-os-init` wrapper for zero-install use. |

---

### minimal/running-document-template.md
| Field | Value |
|-------|-------|
| Current form | Manual template |
| Automation candidate | Schema + Script |
| Effort | Medium |
| Value | High |
| Priority | Later |
| Notes | Could become a YAML schema with a CLI to generate the Markdown. More valuable: a CLI command to update the decisions log or add a correction without opening the file manually. |

---

### minimal/canonical-numbers-template.md
| Field | Value |
|-------|-------|
| Current form | Manual template |
| Automation candidate | Schema + Plugin |
| Effort | Medium |
| Value | High |
| Priority | Later |
| Notes | High schema candidate — tables of numbers map naturally to structured data. A plugin that reads the canonical numbers and makes them available to AI at session start without manual copy-paste would eliminate a significant friction point. |

---

### minimal/failure-log-template.md
| Field | Value |
|-------|-------|
| Current form | Manual template |
| Automation candidate | Schema + Script |
| Effort | Low |
| Value | Medium |
| Priority | Later |
| Notes | TraceSpec schema from Paper 3 is already a spec for this. A script that creates a new dated failure entry with the right fields would reduce the friction of logging (people skip logging when it's manual). |

---

### full/STRATEGY-MASTER-TEMPLATE.md
| Field | Value |
|-------|-------|
| Current form | Manual template |
| Automation candidate | Script (guided setup) |
| Effort | Medium |
| Value | Medium |
| Priority | Later |
| Notes | The init script already handles simple strategy master creation. A more interactive CLI that walks through each section would improve adoption for non-technical users. |

---

### full/challenge-protocol.md
| Field | Value |
|-------|-------|
| Current form | Manual reference document |
| Automation candidate | Runtime (AI system prompt fragment) |
| Effort | Low |
| Value | High |
| Priority | Now |
| Notes | The Challenge Protocol is essentially a prompt fragment that the AI should have active during sessions. Could be distributed as a Claude project instruction snippet rather than a document to paste. |

---

### full/repair-protocol.md (SDRN)
| Field | Value |
|-------|-------|
| Current form | Manual reference document |
| Automation candidate | Runtime |
| Effort | High |
| Value | High |
| Priority | Later (Niyom handles this) |
| Notes | SDRN is partially automated by Niyom's VERIFY→REPAIR pipeline. Full automation requires detecting failure onset, which is a runtime AI capability, not a template. The manual document remains necessary for human-side repair. |

---

### full/stability-ping-template.md
| Field | Value |
|-------|-------|
| Current form | Manual template |
| Automation candidate | Script (scheduled) |
| Effort | Low |
| Value | Medium |
| Priority | Later |
| Notes | A scheduled task (Cowork's scheduling feature) could trigger a Stability Ping reminder after N sessions or after a configurable time gap. Low effort, meaningful nudge. |

---

### Weekly-Review-Checklist.md
| Field | Value |
|-------|-------|
| Current form | Manual checklist |
| Automation candidate | Script (scheduled reminder + auto-populate) |
| Effort | Medium |
| Value | High |
| Priority | Later |
| Notes | A scheduled task that opens a pre-populated weekly review session with current date and pulls in canonical numbers for review would significantly increase consistency of the weekly practice. |

---

### examples/ (all domain examples)
| Field | Value |
|-------|-------|
| Current form | Worked examples (static Markdown) |
| Automation candidate | Script (generate new domain example from template) |
| Effort | Low |
| Value | Medium |
| Priority | Later |
| Notes | A CLI command `node scripts/new-example.js [domain]` that generates a blank domain folder with the right structure would help practitioners create their own domain examples. |

---

### references/Practitioners_Guide.md
| Field | Value |
|-------|-------|
| Current form | Markdown document |
| Automation candidate | PDF generator (GitHub Action via Pandoc) |
| Effort | Low |
| Value | Medium |
| Priority | Later |
| Notes | A GitHub Action that auto-generates a PDF from the Markdown on push would keep the PDF in sync without manual conversion. |

---

## Priority Summary

| Priority | Artefacts | Notes |
|----------|-----------|-------|
| **Now** | Challenge Protocol → AI prompt snippet | Low effort, high value, no code required |
| **Later — Low effort** | Failure log entry script, Stability Ping scheduler, PDF auto-generation | Quick wins |
| **Later — Medium effort** | Canonical numbers schema + plugin, Running Document CLI updater, weekly review auto-populate | High value but requires more design |
| **Later — High effort** | Full SDRN automation, multi-artefact sync | Niyom handles the runtime layer; LC-OS-Project handles the human layer |
| **Never** | Strategy Master full automation | Strategic decisions cannot and should not be automated |

---

## What Should Not Be Automated

- **Strategy Master content** — principles and scope require human judgment
- **Failure log analysis** — pattern recognition across failures is a human synthesis task
- **Decisions in the decisions log** — decisions are human; logging them can be assisted

---

## Next Steps

This audit is a classification. Implementation depends on priorities set by the researcher.
The most immediately actionable item (Challenge Protocol as prompt snippet) requires no
code and could be added to LC-OS-Project immediately as a `prompt-snippets/` folder.
