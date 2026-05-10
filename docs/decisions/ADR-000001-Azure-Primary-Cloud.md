# ADR-000001 — Azure as Primary Cloud Platform

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

A primary cloud platform was required for all LES infrastructure. The decision determines where compute, storage, databases, AI services, and identity management are hosted for the duration of the project.

Platforms evaluated: Microsoft Azure, Amazon Web Services (AWS), Google Cloud Platform (GCP).

## Decision

Microsoft Azure is the primary cloud platform for all LES infrastructure. Alternative platforms are adopted only where they are demonstrably superior for a specific function and the integration overhead is justified.

## Rationale

- Microsoft ecosystem alignment — Microsoft 365, Power Platform, GitHub, and Azure form a coherent stack
- Certification pathway — Azure certifications (AZ-900 through AZ-305) map directly to the Finance Transformation Architect career target
- Enterprise credibility — Azure is the dominant platform in enterprise finance environments
- Azure OpenAI Service — direct access to GPT-4 models within the Azure security boundary, relevant for LES-AGT
- Data sovereignty — Azure provides EU-based data residency options aligned with personal data governance requirements

## Consequences

- All infrastructure is provisioned in Azure unless a specific exception is justified and documented
- Exceptions require a new ADR documenting the alternative platform, the function, and the justification
- Azure certifications are the primary certification pathway
- Cost management is an ongoing concern — Azure free tier used initially, consumption model adopted as usage grows
