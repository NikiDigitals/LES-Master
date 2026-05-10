# ADR-000011 — GitBook Documentation Trigger Points

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

GitBook serves as the thinking layer of the portfolio — the place where architectural reasoning, learning depth, and research are documented at a level of rigour appropriate for a technical and academic audience. A decision was required on when GitBook entries are created to ensure quality is maintained and documentation effort is focused where it adds genuine value.

---

## Decision

GitBook entries are created at defined trigger points only. Not every session produces a GitBook entry.

**Trigger points that warrant a GitBook entry:**

| Trigger | Entry Type | Example |
|---|---|---|
| A significant architectural decision is made | ADR | Repository architecture, portfolio structure |
| A concept is deeply understood through study | Learning note | Cloud fundamentals, data modelling principles |
| A module or feature is completed | Completion record | LES-FIN data model finalised |
| A phase is completed | Phase retrospective | Phase 0 — Foundation complete |
| A research finding of substance is produced | Research note | Academic literature on personal informatics |
| A governance framework is established | Governance document | Session closing ritual, documentation standards |

**Trigger points that do not warrant a GitBook entry:**

- Routine session progress updates
- Minor task completions
- Administrative changes to the master context
- Work in progress without a concluded finding or decision

---

## Rationale

Documentation quality degrades when volume is prioritised over substance. A GitBook that contains fifty entries of varying depth is less credible than one that contains twenty entries of consistent rigour. Every GitBook entry should be worth reading independently by a technical professional who has no other context about the project.

The trigger point framework also protects time. Documentation is not the work — it records and communicates the work. The ratio of doing to documenting should remain high, particularly in the early phases when infrastructure and foundation are the priority.

---

## Consequences

- Not every session produces a GitBook entry — this is by design
- Entries that are written must meet the standard of the thinking layer — rigorous, considered, and readable by a technical audience
- The session closing ritual includes a documentation check that identifies whether a trigger point was reached
- Over time, the GitBook builds into a coherent body of work rather than a log of activity
