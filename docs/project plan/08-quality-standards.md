# Project Plan — Quality Standards

*Document code: LES-PLAN-v2.3 | Phase 0 | May 2026*

---

## Definition of Done

A module or feature is not considered complete until all of the following criteria are met:

- The data model is documented in the module specification and deployed to Azure SQL
- All code is committed to the module repository with clear, meaningful comments
- The GitBook documentation entry for this component is written and published
- At least one ADR documents the key architectural decision for this component
- The functionality has been used in real life — not just tested in isolation
- The CHANGELOG in the module repository is updated

---

## Code Quality Standards

- All code is version controlled. Nothing exists only on a local machine.
- Commit messages follow the convention: `[Session type] — [description]`
- Sensitive data — credentials, personal financial data, health data — is never committed to a repository
- Infrastructure is always defined as code in LES-INFRA. No manual Azure portal configuration that is not also in code.

---

## Documentation Quality Standards

- Every document is written in UK English
- Tone is businesslike and professional throughout
- Every document includes a document control section with version history
- GitHub holds working documentation. GitBook holds published, reader-facing documentation — updated manually when documents are complete.
- No document is considered published until reviewed for clarity and completeness

---

## Architecture Quality Standards

- No architectural decision is implemented without a corresponding ADR
- ADR files follow the convention `ADR-YYYY-MM-DD.md` — one file per day, decisions grouped by subject
- The complete data model is designed before any module is built
- Security is considered at every layer — not added after the fact
- Cost implications are assessed at every phase gate
- Diagrams follow confirmed standards: C4 Model (architecture), BPMN 2.0 (process), ERD (data), Azure Architecture icons (infrastructure) — all in draw.io

---

## Journal Standards

- One journal entry per week — covers all sessions across all days that week
- Document code: LES-JOUR-000[NNN]
- Published to GitBook when content is substantial, standalone, and reader-facing

---

*Developed by [NikiDigitals](https://nikidigitals.com)*
