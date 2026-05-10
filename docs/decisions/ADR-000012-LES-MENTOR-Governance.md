# ADR-000012 — LES-MENTOR as Home Base Chat Type

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

The LES project uses Claude as a mentor, teacher, and technical guide. Sessions occur across multiple chat types — learning, building, documentation, setup. A decision was required on how to manage continuity across sessions given that Claude has no persistent memory between conversations without explicit context provided.

---

## Decision

`LES-MENTOR` is established as the home base chat type. A new LES-MENTOR chat is opened once per week following this convention:

**Naming:** `LES-MENTOR — Week [N] — [Month Year]`

**Opening:** The full master context document is pasted at the start of every LES-MENTOR chat.

**Purpose:** Report back on work completed during the week, update the master context document, run the documentation check, and receive the next assigned step.

**Cycle:**
1. Open new LES-MENTOR chat with updated master context
2. Report back on completed work
3. Documentation check — identify what needs to be committed to GitHub or written for GitBook
4. Master context updated
5. Next step assigned
6. Session closing ritual completed — master context committed to GitHub, journal entry written

**Rule:** One LES-MENTOR chat per week. Chats are not carried over. If it is not committed to GitHub, it did not happen.

---

## Rationale

Claude's lack of persistent memory between conversations is a constraint that must be managed architecturally, not worked around informally. The LES-MENTOR structure treats the master context document as the memory layer — it is maintained in GitHub and pasted at the start of every session, giving Claude full project context regardless of when the chat was opened.

The weekly cadence provides accountability without rigidity. Progress is reviewed, decisions are captured, and the next step is always clear. This mirrors how a real project management cadence works — regular check-ins, documented outputs, clear next actions.

---

## Consequences

- Every week begins with an updated master context committed to GitHub
- No project knowledge exists only in a chat — everything is externalised to GitHub
- The LES-MENTOR chat serves as a project management layer, not a technical working session
- Specific technical work happens in dedicated chat types (LES-SETUP, LES-LEARN, LES-BUILD) and is reported back through LES-MENTOR
