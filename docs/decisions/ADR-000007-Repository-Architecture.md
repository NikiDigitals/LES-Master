# ADR-000007 — Repository Architecture

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

The Life Enterprise System (LES) is a multi-module, long-term project spanning 5 years and encompassing 13 functional modules plus infrastructure and portfolio components. A decision was required on how to structure the codebase and documentation across GitHub to support this scope while maintaining clarity, consistency, and professional standards.

Three options were considered:

1. A single monolithic repository containing all modules
2. A GitHub Organisation with one repository per module
3. All repositories under a single personal account (NikiDigitals) with consistent naming conventions

---

## Decision

All repositories sit directly under the NikiDigitals personal GitHub account. No separate Organisation is used. A total of 15 repositories are established, one per module plus master, infrastructure, and portfolio components.

**Naming convention:** `LES-[UPPERCASE]` for all repositories except the master repository which is named `LES`.

**Repository list:**

| Repository | Purpose |
|---|---|
| `LES` | Master — documentation, architecture, governance, decisions, research, journal |
| `LES-INFRASTRUCTURE` | Azure Infrastructure as Code — all environments |
| `LES-PORTFOLIO` | NikiDigitals website documentation |
| `LES-API` | Central API gateway layer |
| `LES-CORE` | Shared libraries and common utilities |
| `LES-FIN` | Finance & Wealth Management |
| `LES-EDU` | Education & Knowledge |
| `LES-PRJ` | Projects & Goals |
| `LES-KNW` | Knowledge Base |
| `LES-HLT` | Health & Performance |
| `LES-REL` | Relationships & Network |
| `LES-OPS` | Daily Operations |
| `LES-INT` | Intelligence & Analytics |
| `LES-AGT` | AI Agent Orchestration |
| `LES-SEC` | Security, GRC & Compliance |

**Visibility:** `LES` is public. All other repositories are private until content reaches a presentable standard.

**Creation rule:** Repositories are created when content exists — never speculatively. All 15 were created as empty placeholders at the start of Phase 0 to establish the full architecture.

---

## Universal Folder Structure

Every repository follows the same internal structure:

```
LES-[MODULE]/
├── README.md
├── docs/
│   ├── architecture/
│   │   └── diagrams/
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

One `TEMPLATE.md` per folder — each template sits inside the folder it applies to, eliminating cross-referencing at scale.

---

## Rationale

A single personal account was selected over a GitHub Organisation for simplicity of management and single professional identity. The volume of repositories (15) does not warrant the overhead of an Organisation at this stage, and the architecture supports migration if that decision changes.

Separate repositories per module reflect the enterprise principle of separation of concerns. Each module is independently versioned, independently documented, and independently deployable. This mirrors how real enterprise systems are structured and directly supports the Finance Transformation Architect career objective.

The uppercase naming convention was adopted for visual consistency and professional readability across all repository listings.

---

## Consequences

- All 15 repositories must follow the same internal folder structure without exception
- Security is a cross-cutting concern embedded in every repository — LES-SEC governs the framework, individual repositories implement it
- Any future migration to a GitHub Organisation is supported — repository names and structures do not need to change
- The universal template structure means onboarding any future collaborator requires no explanation of where to find things
