# ADR-000013 — GitHub as Single Source of Truth

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

The LES project produces documentation across multiple platforms — Claude chats, GitBook, a WordPress website, and LinkedIn. A decision was required on which platform holds the authoritative version of all project documents and serves as the permanent record of the project.

---

## Decision

GitHub is the single source of truth for all LES project documents.

**Implications:**
- Every document produced in a Claude chat must be committed to GitHub before the chat is closed
- GitBook syncs from GitHub — never written directly in GitBook
- Website content is written as markdown and committed to GitHub before being entered into WordPress
- LinkedIn articles are published on LinkedIn but the source markdown is committed to GitHub
- Claude chats are temporary workspaces — they are not archives

**The governing principle:** If it is not in GitHub, it did not happen.

---

## Rationale

Claude has no persistent memory between conversations. Chat histories are not searchable, not version-controlled, and not guaranteed to be accessible long-term. Any document that exists only in a Claude chat is at risk of being lost.

GitHub provides version control, a full history of every change, a public-facing record of progress, and a platform-independent storage layer that is not dependent on any single tool or service remaining available.

GitBook syncing from GitHub — rather than being written directly — ensures that the GitBook content is always a reflection of the GitHub content, never ahead of it. This eliminates the risk of content drift between platforms.

---

## Consequences

- Every session that produces a document ends with a GitHub commit — no exceptions
- The session closing ritual includes committing the updated master context and any new documents
- GitBook is a publishing layer, not an authoring layer
- If a tool or platform becomes unavailable, the full project record exists in GitHub independently
- The GitHub commit history becomes a timestamped record of the entire project journey — an artefact of value in its own right
