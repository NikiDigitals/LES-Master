# Master Roadmap — Repository Architecture

*Document code: LES-ROAD-001 v3.8 | Phase 0 | May 2026*

---

LES is structured across 18 repositories under the NikiDigitals personal GitHub account at `github.com/NikiDigitals`. There is no separate GitHub Organisation — all repositories sit under one professional identity.

---

## Repository Map

| Repository | Type | Purpose | Visibility |
|---|---|---|---|
| `NikiDigitals` | Profile | GitHub profile README — NikiDigitals professional identity | Public |
| `LES-Master` | Master | Architecture, governance, decisions, research, journal | Public |
| `LES-INFRA` | Operational | Azure Infrastructure as Code — all environments | Private |
| `LES-PORT` | Operational | NikiDigitals portfolio website — documentation, content, future custom build | Private |
| `LES-API` | Operational | Central API gateway layer | Private |
| `LES-CORE` | Shared | Shared libraries and common utilities | Private |
| `LES-DASH` | Operational | Dashboard — Power BI Phase 1–2, custom React from Phase 3 | Private |
| `LES-demo-data` | Demo | Synthetic data generation for demo environment | Private |
| `LES-FIN` | Module | Finance & Wealth Management | Private |
| `LES-EDU` | Module | Education & Knowledge | Private |
| `LES-PRJ` | Module | Projects & Goals | Private |
| `LES-KNW` | Module | Knowledge Base | Private |
| `LES-HLT` | Module | Health & Performance | Private |
| `LES-REL` | Module | Relationships & Network | Private |
| `LES-OPS` | Module | Daily Operations | Private |
| `LES-INT` | Module | Intelligence & Analytics | Private |
| `LES-AGT` | Agent Layer | Custom-built multi-agent orchestration system | Private |
| `LES-SEC` | Module + Cross-cutting | Security, GRC & Compliance | Private |

---

## Universal Folder Structure

Every repository follows the same internal structure without exception.

```
LES-[MODULE]/
├── README.md
├── src/
│   └── tests/
├── docs/
│   ├── architecture/
│   │   └── diagrams/
│   ├── decisions/
│   ├── governance/
│   ├── research/
│   ├── roadmap/
│   └── specs/
├── journal/
└── TEMPLATE.md
```

---

## Repository Principles

- Every repository follows the same internal folder structure without exception
- Security is a cross-cutting concern — LES-SEC governs the framework, individual repositories implement it
- Repositories are made public only when content reaches a presentable standard
- `LES-Master` remains public as the project's public face on GitHub
- All 18 repositories were created as placeholders during Phase 0 to establish the full architecture

---

*Developed by [NikiDigitals](https://nikidigitals.com)*
