# Hypotheses — Group 1

**Format:** *We believe that [solution] will help [user] because [reason from research].*
**Source:** Synthesised from 6 interviews with working professionals. See `/research/synthesis.md` and `/research/transcripts/`.
**Sprint week:** Written end of Week 1 (20 March 2026)

These are the four testable hypotheses that drove our high-fidelity prototype. Each one is mapped to the pain point it addresses, the screen(s) that operationalise it, and the validation signal from the interviews.

---

## H1 — Centralized Task Roadmap

**We believe that** a modular onboarding journey with a clear "what to do next" workflow
**will help new starters**
**because** we heard they specifically miss having a "list of pending tasks" and feel lost during their first week.

- **Pain point addressed:** No clear daily priority. New joiners drift between tools without a structured next step.
- **Tested via screens:** Dashboard (home) — active project card with milestone phase indicator (e.g. "Phase 3 of 5") and Up Next panel. Tasks — 4-column kanban with task counts per column.
- **Validation signal from research:** Multiple interviewees described the absence of a pending-task list. "I open my laptop and I don't know what's first" came up repeatedly.

---

## H2 — Human-in-the-Loop AI Verification

**We believe that** adding source citations and "human-review" flags to AI answers
**will help working professionals trust the system**
**because** participants believe a human must still be the judge of whether AI-generated facts are reliable.

- **Pain point addressed:** Trust in AI tools. Users will not act on a black-box answer.
- **Tested via screens:** Resources page — AI search bar ("Ask hive") with a visible "cites sources" label on every reply, and click-through to the underlying SOP / Fundamentals document.
- **Validation signal from research:** One interviewee said they had stopped trusting an AI tool at work because, in their words, "it just made things up." A second participant added that AI answers should always be verifiable by a person before being acted on.
- **Note:** This was the strongest validated hypothesis in the Week 4 validation call. Both Arefin Shaon and the corporate cousin specifically called out the source-citation pattern as the right move (see `/delivery/validation-report.md`, finding F4).

---

## H3 — Unified Knowledge Hub

**We believe that** a single "Information Hub" for all company rules, guides and SOPs
**will help employees**
**because** they currently waste time "switching between tools" and managing fragmented information across multiple platforms.

- **Pain point addressed:** System fragmentation. Knowledge currently lives across Slack, Drive, Notion and email with no version awareness.
- **Tested via screens:** Resources — Knowledge Hub split into three categories (SOPs, Fundamentals, Weekly Handbook), each item carrying a version number (e.g. "V2.4") and a "Verified" badge to remove the "is this the current one?" ambiguity.
- **Validation signal from research:** "I can never find anything" appeared in 4 of 6 transcripts in some form. Multiple participants described the cost of bouncing between platforms looking for the same piece of information.

---

## H4 — Workspace & Culture Setup Guide

**We believe that** a digital guide with automated setup checklists
**will help new employees**
**because** we heard they currently feel "confused" and "lost" due to a lack of clear instructions on how to set up their workspace and environment.

- **Pain point addressed:** Lack of structured first-day setup. New joiners are expected to figure out tooling, accounts and culture without a guided path.
- **Tested via screens:** Dashboard (home) — onboarding day count in the header ("Day 8 of 14"), role-aware project card. Settings — profile, working style, time zone, connected tools, AI preferences. Resources — Fundamentals section ("Company DNA") for culture and how-we-work documents.
- **Validation signal from research:** Participants used the words "confused" and "lost" specifically when describing their first week. Two said they had wanted to ask basic setup questions but did not, for fear of looking stupid.

---

## How these hypotheses were tested

Each hypothesis was operationalised in the high-fidelity prototype and stress-tested in the Week 4 validation call (see `/delivery/validation-report.md`).

| Hypothesis | Validation outcome |
|---|---|
| **H1 — Centralized Task Roadmap** | Supported. The Dashboard home + Tasks kanban combination conveyed daily priority within the 30-second value-clarity target. Caveat: information density was flagged as too high (finding F7). |
| **H2 — Human-in-the-Loop AI Verification** | Strongly supported. The "cites sources" pattern received the clearest positive feedback of any single design choice. Both validation participants rated AI trust higher because of it. |
| **H3 — Unified Knowledge Hub** | Supported. Versioned and verified content was instantly understood. Caveat: decorative sparklines under SOPs and Fundamentals were flagged as "decoration pretending to be information" (finding F10) and recommended for removal. |
| **H4 — Workspace & Culture Setup Guide** | Partially tested. The Settings sub-nav and Day-of-onboarding header were liked, but a full "checklist" surface for workspace setup was not built into the prototype within the four-week window. Recommended for HiveMind's MVP backlog. |

---

## Honest note on H4

H4 was the hypothesis we did **least** justice to in the prototype. The brief gave us a four-week window and we prioritised H1, H2 and H3, which were all directly addressable through screens we already had in scope. H4 implies a dedicated checklist or wizard surface ("Day 1: connect Slack ✓ · Day 2: set up dev env · Day 3: meet your pod") that would have required either a new screen or a significant expansion of Settings. Logged in `/docs/decisions.md` as a candidate for the MVP backlog rather than something we validated.
