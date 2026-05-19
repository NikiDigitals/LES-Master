# LES-JOUR-000006 — Week 2 Journal
**Document Code:** LES-JOUR-000006
**Author:** Nicolette Martine Langendam — NikiDigitals
**Week:** Week 2 — 10 to 17 May 2026
**Published:** 19 May 2026
**Location:** LES-Master/journal/
**GitBook:** The Journey → LES-JOUR-000006

---

## Week in Summary

Week 2 was the week the infrastructure became real. Not planned — real. The website went live. The GitBook became a published document. The research stack moved from a configuration task to an operational pipeline. By the end of the week, every layer of the four-layer portfolio architecture had content in it, and the documentation system that will carry this project across five years was running.

It was also the week that produced the most decisions in a single period — 82 decisions recorded by close of week, spanning everything from brand typography to citation key formulae to the depth standard that governs every hour of study in this programme.

---

## What Was Built

### NikiDigitals Website — Live

Six pages built, styled, and published at nikidigitals.com. Home, LES — The Project, Portfolio, About, Insights, and Contact. Full brand system applied — Navy Night, Circuit Blue, Syne Bold headings, DM Sans body. Responsive across desktop, tablet, and mobile. WPForms and WP Mail SMTP configured and confirmed working. Footer cross-links to GitBook, GitHub, and LinkedIn on every page.

The About page includes a full professional experience section — six roles confirmed since October 2025. The Portfolio page uses a three-button card template established as the standard for all future project entries. The Contact page routes to contact@nikidigitals.com via mail.site.eu.

This is the executive layer of the portfolio. It does not go deep — it points to depth. Every page exists to give a visitor one clear next step toward the work that demonstrates the expertise.

### GitBook — Vision & Strategy Fully Populated

The GitBook space went from a skeleton structure to a published knowledge base. The Vision & Strategy section received 19 sub-pages — 11 under Project Plan and 8 under Master Roadmap. The landing page was written and published, leading with the portfolio purpose rather than a project description.

The GitBook is the thinking layer. Where the website gives the what, GitBook gives the why and the how — the architectural reasoning, the decisions, the learning, and the research. Week 2 established the content standard that will govern every entry added across the five-year programme.

### Research Stack — Operational

Zotero 9 and Obsidian were configured and the full pipeline tested in a single session on 17 May 2026.

Zotero manages all external sources — academic papers, reports, books, and primary source documents. Better BibTeX generates stable citation keys using the formula `[auth][year]`. The Chrome Connector captures sources in one click. Citation standard: Cite Them Right 12th edition, author-date (Harvard).

Obsidian is the working knowledge layer. The vault sits at `C:\Projects\LES\LES-KNW\vault\` and is committed to the LES-KNW repository via Git. The methodology is Zettelkasten-light — a seven-folder structure that separates incoming material (Inbox), source interpretations (Literature Notes), synthesised ideas (Permanent Notes), domain hub pages (MOCs), active project working notes (Projects), templates, and archive.

Three community plugins are installed: Zotero Integration (pulls source records directly into Obsidian Literature Notes), Templater (structured note templates), and Dataview (queries the vault as a database by tag, date, or metadata).

The pipeline was tested end-to-end. The Cadbury Report (Committee on the Financial Aspects of Corporate Governance, 1992) was added to Zotero, assigned a citation key, and imported into Obsidian as a Literature Note with bibliographic reference auto-generated. The pipeline works.

### GitHub — 18 Repositories Structured

All 18 repositories created as placeholders, cloned to the local machine, and structured with the universal folder architecture. The GitHub profile README is live with the full NikiDigitals identity and portfolio table. SSH key configured. All repositories pushed.

The universal folder structure — `docs/`, `src/`, `tests/`, `journal/`, `TEMPLATE.md` — is consistent across every repository. Decisions, architecture documents, roadmaps, research notes, and specifications each have a defined home. Nothing will need to be reorganised later because the structure was designed before content was added.

---

## Decisions Made

82 decisions recorded by the close of Week 2, spanning four ADR files:

- **ADR-2026-05-12.md** — decisions 1 to 60 — the founding architecture decisions: cloud platform, repository structure, portfolio layers, brand system, documentation taxonomy, security, GitBook structure, and the operational conventions that govern the project.

- **ADR-2026-05-14.md** — decisions 61 to 64 — diagramming standards (C4, BPMN 2.0, ERD, Azure icons), ADR file convention, and journal cadence.

- **ADR-2026-05-16.md** — decisions 65 and 66 — the learning methodology (five-step: Study, Discuss, Sandbox, Review, Apply) and the depth standard (global expert level, no minimum viable answers).

- **ADR-2026-05-17.md** — decisions 67 to 82 — the full research stack configuration: Obsidian adoption, vault location and methodology, Zotero configuration, citation standard, collection structure, plugin suite, Better BibTeX, Week 1 plan, three-file update rule, and week close automation.

Two decisions from this week deserve specific attention.

**ADR-000065 — Five-Step Learning Methodology.** Every concept studied in this programme follows a defined sequence: Study, Discuss, Sandbox, Review, Apply. No step is skipped. No concept is implemented in LES until Step 4 — Review — is complete. The sandbox (Step 3) produces a committed LES-LABS repository, not a throwaway exercise. This decision defines the rhythm of every future learning session.

**ADR-000066 — Global Expert Depth Standard.** The depth standard for this programme is global expert level. Not exam pass level. Not practitioner level. The deepest possible understanding that exists in each domain — the mathematical derivation before the formula, the legal principle before the rule, the architectural rationale before the implementation pattern. This decision is permanent and applies without exception to every topic, every session, every question.

These two decisions together define what kind of programme this is. They are the answer to the question: what makes LES different from studying for a certification or building a hobby project?

---

## The Research Stack — A Longer Reflection

The research stack deserves more than a task completion entry. Zotero and Obsidian together are not tools for taking notes. They are the infrastructure for building a body of knowledge that compounds over time.

The Zettelkasten methodology — at its core — is the insight that ideas become more valuable when they are connected to each other than when they are isolated in separate documents. A Literature Note on the Zachman Framework for Information Systems Architecture (1987) sitting in isolation is a reference entry. The same note linked to a Permanent Note on enterprise architecture principles, which links to a project note on LES data model design decisions, which connects to a research note on ERP evaluation frameworks — that is a knowledge network. That network, built incrementally over five years, is what produces original research.

The Cadbury Report was the first source to pass through the full pipeline. It is the right starting point. Published in 1992, it established the principles of corporate governance that shaped UK company law and, subsequently, the governance frameworks that now underpin listed company reporting. For a programme whose financial module (LES-FIN) must reflect real-world accounting and governance requirements, and whose research programme will engage with IFRS, AML compliance, and financial crime prevention — understanding where modern governance thinking originated is foundational, not peripheral.

The pipeline worked. The infrastructure is operational. The intellectual work can begin.

---

## What Did Not Get Done

Three items carried from Week 2 into Week 3:

**ACCA BT exam slot not booked.** This is the most important outstanding item in the programme. The ACCA BT examination must be sat before moving to FA. Without a booked slot, the Q1 timeline is at risk. This is the first task of Week 3.

**Master architecture diagram not created.** The C4 Model system diagram that shows LES at the highest level of abstraction — context, containers, and their relationships — has not been started. This is a Phase 0 deliverable. Scheduled for Week 3.

**First Insights article not written.** The nikidigitals.com Insights page is live but empty. The first article needs a subject, a draft, and a publication date. Scheduled for after the first active learning session produces material worth writing about publicly.

---

## Looking Ahead — Week 3

Week 3 is where learning begins in earnest. The infrastructure is complete. The documentation system is running. The research stack is operational. There is nothing left to set up.

The five-step methodology activates this week. Pre-algebra and Charles Petzold's *Code: The Hidden Language of Computer Hardware and Software* are the first two study tracks. The Cadbury Report Literature Note will be written properly — not as a pipeline test, but as a genuine intellectual engagement with the source. The ACCA BT exam slot will be booked. The education architecture will be reviewed and fully aligned across all three governing documents.

The programme is no longer in preparation. It has started.

---

## Week 2 — By the Numbers

| Metric | Count |
|---|---|
| Portfolio layers active | 4 of 4 |
| Website pages live | 6 |
| GitBook sub-pages published | 19 |
| GitHub repositories structured | 18 |
| Decisions recorded | 82 |
| ADR files written | 4 |
| Research sources added to Zotero | 1 |
| Pipeline tests passed | 1 |
| Certifications earned | 0 |
| Articles published | 0 |

The certifications and articles will come. The infrastructure that makes them mean something is already built.

---

*Document Code: LES-JOUR-000006*
*Week: 2 — 10 to 17 May 2026*
*Author: Nicolette Martine Langendam — NikiDigitals*
*Location: LES-Master/journal/LES-JOUR-000006.md*
*GitBook: The Journey → Week 2 Journal*
*Next entry: LES-JOUR-000007 — Week 3 — 18 to 24 May 2026*
