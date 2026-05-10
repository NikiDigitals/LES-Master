# ADR-000002 — Data Sovereignty — Personal Azure Tenant First

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

LES holds deeply personal data across all modules — financial records, health metrics, relationship data, daily operations, learning history. A decision was required on where this data resides, who controls it, and what the governance model is.

## Decision

All personal data is stored in a personal Azure tenant under full NikiDigitals control. No third-party SaaS platforms hold primary data. Architecture is designed to support expansion — selective exposure of specific data to external services is permitted where justified and documented.

## Rationale

- Full ownership — no dependency on third-party data policies
- Azure security boundary — encryption, access control, and audit logging within a single tenant
- EU data residency — personal data stored in EU Azure regions
- Expansion optionality — architecture supports connecting external services without migrating the core data layer

## Consequences

- All module data models are designed for Azure SQL or Cosmos DB as primary stores
- External service integrations must justify data sharing — no default data sharing
- Each expansion of the data boundary requires a documented decision
- Cost is managed within the personal Azure tenant — no hidden SaaS data costs
