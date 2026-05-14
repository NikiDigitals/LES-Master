# Master Roadmap — Technology Stack

*Document code: LES-ROAD-001 v3.8 | Phase 0 | May 2026*

---

The following represents the confirmed and proposed technology stack for LES. Items marked "Confirmed" are decided. Items marked "To be confirmed" will be discussed, understood, and confirmed before adoption.

| Layer | Technology | Status |
|---|---|---|
| Cloud Platform | Microsoft Azure | Confirmed |
| Database (Relational) | Azure SQL Database | To be confirmed |
| Database (NoSQL) | Azure Cosmos DB | To be confirmed |
| Data Warehouse | Microsoft Fabric / Synapse | To be confirmed |
| Serverless Compute | Azure Functions | To be confirmed |
| Workflow Automation | Azure Logic Apps | To be confirmed |
| Analytics & Reporting | Microsoft Fabric & Power BI | To be confirmed |
| Front-end (Personal) | Power Apps / Power BI | To be confirmed |
| Dashboard | Power BI Phase 1–2, custom React Phase 3+ | Confirmed |
| AI & LLM Infrastructure | Azure OpenAI Service | To be confirmed |
| Agent Architecture | Custom-built from first principles | Confirmed |
| Version Control | GitHub | Confirmed |
| Documentation (GitHub) | Markdown — technical reference version | Confirmed |
| Documentation (GitBook) | Narrative version — manually published | Confirmed |
| Infrastructure as Code | Azure Bicep | To be confirmed |
| Programming Language | Python | To be confirmed |
| Identity & Access | Azure Entra ID | To be confirmed |
| Monitoring | Azure Monitor / Application Insights | To be confirmed |
| Diagramming | draw.io | Confirmed |

---

## Diagramming Standards

All LES diagrams follow a consistent professional standard:

| Diagram Type | Standard | Use Case |
|---|---|---|
| System architecture | C4 Model | Component relationships, system context, container diagrams |
| Process flows | BPMN 2.0 | Module workflows, agent decision flows, integration flows |
| Data models | ERD notation | Entity relationships, database schemas |
| Infrastructure | Azure Architecture icons | Azure resource diagrams, networking, subscriptions |

Reference: [c4model.com](https://c4model.com) — [omg.org/spec/BPMN](https://www.omg.org/spec/BPMN)

---

## Agent Architecture — A Note

LES-AGT is not built on a pre-packaged agent framework. Azure OpenAI Service provides the LLM engine only — the underlying language model capability. The agents themselves — their architecture, orchestration layer, context management, memory, inter-agent communication, and decision logic — are designed and built as part of LES from first principles.

Semantic Kernel, AutoGen, and LangChain are studied for architectural patterns. They are not adopted.

The distinction matters: using an agent framework demonstrates familiarity with a tool. Building one from scratch demonstrates understanding of what the tool actually does.

---

*Developed by [NikiDigitals](https://nikidigitals.com)*
