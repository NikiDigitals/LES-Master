# Project Plan — Risk Register

*Document code: LES-PLAN-v2.3 | Phase 0 | May 2026*

---

| # | Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|---|
| R-001 | Motivation loss over a 5-year programme | Medium | High | Public accountability via LinkedIn. Modular structure ensures always something completable. Certification milestones provide external momentum. |
| R-002 | Azure cloud costs exceed budget | Low | Medium | Cost alerts configured from day one. Azure free tier maximised in Phase 0–1. Architecture reviewed at each phase gate for cost efficiency. |
| R-003 | Scope creep expands project beyond manageable size | High | High | Formal scope definition in place. Change management process enforced. ADR required before any scope addition. |
| R-004 | Learning pace slower than phase plan assumes | Medium | Low | Phase timeline is guidance, not constraint. Depth over speed is a foundational principle. Phases have no hard external deadlines. |
| R-005 | Technology choices become obsolete | Low | Medium | Architectural principles chosen over specific tools. Azure ecosystem aligned with enterprise direction. Review at each phase gate. |
| R-006 | Azure platform outage or service disruption | Low | Low | Architecture designed for resilience. Personal data sovereignty maintained. Backup and recovery documented in LES-SEC. |
| R-007 | Documentation discipline breaks down under build pressure | Medium | Medium | Weekly journal standard. Minimum one commit per session. Master context updated every session without exception. |
| R-008 | Data architecture requires major redesign mid-project | Low | High | Complete data model designed in Phase 1 before any module is built. All entities and relationships defined upfront. Schema migrations managed formally. |
| R-009 | Real personal data accidentally exposed during demonstration | Low | High | Completely separate Azure subscription for demo environment. No shared resources between production and demo. Demo environment populated exclusively with synthetic data. |

---

*Developed by [NikiDigitals](https://nikidigitals.com)*
