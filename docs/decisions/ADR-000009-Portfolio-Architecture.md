# ADR-000009 — Four-Layer Portfolio Architecture

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

LES is simultaneously a working system, a learning journey, a body of published work, and a career development instrument. A single platform cannot serve all of these purposes for different audiences with different expectations. A decision was required on how to structure the portfolio across multiple platforms in a way that is coherent, maintainable, and professionally credible.

---

## Decision

The portfolio is structured across four distinct layers, each serving a specific audience and purpose.

| Layer | Platform | Audience | Purpose | Tone |
|---|---|---|---|---|
| Executive | Website (NikiDigitals) | General professional, recruiters, collaborators | High-level narrative — who, what, why | Confident, visionary, accessible |
| Thinking | GitBook | Technical professionals, researchers, architects | Deep documentation — decisions, architecture, research, learning | Academic, rigorous, precise |
| Evidence | GitHub | Developers, engineers, technical evaluators | Working proof — code, infrastructure, version history | Technical, structured, well-commented |
| Professional | LinkedIn | Professional network, industry peers, academic community | Thought leadership, milestone announcements, networking | Professional, insightful, authoritative |

---

## Rationale

Different audiences arrive with different questions. A recruiter visiting a GitHub repository without context gains nothing. A developer visiting a personal website without technical depth gains nothing. Separating the layers ensures each audience receives the right level of detail in the right format without compromise.

The four-layer structure also enforces discipline in how content is produced. Not everything belongs everywhere. A learning note belongs in GitBook. A phase completion belongs on LinkedIn. Code belongs on GitHub. The website communicates the vision, not the detail.

GitBook entries are created at defined trigger points only — decisions, deep learning milestones, and phase completions. This prevents dilution of documentation quality and ensures every GitBook entry carries genuine intellectual weight.

---

## Consequences

- Every piece of content produced must be assigned to the correct layer before it is written
- Cross-posting is deliberate and infrequent — LinkedIn articles are condensed versions of GitBook entries, not duplicates
- The website is updated rarely — only when there is something worth showing to someone who knows nothing about the project
- GitHub is updated frequently — every session that produces a document, decision, or code produces a commit
- All layers are connected: the website links to GitBook and GitHub, LinkedIn articles link back to GitBook entries
