# ADR-000004 — Four-Layer Portfolio Architecture

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

LES produces output across multiple dimensions — working system, documentation, professional presence, and published thought leadership. A single platform cannot serve all audiences. A decision was required on how to structure the portfolio.

## Decision

The portfolio operates across four layers, each serving a distinct audience and purpose.

| Layer | Platform | Audience | Purpose |
|---|---|---|---|
| Executive | Website — NikiDigitals | General professional, recruiters | Vision, overview, milestones |
| Thinking | GitBook | Technical, academic, architects | Deep documentation, research, decisions |
| Evidence | GitHub | Developers, engineers | Code, infrastructure, version history |
| Professional | LinkedIn | Professional network | Thought leadership, milestones, networking |

## Rationale

Different audiences arrive with different questions and different tolerances for depth. Separating layers ensures each audience receives the right content in the right format. It also enforces discipline — not everything belongs everywhere.

## Consequences

- Every piece of content is assigned to a layer before it is written
- GitHub and GitBook both contain documentation — different versions for different audiences
- The website is updated rarely — phase completions and major milestones only
- LinkedIn is updated when there is something genuinely worth saying — not on a schedule
- All layers are interconnected — website links to GitBook, LinkedIn links to GitBook entries
