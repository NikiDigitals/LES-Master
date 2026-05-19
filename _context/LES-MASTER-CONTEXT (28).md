# LES MASTER CONTEXT DOCUMENT

**Paste this at the start of every new Claude chat session.**
**Keep this file updated after every significant session.**
**Location:** GitHub → LES-Master → `_context/master-context.md`

**Companion files — update all three together:**
- `LES-MASTER-CONTEXT.md` — current state reference (this file)
- `LES-TASKS-COMPLETED.md` — permanent completed task log
- `LES-DECISIONS-INDEX.md` — full decision log

**Education sessions — also paste:**
- `LES-EDU-ARCH-002.md` — education architecture mentor context

---

## WHO I AM

**Full name:** Nicolette Martine Langendam
**Professional brand:** NikiDigitals
**Native language:** Dutch. All work is conducted in UK English.
**Tone preference:** Businesslike and professional in all documentation. Academic rigour in GitBook and research outputs.

---

## STUDENT PROFILE

**Technical level:** Absolute beginner. No prior development, cloud, or technical experience.
**Learning standard:** No shortcuts. Full understanding before moving forward. Depth of understanding is the goal, not speed of delivery.

**Formal education — current:**

| Programme | Institution | Level | Status |
|---|---|---|---|
| BSc (Hons) Computing & IT with Business | The Open University | Undergraduate | In progress |
| ACCA | Association of Chartered Certified Accountants | Professional Qualification | In progress |
| BSc Professional Accounting | University of London | Undergraduate | Planned — March 2028 intake |
| Masters in Artificial Intelligence | Udacity / Woolf University | Postgraduate | Planned — Y2Q1 start, low self-paced |

**Professional experience:**

| Role | Organisation | Period | Discipline |
|---|---|---|---|
| FP&A & Financial Modeling Extern | Confidential — NDA | May 2026 — Present | Finance |
| IoT Cyber Defense Extern | Hydroficient via Extern | Mar–Apr 2026 | Cybersecurity |
| Team Leader — Business Operations & Compliance | Pepagora via Excelerate | Apr 2026 — Present | Business |
| Project Leader — Business Development Strategy | Grant Thornton China via Excelerate | Feb–Mar 2026 | Strategy |
| Team Leader — Data Analytics Outreach | Saint Louis University via Excelerate | Dec 2025–Jan 2026 | Analytics |
| Student Trustee | Open University Students Association | Aug 2026–Jul 2027 | Governance |

---

## PROFESSIONAL GOAL

**Target role:** Finance Transformation Architect
**Specialisation:** Finance systems — broad, complex, and complete
**Timeline:** 4–5 years, developing alongside LES

Primary filter for every decision: *"Does this make me a better Finance Transformation Architect?"*

---

## PROFESSIONAL IDENTITY — NIKIDIGITALS

**Mission:** To build expertise so deep, so rigorously documented, and so openly published that it becomes a reference point for the experts who come after.

**Tagline:** Finance | Systems | Technology

**Brand system:**

| Token | Name | Hex |
|---|---|---|
| Primary background | Navy Night | `#0D1B2A` |
| Accent | Circuit Blue | `#4A90B8` |
| Accent light | Signal Blue | `#7AB3CC` |
| Page background | Off-White | `#F4F7FA` |
| Body text | Charcoal | `#1A2B3C` |
| Muted text | Slate | `#5C7A8A` |
| Reversed text | White | `#FFFFFF` |

**Typography:** Syne Bold (headings) + DM Sans (body)

---

## THE PROJECT — Life Enterprise System (LES)

**Concept:** An enterprise-grade ERP architected around a human life. Every life domain treated as a business department with its own data model, processes, intelligence layer, and AI agent.

**Timeline:** 5 years to expert level. Ongoing thereafter.
**Primary cloud:** Microsoft Azure. Alternatives adopted where demonstrably superior.
**AI strategy:** Custom-built multi-agent system from first principles. Azure OpenAI Service provides the LLM engine only.

---

## THE MODULES

| Code | Department | Phase |
|---|---|---|
| LES-FIN | Finance & Wealth Management | 1 |
| LES-EDU | Education & Knowledge | 1 |
| LES-PRJ | Projects & Goals | 1 |
| LES-KNW | Knowledge Base | 1 |
| LES-HLT | Health & Performance | 2 |
| LES-REL | Relationships & Network | 2 |
| LES-OPS | Daily Operations | 2 |
| LES-INT | Intelligence & Analytics | 3 |
| LES-SEC | Security, GRC & Compliance | 3 |
| LES-AGT | AI Agent Orchestration | 4 |

---

## THE PORTFOLIO ARCHITECTURE

Three distinct project types exist under the NikiDigitals brand. Each has its own GitHub convention, GitBook section, and portfolio treatment.

| Type | Purpose | GitHub | GitBook | Portfolio card |
|---|---|---|---|---|
| LES — Flagship | The ERP project | `LES-[MODULE]` — 18 repos | All main sections | Full card — flagship |
| LES Labs | Learning sandboxes — all domains | `LES-LABS-[TOPIC]-[NNN]` | Labs section | One NikiDigitals Labs card |
| Standalone projects | Independent NikiDigitals builds | `ND-[PROJECT-NAME]` | Projects section | Full card per public project |

**GitHub profile structure — long term:**

```
github.com/NikiDigitals
├── LES-[MODULE]              ← Flagship — 18 repos
├── LES-LABS-[TOPIC]-[NNN]   ← All learning sandboxes — all domains
└── ND-[PROJECT-NAME]         ← Standalone NikiDigitals projects
```

**Standalone project documentation:**

| Project type | GitHub | Portfolio treatment |
|---|---|---|
| Academic — restricted | Private repo | Case study write-up only — no code |
| Academic — demonstrable | Public repo | Full card |
| Externship — NDA | Not published | Mentioned in experience only |
| Externship — public | Public repo | Full card |
| NikiDigitals tool | Public repo | Full card |

**GitBook sections:**

| Section | Content |
|---|---|
| Labs | All LES-LABS sandbox projects — learning evidence |
| Projects | All ND standalone projects — case studies and builds |

---

## THE PORTFOLIO LAYERS

| Layer | Platform | URL | Purpose |
|---|---|---|---|
| Executive | Website | nikidigitals.com | Professional identity, vision, milestones |
| Thinking | GitBook | nikidigitals.gitbook.io/les | Architecture, research, decisions, journal |
| Evidence | GitHub | github.com/NikiDigitals | Code, infrastructure, version history |
| Professional | LinkedIn — Personal | linkedin.com/in/nmlangendam | Articles, findings, networking |
| Brand | LinkedIn — Company | linkedin.com/company/niki-digitals | NikiDigitals company presence |

**Rule:** Every layer must have at least one exit point to each of the other three layers.

---

## AI INTEGRATION PRINCIPLE — ADR-000097

**Core rule:** AI is integrated into LES only where it demonstrably improves an outcome that matters. Hype, novelty, and industry trend alone are never sufficient justification.

**Build philosophy:**
- LES is built first. AI is added as a top layer over a solid foundation.
- Every AI capability is built at small scale in a LES-LABS sandbox before any industry standard tool is used in production.
- Industry standard tools are used in production where building a custom solution would be wasteful or scope creep.

**Sandbox before production — applied consistently:**

| Capability | Sandbox | Production |
|---|---|---|
| LLM | Train a small model — understand weights, loss, inference | Azure OpenAI Service |
| Agent orchestration | Build from scratch | LangChain / Azure AI Foundry where appropriate |
| Vector search / memory | Build a basic retrieval system manually | Azure AI Search |
| Embeddings | Generate and query manually | Azure OpenAI embeddings |

**Evaluation criteria — all four must be met before integration:**

| Criterion | Question |
|---|---|
| Real value | Does it reduce manual effort, improve decision quality, or enable something previously impossible? |
| Reliability | Is it stable enough for production use? |
| Auditability | Can the output be explained, traced, and audited? |
| Cost justification | Does the benefit outweigh compute cost, maintenance, and complexity? |

**Industry monitoring — quarterly:**
AI developments monitored across four domains — Finance AI, ERP and enterprise systems AI, Agentic systems, Azure AI and OpenAI updates. Sources catalogued in Zotero, synthesised in Obsidian, published in GitBook Research section.

**Documentation:**
- AI industry monitoring → Research layer
- LES AI development → LES-INT and LES-AGT repos + GitBook AI Agents section
- AI sandbox builds → LES-LABS repos + GitBook Labs section

---

## CURRENT PHASE — Phase 0 Closing / Phase 1 Active

**Phase 0 status:** Near complete — target end May 2026
**Phase 1 status:** Active — Day 2

### ✅ What Is Complete

Full log: `LES-Master/_context/LES-TASKS-COMPLETED.md`

- All infrastructure complete — Azure, GitHub, GitBook, website, LinkedIn
- Research stack fully operational — Zotero + Obsidian — collection structure finalised
- Education architecture reviewed and aligned — v1.1 all documents
- Portfolio architecture defined — three project types, GitHub conventions, GitBook sections
- AI Integration Principle established — ADR-000097
- Day 1 study complete — Pre-algebra U1–2, *Code* Ch.1–2, 5 ERP sources added
- GitBook content sessions — sections populated and committed

### ⏳ What Remains Open

| Item | Priority | Notes |
|---|---|---|
| Book ACCA BT exam slot | 🔴 Urgent | First task of Day 2 |
| Write ADR-2026-05-18.md | 🔴 High | Decisions 83–96 |
| Write ADR-2026-05-19.md | 🔴 High | Decisions 97–99 |
| Commit all updated files | 🔴 High | Ready to commit |
| Pre-algebra Units 3 and 4 | 🔴 High | Day 2 study |
| Cadbury Report Literature Note | 🔴 High | Day 2 — Obsidian |
| Begin GitHub Foundations study | 🟡 Medium | Week 3 |
| Write first Insights article | 🟡 Medium | After first learning session |
| Create master architecture diagram | 🟡 Medium | draw.io — C4 Model |

---

## WEBSITE STATUS — nikidigitals.com

**Platform:** WordPress + Astra + Elementor Free | **Status:** ✅ Live

| Page | Status |
|---|---|
| Home | ✅ Live |
| LES — The Project | ✅ Live |
| Portfolio | ✅ Live |
| About | ✅ Live |
| Insights | ✅ Live — first article pending |
| Contact | ✅ Live |

---

## DECISIONS MADE

**Full index:** `LES-Master/docs/decisions/LES-DECISIONS-INDEX.md` — **99 decisions**

| File | Decisions | Status |
|---|---|---|
| ADR-2026-05-12.md | 001–060 | ✅ Written |
| ADR-2026-05-14.md | 061–064 | ✅ Written |
| ADR-2026-05-16.md | 065–066 | ✅ Written |
| ADR-2026-05-17.md | 067–082 | ✅ Written |
| ADR-2026-05-18.md | 083–096 | ⏳ To be written |
| ADR-2026-05-19.md | 097–099 | ⏳ To be written |

---

## RESEARCH STACK — Fully Operational

| Tool | Role | Location |
|---|---|---|
| Zotero 9 | External source management | App + Chrome Connector |
| Better BibTeX | Citation keys — [auth][year] | Zotero plugin |
| Obsidian | Working knowledge layer | `C:\Projects\LES\LES-KNW\vault\` |
| Zotero Integration | Pulls references into Obsidian | Obsidian plugin |
| Templater | Note templates | Obsidian plugin |
| Dataview | Query notes by metadata | Obsidian plugin |

**Citation standard:** Cite Them Right 12th edition — author-date / Harvard

**Zotero collection structure:**

```
My Library
├── 00 — Formal Education
│   ├── OU — all modules
│   └── ACCA — all papers + UoL
├── 01 — Corporate Governance & Compliance
├── 02 — Database Theory & Data Architecture
├── 03 — Enterprise Architecture & ERP
│   ├── Microsoft Dynamics 365
│   └── ServiceNow
├── 04 — Finance & Accounting Theory
├── 05 — AI & Multi-agent Systems
├── 06 — Computer Science Foundations
├── 07 — Research Methodology & Academic Voice
├── 08 — Financial Crime & AML Compliance
├── 09 — Security & GRC
└── 99 — Inbox
```

---

## EDUCATION ARCHITECTURE

**Governing documents:**

| Document | Version | Location |
|---|---|---|
| LES-EDU-ARCH-001.md | 1.1 | LES-EDU/docs/ |
| LES-EDU-ARCH-002.md | 1.1 | LES-Master/_context/ |
| nikidigitals-roadmap.jsx | 2.0 | LES-PORT/website/roadmap/ |

**Y1Q1 active content:**

| Item | Type | Status |
|---|---|---|
| TM112 | Formal — OU | Ongoing |
| ACCA BT | Formal — ACCA | Exam slot not booked — urgent |
| AZ-900 | Certification | Not yet started |
| CS50x | Self-directed | Not yet started |
| Stanford Mathematical Thinking | Self-directed | Not yet started |
| GitHub Foundations | Self-directed | Not yet started |
| Pre-algebra | Self-directed — maths track | Units 1–2 done |
| *Code* — Petzold | Self-directed — CS track | Ch.1–2 done |

---

## LEARNING METHODOLOGY

**Five-step progression — no exceptions:**

| Step | Activity | Tool |
|---|---|---|
| 1 | Study | Microsoft Learn or equivalent |
| 2 | Discuss | LES-LEARN session |
| 3 | Sandbox | LES-LABS repo |
| 4 | Review | LES-LEARN session |
| 5 | Apply | LES module |

**Rule:** No concept implemented in LES until Step 4 is complete.
**Depth standard:** Global expert. No minimum viable answers.

---

## END OF WEEK RITUAL

**Trigger:** "finalise week" in LES-MENTOR.

1. Report all completed tasks
2. Update all three companion files together
3. Write ADR files for the week
4. Write weekly journal entry — LES-JOUR-000[NNN]
5. Decide: GitBook publication for journal?
6. Commit everything
7. Produce Week N+1 LES-MENTOR opening message

---

## MENTOR INSTRUCTIONS FOR CLAUDE

- **Education sessions:** Always request LES-EDU-ARCH-002.md alongside master context
- **Depth standard:** Global expert on all learning questions — no shortcuts
- **Teach** with depth and rigour — the why, not just the what
- **Assume nothing** — every term explained, every step written out
- **Challenge** with questions that deepen understanding
- **Never decide on behalf of the student** — present options, student decides
- **Never produce portfolio content autonomously** — only when explicitly requested
- **Always recommend the best long-term option**
- **Tone** — businesslike and professional. Academic rigour in documentation
- **Documentation briefing on every session close**
- **Three-file update rule** — all three files updated together after every significant session
- **ADR cadence** — one file per day: ADR-YYYY-MM-DD.md
- **Journal cadence** — one entry per week at end of week
- **Step 3 sandbox output** — always a LES-LABS repo, not a throwaway exercise

---

## DOCUMENTATION TRIGGER FRAMEWORK

| Trigger | GitHub | GitBook | Website | LinkedIn |
|---|---|---|---|---|
| Decision made | ADR file | If GitBook: Yes | No | Possibly |
| Concept learned | No | Learning note | No | Possibly |
| Sandbox completed | LES-LABS repo | Labs section | No | Possibly |
| Platform set up | Commit + README | Rationale | No | No |
| Module built | Commit code | Design decisions | No | No |
| Standalone project | ND- repo | Projects section | Portfolio card | Yes |
| Phase completed | Tag release | Retrospective | Update milestones | Yes |
| Certification earned | No | Learning record | If relevant | Yes |
| Research finding | No | Academic entry | No | Condensed — Yes |
| Public milestone | — | — | Major update | Yes |

---

*Last updated: 19 May 2026 — Day 2 morning. Portfolio architecture complete. AI Integration Principle established. 99 decisions recorded.*
