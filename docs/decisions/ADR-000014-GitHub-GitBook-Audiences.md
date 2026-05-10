# ADR-000014 — GitHub and GitBook Serve Different Audiences

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

An earlier decision attempted to eliminate documentation duplication by assigning each document type to a single platform. This created a problem: GitHub visitors — developers and technical evaluators — found no documentation. GitBook visitors — architects and researchers — found documents written for a technical audience rather than a thinking-layer audience.

## Decision

Both GitHub and GitBook contain documentation. They are not copies of each other. The same decision or concept is written in two versions — one for each audience.

| Version | Platform | Audience | Tone |
|---|---|---|---|
| Technical reference | GitHub `docs/` | Developers, engineers | Concise, structured, factual |
| Thinking layer | GitBook | Architects, researchers, serious readers | Narrative, contextual, polished |

**GitHub only — never published to GitBook:**
- `_context/` — master context document
- `TEMPLATE.md` files — scaffolding
- Working drafts — in-progress documents

## Rationale

A developer visiting a GitHub repository expects to find documentation there. Removing it in favour of a GitBook link creates friction and signals that the project is not self-contained. A researcher visiting GitBook expects narrative depth and context — not a technical reference sheet.

The two versions serve the same underlying content to two different audiences in the format each expects.

## Consequences

- Every significant document is written in two versions — GitHub technical and GitBook narrative
- The taxonomy code is the same for both — the platform distinguishes the version
- Internal documents remain GitHub-only — they are never published anywhere
- Writing two versions takes more time but produces a more complete and credible portfolio
