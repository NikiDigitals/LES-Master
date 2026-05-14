# Project Plan — System Architecture

*Document code: LES-PLAN-v2.3 | Phase 0 | May 2026*

---

## The Enterprise Analogy

Every enterprise ERP system is built around a set of functional modules — Finance, Human Resources, Supply Chain, Customer Relations, Manufacturing, and so forth. Each module manages a distinct business domain with its own data model, processes, and reporting layer. An integration layer connects all modules, enabling intelligence to flow across the entire organisation.

LES follows an identical architectural pattern. Each life domain is a module. Each module has its own Azure SQL database schema, its own API layer, its own reporting dashboard, and — by Phase 4 — its own dedicated AI agent. A central orchestration layer connects all modules and coordinates cross-domain intelligence.

---

## The LES Modules

| Module | Department | Scope | Phase |
|---|---|---|---|
| LES-FIN | Finance & Wealth Management | General ledger, budgeting, forecasting, investment tracking, tax awareness, financial reporting, CFO AI agent | Phase 1 |
| LES-EDU | Education & Knowledge | Learning tracker, certification log, course management, reading records, knowledge retention metrics | Phase 1 |
| LES-PRJ | Projects & Goals | Goal definition, project planning, task management, milestone tracking, execution analytics | Phase 1 |
| LES-KNW | Knowledge Base | Document management, research library, note organisation, semantic search, knowledge graph | Phase 1 |
| LES-HLT | Health & Performance | Biometric tracking, fitness logging, nutrition management, sleep analysis, performance trends | Phase 2 |
| LES-REL | Relationships & Network | Contact management, interaction history, network mapping, commitment tracking | Phase 2 |
| LES-OPS | Daily Operations | Routine management, habit tracking, calendar intelligence, operational efficiency metrics | Phase 2 |
| LES-INT | Intelligence & Analytics | Cross-module analytics, executive dashboard, predictive modelling, anomaly detection | Phase 3 |
| LES-SEC | Security, GRC & Compliance | Access control, data governance, audit logging, compliance framework, security monitoring | Phase 3 |
| LES-AGT | AI Agent Orchestration | Multi-agent system, department agents, orchestrator agent, natural language interface | Phase 4 |

---

## Technology Foundation

| Layer | Technology | Rationale |
|---|---|---|
| Cloud Platform | Microsoft Azure | Enterprise standard. Certification pathway aligned. |
| Database | Azure SQL Database | Relational, enterprise-grade, T-SQL skills directly transferable |
| File Storage | Azure Blob Storage | Documents, images, media at scale |
| Application Backend | Python with FastAPI | Readable, AI-ecosystem aligned, strong community |
| Automation | Azure Logic Apps & Azure Functions | Serverless workflows, event-driven architecture |
| Analytics & Reporting | Microsoft Fabric & Power BI | Enterprise analytics standard |
| AI & Language Models | Azure OpenAI Service | Enterprise AI — LLM engine only, not the agent framework |
| Agent Architecture | Custom-built from first principles | Agents designed and built as part of LES |
| Identity & Security | Microsoft Entra ID | Enterprise identity management standard |
| Infrastructure as Code | Azure Bicep | Reproducible, version-controlled infrastructure |
| Diagramming | draw.io | C4 Model (architecture), BPMN 2.0 (process), ERD (data), Azure icons (infrastructure) |

---

## Repository Architecture

LES is structured across 18 repositories under the NikiDigitals personal GitHub account. No separate GitHub Organisation — all repositories sit directly under `github.com/NikiDigitals`.

| Repository | Type | Purpose |
|---|---|---|
| `NikiDigitals` | Profile | GitHub profile README |
| `LES-Master` | Master | Architecture, governance, decisions, research, journal |
| `LES-INFRA` | Operational | Azure Infrastructure as Code |
| `LES-PORT` | Operational | NikiDigitals portfolio website |
| `LES-API` | Operational | Central API gateway |
| `LES-CORE` | Shared | Shared libraries and utilities |
| `LES-DASH` | Operational | Dashboard — Power BI Phase 1–2, custom React Phase 3+ |
| `LES-demo-data` | Demo | Synthetic data for demo environment |
| `LES-FIN` through `LES-AGT` | Modules | One per department |
| `LES-SEC` | Module + Cross-cutting | Security, GRC & Compliance |

---

## Environment Architecture

LES operates across two completely isolated Azure environments.

| | Production | Demo |
|---|---|---|
| **Purpose** | Personal daily operating system | Safe public demonstration |
| **Data** | Real personal data | Synthetic data only |
| **Azure Subscription** | Personal production subscription | Separate isolated subscription |
| **Access** | Private | Public — safe to show anyone |
| **Build Phase** | Phase 0 onwards | Phase 2 |

The demo environment is populated with a fully constructed fictional persona — a believable individual whose life data demonstrates every LES module meaningfully without exposing any real personal information. A dedicated repository — `LES-demo-data` — contains the scripts that generate and maintain the synthetic dataset.

---

*Developed by [NikiDigitals](https://nikidigitals.com)*
