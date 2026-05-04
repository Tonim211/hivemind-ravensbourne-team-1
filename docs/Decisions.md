# Decisions Log — Group 1

A running record of scope changes, design decisions, and trade-offs made during the sprint. Logged in date order within two sections: foundational design inclusions (what we deliberately built **in** and why), and process / scope decisions made over the four weeks.

---

## Foundational design inclusions

These four were the load-bearing design decisions of the prototype. Each one is traceable to a pain point named in the HiveMind brief and to a hypothesis in `/docs/hypotheses.md`.

### D0.1 — Verified Knowledge Hub

**Decision:** Include a Knowledge Hub as a top-level section, split into SOPs, Fundamentals and the Weekly Handbook, with each item carrying a version tag (e.g. "V2.4") and a "Verified" badge.

**Reason:** Solves the **Information Fragmentation** pain point by providing a central location for SOPs, company-DNA documents and what-changed-this-week updates. Removes the user's question of "is this the current version?" by making version state visible.

- **Linked hypothesis:** H3 — Unified Knowledge Hub
- **Linked screen:** Resources
- **Validation outcome:** Supported in Week 4. The versioned and verified content was instantly understood by both validation participants. Caveat: decorative sparklines beneath the section cards were flagged for removal (see D15).

### D0.2 — Resource Signposting

**Decision:** Treat the dashboard as a launchpad to external tools rather than trying to replace them. The Knowledge Hub previews on the Dashboard home, and the Resources page itself, are designed to point users into the right system rather than re-host every document.

**Reason:** Bridges the **Integration Gap** for employees who use 20+ tools day-to-day. New joiners do not need another silo. They need a signpost that tells them where the canonical version of a thing lives.

- **Linked hypothesis:** H3 — Unified Knowledge Hub (extends it)
- **Linked screen:** Dashboard (Knowledge Hub previews), Resources
- **Validation outcome:** Implicitly supported. No participant asked "but where is the actual document?" — the signposting model was understood without explanation.

### D0.3 — HiveMind AI Assistant

**Decision:** Include an AI assistant on the Resources page that supports natural-language queries ("Ask hive…") and returns answers with visible source citations linking back to the underlying SOP or Fundamentals document.

**Reason:** Addresses user demands for **transparency and accuracy** in AI tools. Uses two specific patterns: natural-language query (so users don't have to learn a search syntax) and cited answers (so users can verify the reply rather than trust a black box).

- **Linked hypothesis:** H2 — Human-in-the-Loop AI Verification
- **Linked screen:** Resources (inline AI search bar)
- **Validation outcome:** Strongest validation signal of any single design choice. Arefin rated AI trust 4/5 specifically because of the "cites sources" pattern. Andrei called it out positively in the Week 4 mentor session.

### D0.4 — Unified Task View

**Decision:** Consolidate onboarding tasks and day-to-day work into a single Tasks surface (4-column kanban: To do, In progress, Review, Done), with the Dashboard home surfacing the most urgent items via the "Up Next" panel and the active project card.

**Reason:** Reduces the **cognitive burden of context switching** by removing the artificial separation between "onboarding tasks" and "real work." For a new joiner, those are the same thing. Splitting them across two surfaces would force the user to remember which list a piece of work belongs on.

- **Linked hypothesis:** H1 — Centralized Task Roadmap
- **Linked screen:** Dashboard (home), Tasks
- **Validation outcome:** Supported. The Dashboard + Tasks pairing conveyed daily priority within the 30-second value-clarity target. Caveat: information density was flagged as too high in places (finding F7 in the validation report).

---

## Process and scope decisions

The decisions below are the running log of process choices, scope cuts and refinements made across the four-week sprint.

## D1 — WhatsApp group as primary internal channel

**Date:** Week 1, Wednesday 18 March 2026
**Made by:** Mirazur Rahman Tonim (Project Lead)
**Reason:** Email coordination broke down in the first 48 hours after group allocation. Two unanswered emails, no central thread. WhatsApp gave us a single visible channel for day-to-day coordination while keeping email reserved for HiveMind liaison.
**Result:** Communication was rated cleanest of the six groups by Madalina in Week 3.

## D2 — Tuesday-evening team call as a weekly fixture

**Date:** Week 1
**Made by:** Mirazur Rahman Tonim
**Reason:** Wednesday-only contact wasn't enough to plan a sprint. Each Tuesday call: review last week, agree what was needed for Wednesday, split tasks.
**Result:** Saved the most time of any single habit across the sprint.

## D3 — All groups use the same interview questions

**Date:** Week 1
**Made by:** Cohort-wide Research and Testing check-in
**Reason:** Per the student handbook, this lets findings be compared across the six groups. Md Hossain drafted ours, the cohort cross-checked.
**Result:** 6 transcripts in `/research/transcripts`; cross-group themes emerged.

## D4 — Five dashboard sections derived from interview themes, not from competitor products

**Date:** Week 2, Tuesday call
**Made by:** Pranish Shrestha (UX/IA), Mirazur, full team
**Reason:** We deliberately did not start by sketching another Slack-or-Notion dashboard. The five themes came from affinity-clustering the interview pain points (see `/research/synthesis.md`).
**Result:** Tasks, Directory, Resources, Announcements, Settings — five sections, traceable to research.

## D5 — Real-time presence indicators on the Directory: cut

**Date:** Week 2, Friday
**Made by:** Pritesh Kumar Sah (Technical Feasibility & QA Lead)
**Reason:** Real-time presence requires a backend connection (websocket / pub-sub) we cannot validate in the project window. Static "active recently" badges considered as a fallback but also cut for time.
**Status:** Cut. Recommended for HiveMind's MVP backlog.

## D6 — Inbox / DM surface: cut

**Date:** Week 2
**Made by:** Full team
**Reason:** Direct messaging would compete with Slack rather than complement it. Out of scope for a 4-week sprint.
**Status:** Cut. Not recommended for MVP — would dilute the product's positioning.

## D7 — Full calendar view: cut

**Date:** Week 2
**Made by:** Full team
**Reason:** The "Up Next" panel on the right rail covers the daily need. A full calendar is post-MVP territory.
**Status:** Cut. Recommended for HiveMind's post-MVP roadmap.

## D8 — Goals / OKR surface: cut

**Date:** Week 2
**Made by:** Full team
**Reason:** Considered as a fifth pillar of the IA. Cut after debate because it would explode the surface area and dilute focus on onboarding.
**Status:** Cut. Optional Phase 2.

## D9 — Per-team workspaces: cut

**Date:** Week 2
**Made by:** Full team
**Reason:** Would multiply the IA by team count and turn the product into a different category (workspace tool, not onboarding tool).
**Status:** Cut. Out of scope.

## D10 — Wireframe is bento-box style, deliberately rough

**Date:** Week 2
**Made by:** Pranish Shrestha, full team
**Reason:** Per Andrei's mentor advice, low-fi wireframes should be ugly on purpose so feedback focuses on structure, not visuals.
**Result:** Aruna's "looks too simple" feedback (logged below) was the right kind of feedback for the right stage.

## D11 — Information density increased in high-fidelity (response to Aruna's feedback)

**Date:** Week 3
**Made by:** Mirazur, Ibrahim, full team
**Reason:** Aruna's Week 2 critique that the bento wireframe looked too simple shaped the entire Week 3 plan. The high-fi screens added progress percentages, milestone phase indicators, a velocity sparkline, and focus and task counters.
**Result:** Validation in Week 4 confirmed the direction was right but flagged that density had gone too far in places (see F7, F10 in the validation report).

## D12 — Hexagon as the visual motif

**Date:** Week 3
**Made by:** Mirazur
**Reason:** The company is HiveMind. The hexagon is on-brand, repeats easily across avatars, status pills and category icons, and gives the design a single visual signature.
**Result:** Validated positively by Arefin: "branded without being heavy-handed."

## D13 — GitHub contribution graph reused as Deep Work Hours panel

**Date:** Week 3
**Made by:** Mirazur, Ibrahim
**Reason:** The grid pattern is instantly familiar to developers (and Christoph is a developer persona). Reusing it gave the dashboard one more piece of personality without inventing a new visual language.
**Result:** Liked by validation participants.

## D14 — AI search "cites sources" pattern

**Date:** Week 3
**Made by:** Md Hossain, Mirazur
**Reason:** Directly addresses the trust pain point in the brief. Came out of one interviewee's quote that an AI tool at work had "made things up."
**Result:** Specifically called out positively by Andrei in the Week 4 mentor session, and by Arefin in validation.

## D15 — Decorative sparklines under SOPs / Fundamentals: kept in prototype, flagged as defect, recommended to remove for MVP

**Date:** Week 3 (added) → Week 4 (flagged)
**Made by:** Mirazur (added), Arefin (flagged in validation)
**Reason kept in prototype:** Honestly, they looked good.
**Reason flagged for MVP:** Charts that don't represent real data are decoration pretending to be information. On a product trying to build user trust, this is exactly the wrong move.
**Status:** Kept in prototype as historical record. Recommendation R2 in the validation report says remove for MVP.

## D16 — Final presentation deck: not produced

**Date:** Week 4
**Reason:** Time constraints and prioritisation of the validation report and prototype refinements over the deck.
**Status:** Acknowledged. The validation report (`/delivery/validation-report.md`) and the README are the standalone-readable deliverables.
