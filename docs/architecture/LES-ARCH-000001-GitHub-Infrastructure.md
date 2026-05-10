# LES-ARCH-000001 — GitHub Infrastructure Architecture

**Date:** May 2026
**Status:** Active — Phase 0
**Owner:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Overview

This document defines the GitHub infrastructure architecture for the Life Enterprise System (LES). It covers the repository structure, internal folder conventions, template standards, and naming conventions that apply across all 15 repositories.

This document is the authoritative reference for GitHub infrastructure decisions. All deviations require a new ADR.

---

## Account Structure

**GitHub Account:** github.com/NikiDigitals

All repositories sit directly under the NikiDigitals personal account. No GitHub Organisation is used at this stage. This decision is recorded in ADR-007.

---

## Repository Inventory

| Repository | Type | Purpose | Visibility | Phase Active |
|---|---|---|---|---|
| `LES` | Master | Documentation, architecture, governance, decisions, research, journal | Public | Phase 0 — now |
| `LES-INFRASTRUCTURE` | Operational | Azure Infrastructure as Code — all environments | Private | Phase 1 |
| `LES-PORTFOLIO` | Operational | NikiDigitals website documentation | Private | Phase 0 — now |
| `LES-API` | Operational | Central API gateway layer | Private | Phase 2 |
| `LES-CORE` | Shared | Shared libraries and common utilities | Private | Phase 2 |
| `LES-FIN` | Module | Finance & Wealth Management | Private | Phase 1 |
| `LES-EDU` | Module | Education & Knowledge | Private | Phase 1 |
| `LES-PRJ` | Module | Projects & Goals | Private | Phase 1 |
| `LES-KNW` | Module | Knowledge Base | Private | Phase 1 |
| `LES-HLT` | Module | Health & Performance | Private | Phase 2 |
| `LES-REL` | Module | Relationships & Network | Private | Phase 2 |
| `LES-OPS` | Module | Daily Operations | Private | Phase 2 |
| `LES-INT` | Module | Intelligence & Analytics | Private | Phase 3 |
| `LES-AGT` | Module | AI Agent Orchestration | Private | Phase 4 |
| `LES-SEC` | Module + Cross-cutting | Security, GRC & Compliance | Private | Phase 0 — framework |

---

## Universal Folder Structure

Every repository follows this internal structure without exception:

```
LES-[MODULE]/
├── README.md
├── docs/
│   ├── architecture/
│   │   ├── diagrams/
│   │   │   └── TEMPLATE.md
│   │   └── TEMPLATE.md
│   ├── decisions/
│   │   └── TEMPLATE.md
│   ├── governance/
│   │   └── TEMPLATE.md
│   ├── research/
│   │   └── TEMPLATE.md
│   └── roadmap/
│       └── TEMPLATE.md
├── journal/
│   └── TEMPLATE.md
└── TEMPLATE.md
```

### Exceptions

Three repositories have additional folders:

| Repository | Additional Folder | Purpose |
|---|---|---|
| `LES` | `_context/` | Master context document — session briefing file |
| `LES-INFRASTRUCTURE` | `environments/` | Azure environment-specific configurations |
| `LES-PORTFOLIO` | `website/` | WordPress content in markdown format |

---

## Template Convention

One `TEMPLATE.md` per folder. Each template sits inside the folder it applies to.

**Rationale:** At scale, a single master template file requires cross-referencing. One template per folder eliminates that dependency. Opening any folder reveals immediately what a document inside it should look like.

---

## Document Taxonomy

All documents follow the taxonomy established in ADR-014:

| Code | Type | Location |
|---|---|---|
| `ADR-[NNN]` | Architecture Decision Records | `docs/decisions/` |
| `LES-ARCH-[NNN]` | Architecture Documents | `docs/architecture/` |
| `LES-DIAG-[NNN]` | Diagrams | `docs/architecture/diagrams/` |
| `LES-ROAD-[NNN]` | Roadmaps | `docs/roadmap/` |
| `LES-[MOD]-[NNN]` | Module Specifications | `docs/LES-[MOD]/` |
| `LES-GOV-[NNN]` | Governance Frameworks | `docs/governance/` |
| `LES-RES-[NNN]` | Research Notes | `docs/research/` |
| `LES-JOUR-[NNN]` | Learning Journal | `journal/` |

---

## README Standard

Every repository README follows this structure:

```markdown
# LES-[MODULE] — [Full Name]

**Part of:** Life Enterprise System (LES)
**Owner:** NikiDigitals
**Status:** [Planned / In Progress / Active]
**Phase:** [Phase number when this module becomes active]
**Visibility:** [Public / Private]

## Purpose
[One paragraph — what this repository contains and why it exists]

## Repository Structure
[Folder tree]

## Related Repositories
[Links to dependent or related repos]

## Documentation
[Link to GitBook section for this module]
```

---

## Naming Conventions

| Element | Convention | Example |
|---|---|---|
| Repository name | `LES-[UPPERCASE]` | `LES-FIN`, `LES-SEC` |
| Document files | `[CODE]-[NNN]-[kebab-title].md` | `ADR-007-Repository-Architecture.md` |
| Commit messages | `[Session type] — [description]` | `LES-MENTOR Week 1 — Added ADR-007` |
| Branch names | `[type]/[kebab-description]` | `docs/add-adr-007` |

---

## Version History

| Version | Date | Changes |
|---|---|---|
| 1.0 | May 2026 | Initial architecture document established |
