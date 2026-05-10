# LES-GOV-000001 — Session Closing Ritual

**Date:** May 2026
**Status:** Active
**Owner:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Purpose

This document defines the standard closing ritual for every LES working session. The ritual ensures that no work is lost, all decisions are recorded, and the project maintains continuity between sessions regardless of time elapsed.

The ritual takes a maximum of ten minutes. It is not optional.

---

## The Ritual

At the close of every working session, complete the following steps in order:

### Step 1 — Update the Master Context Document
Open the master context document. Update:
- Any tasks completed — mark as ✅ Complete
- Any new decisions made — add to the decisions table with rationale and date
- Any new tasks created — add to the active tasks table
- Open sessions section — update the status of any active chat

### Step 2 — Documentation Check
Review what happened in the session against the GitBook trigger point framework (ADR-011). Identify:
- Does any decision warrant an ADR?
- Does any learning milestone warrant a GitBook entry?
- Does any completion warrant a journal entry?

If yes — write the document now or log it as a task for the next LES-DOCS session.

### Step 3 — Commit to GitHub
Commit all of the following to GitHub before closing:
- Updated master context document → `_context/LES-MASTER-CONTEXT.md`
- Any new documents produced → correct folder per taxonomy (ADR-NNN, LES-ARCH-NNN, etc.)
- Any updated documents

Commit message format: `[Session type] — [brief description of what changed]`

Example: `LES-MENTOR Week 1 — Updated master context, added ADR-007 and ADR-008`

### Step 4 — Write Session Journal Entry
Write 3–5 sentences in the session journal. Location: `journal/LES-JOUR-[NNN]-[brief-title].md`

The journal entry answers three questions:
- What was done or decided in this session?
- What was the most significant moment and why?
- What comes next?

---

## Why This Ritual Exists

Without a closing ritual, work accumulates in chat histories that are not version-controlled, not searchable, and not permanent. Decisions made verbally or in a chat without being committed to GitHub exist only in that chat — which is a temporary workspace, not an archive.

The ritual is also a reflection practice. Writing 3–5 sentences about what happened forces a moment of synthesis that deepens understanding and retention. Over five years, the journal becomes a complete record of the learning journey — an artefact of professional and personal value.

---

## Commit Message Convention

| Session Type | Commit Message Format |
|---|---|
| LES-MENTOR | `LES-MENTOR Week [N] — [description]` |
| LES-SETUP | `LES-SETUP — [description]` |
| LES-LEARN | `LES-LEARN-[topic] — [description]` |
| LES-BUILD | `LES-BUILD-[module] — [description]` |
| LES-DOCS | `LES-DOCS — [description]` |
| LES-WEBSITE | `LES-WEBSITE-[NNN] — [description]` |

---

## Version History

| Version | Date | Changes |
|---|---|---|
| 1.0 | May 2026 | Initial governance document established |
