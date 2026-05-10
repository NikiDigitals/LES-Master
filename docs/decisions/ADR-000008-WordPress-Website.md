# ADR-000008 — WordPress for NikiDigitals Website — Initial Version

**Date:** May 2026
**Status:** Accepted
**Decider:** NikiDigitals
**Version:** GitHub — Technical Reference

---

## Context

A professional web presence was required to serve as the executive layer of the four-layer portfolio architecture. The purpose of the site is professional presence — communicating who NikiDigitals is, what LES is, and establishing credibility with a professional audience. A decision was required on the technology stack for this initial version.

Two primary options were considered:

1. Custom-built website using React / Next.js
2. WordPress with a lightweight theme and page builder

---

## Decision

WordPress was selected as the initial website technology, using the Astra theme and Elementor Free page builder.

**Stack:**
- Platform: WordPress (self-hosted)
- Theme: Astra
- Builder: Elementor Free
- Posts widget: Deferred — requires Elementor Pro. Manual placeholders used in the interim.

**Scope:** Content only at this stage. All pages are written as markdown before being entered into WordPress. Design and styling are deferred to a dedicated session once all content is in place.

**Custom build status:** A custom React / Next.js build is preserved as a future standalone project. It is not abandoned — it is appropriately sequenced.

---

## Rationale

The purpose of the site is professional presence, not technical showcase. The technical showcase is GitHub, GitBook, and the LES system itself. Investing significant development time in a custom website at Phase 0, before core LES architecture exists, would be a misallocation of effort.

WordPress allows the executive layer of the portfolio to be established immediately, with minimal technical overhead, while development time is directed toward LES core architecture where it has greater long-term value.

The content-first approach ensures that all pages communicate clearly before visual design is applied. Styling an empty or draft page wastes effort. Writing content in markdown first also means all website content is version-controlled in GitHub regardless of the platform it is published on.

---

## Consequences

- The NikiDigitals website is live and functional at Phase 0
- Elementor Pro features (automated posts widget) are unavailable until a decision is made on upgrading
- All website content exists as markdown in GitHub — platform-independent and portable
- A future migration to a custom-built site is fully supported — content is already structured and version-controlled
- Styling decisions are consolidated into a single dedicated session (LES-WEBSITE-002) rather than applied piecemeal
