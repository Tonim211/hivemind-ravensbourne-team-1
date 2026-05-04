# Weekly Log — Group 1, Area A: "Christoph" Dashboard

This log records what we did each week, who did it, and roughly how long it took. Hours include class-dedicated time (4h Wednesdays) plus independent work and team coordination.

**Total target:** 70 hours per person, 16 March – 24 April 2026.

---

## Pre-week (before 16 March)

**Activity:** Reading the brief, project setup document, student handbook and resources pack. Submission of CV and cover letter via Canvas.

| Member | Hours |
|---|---|
| Mirazur Rahman Tonim | 2 |
| Md Hossain | 2 |
| Pranish Shrestha | 2 |
| Ibrahim | 2 |
| Pritesh Kumar Sah | 2 |
| Nakibul Hasan Alif | 2 |

**Notes:** Group allocations published. First contact between team members was patchy — emails went unanswered for the first 48 hours. We did not yet have a working communication channel.

---

## Week 1 — Discovery and hypotheses (16–20 March)

**Goal:** Understand the Christoph persona and pain points; run interviews with working professionals; produce journey map and hypotheses.

### What happened

- **Mon–Tue:** Communication problem identified. As Project Lead, Mirazur asked everyone for WhatsApp numbers and set up a group chat. First Tuesday-evening team call held the same evening: agenda, role check, task split.
- **Wed (class):** Mentor session with Madalina and Andrei. Christoph persona walkthrough, three pain points (cognitive load, system fragmentation, no trusted knowledge source).
- **Wed evening:** Md Hossain drafted six interview questions. Cross-checked in cohort-wide Research and Testing check-in so all six groups asked the same things.
- **Thu–Fri:** Each member ran at least one interview. Six interviews total across retail, hospitality, junior software, NHS admin, accounting, customer service. Transcripts uploaded to `/research/transcripts`.
- **Fri evening:** Synthesis session as a group. Affinity clustering on a Figma board. Four hypotheses written.
- **Sat:** Mirazur set up the GitHub repo and folder structure. First commit of `/docs/research-plan.md`, `/docs/hypotheses.md`, `/docs/success-metrics.md`. Pranish drafted the Current vs Future journey map in Figma.

### Hours

| Member | Hours | Main contribution |
|---|---|---|
| Mirazur Rahman Tonim | 16 | Set up WhatsApp group, ran first Tuesday call, repo and folder setup, conducted 1 interview, liaison emails to HiveMind |
| Md Hossain | 16 | Drafted interview questions, conducted 1 interview, led synthesis session |
| Pranish Shrestha | 16 | Conducted 1 interview, drafted Current vs Future journey map |
| Ibrahim | 16 | Conducted 1 interview, contributed to synthesis |
| Pritesh Kumar Sah | 16 | Conducted 1 interview, early notes on technical feasibility |
| Nakibul Hasan Alif | 16 | Conducted 1 interview, started weekly evidence pack |

**Blockers:** Initial communication. Resolved by setting up the WhatsApp group on the first Wednesday.

**Wins:** Six clean transcripts in the repo before the end of the week. Strong cross-sector spread of interviewees.

---

## Week 2 — Pain points, IA and bento-box wireframes (23–27 March)

**Goal:** Cluster pain points into themes, define the information architecture, produce low-fidelity wireframes.

### What happened

- **Tue evening:** Team call. We talked through the four hypotheses and agreed the five themes that would become the dashboard sections: scattered info, no clear daily priority, no view of teammates, weak announcements, settings buried.
- **Wed (class):** Mentor session with Andrei. Critique of the journey map and hypotheses. Andrei told us our wireframes were "trying to do too much" — we trimmed scope the same week.
- **Wed–Thu:** Pranish drew the IA diagram and sitemap in Figma. Three critical user tasks defined: find a document in under 3 clicks, see what to work on today, know who to ask.
- **Thu–Fri:** Bento-box style low-fidelity wireframes built in Figma. Grey blocks, no colour, no real type. Deliberately rough.
- **Fri:** Wireframes shown to Dr Aruna Duraisingam. Her feedback: "looks too simple — people respond more to prototypes that include diagrams, percentages and progress indicators rather than empty boxes." We logged this in `/docs/decisions.md` and built the response into the Week 3 plan.
- **Sat:** Pritesh ran a technical feasibility review and flagged three things that were not feasible in the project window, including a real-time presence indicator on the directory page. Logged in `/docs/decisions.md`.

### Hours

| Member | Hours | Main contribution |
|---|---|---|
| Mirazur Rahman Tonim | 16 | Tuesday call, scope discussion with mentors, decision logging, liaison emails |
| Md Hossain | 16 | Pain-point clustering, supported task definition |
| Pranish Shrestha | 18 | IA diagram, sitemap, journey map iteration, wireframes |
| Ibrahim | 16 | Wireframe contributions, early UI references |
| Pritesh Kumar Sah | 16 | Technical feasibility review, scope-cut documentation |
| Nakibul Hasan Alif | 14 | Documentation of decisions, evidence pack updates |

**Blockers:** Disagreement between Pranish and Md Hossain on what should sit on the dashboard. Resolved in Tuesday call by going back to interview data, not personal preference.

**Wins:** Aruna's "too simple" feedback, although uncomfortable, gave us the clearest direction for Week 3.

---

## Week 3 — High-fidelity UI, trust patterns, working as one team (30 March – 3 April)

**Goal:** Convert wireframes to high-fidelity screens, build the interactive prototype, address the trust pain point.

### What happened

- **Tue evening:** Team call. Plan agreed: Mirazur leads hi-fi design (strongest Figma background), Ibrahim works alongside on component states and prototype wiring. Everyone else stays on the calls during the work.
- **Wed (class):** Mentor session. Critique on UI and trust patterns. Andrei pushed us on AI transparency.
- **Wed–Sat:** Reference research on Dribbble, Mobbin, Carbon Design System. HiveMind colour palette PDF used as the base. Hexagon visual motif locked in early. GitHub's contribution graph reused as the "Deep work hours" panel.
- **Wed–Sun:** Six core screens designed in high fidelity:
  - Dashboard (welcome, active project, milestone phases, velocity sparkline, upcoming meetings, Knowledge Hub previews)
  - Tasks (4-column kanban with cards)
  - Directory (team cards, hexagonal member avatars)
  - Resources (Knowledge Hub split into SOPs, Fundamentals, Weekly Handbook + AI search bar with "cites sources" label)
  - Announcements (pinned CEO message, comment + RSVP)
  - Settings (profile, working style, role, time zone)
- **Sat–Sun:** Prototype wired up with hover states, kanban column transitions, and a soft fade on the daily standup callout.
- **Mon:** Internal dry-run. One teammate "played" Christoph while the others observed.

### Hours

| Member | Hours | Main contribution |
|---|---|---|
| Mirazur Rahman Tonim | 22 | Reference research, design tokens, all six hi-fi screens, prototype lead |
| Md Hossain | 14 | Microcopy review, AI search "cites sources" pattern, internal dry-run |
| Pranish Shrestha | 16 | IA-to-screen mapping, navigation labels, sitemap-screen alignment |
| Ibrahim | 18 | Component states, prototype wiring, hover and transition logic |
| Pritesh Kumar Sah | 14 | Spacing/alignment QA, technical feasibility check on AI search pattern |
| Nakibul Hasan Alif | 14 | Hi-fi screen exports, evidence pack, design log |

**Blockers:** Hi-fi work took longer than expected. Mirazur went over hours in this week.

**Wins:** Madalina specifically called out our team's communication as the cleanest of the six groups. The "do things together rather than alone" principle from her Week 2 feedback paid off.

---

## Week 4 — Validation, findings, final presentation (6–24 April)

**Goal:** Run usability tests, synthesise findings, write the validation report, present to HiveMind.

### What happened

- **Tue evening:** Team call. Test script reviewed, recruitment finalised.
- **Validation call:** Mirazur set up an hour-long video call with Arefin Shaon (co-founder of BaseTop IT, Bangladesh — the company where Mirazur worked as a Frontend Developer before joining Ravensbourne) and a cousin who works in a corporate office. Mirazur asked Arefin in advance not to be polite.
- **Findings from the validation call (4 specific issues):**
  1. Too many small text labels stacked on top of every information box — eye strain on dark backgrounds.
  2. Right-rail panels (Quick Contacts, focus grid) repeated on every screen even when not relevant — should be removed on inner pages or replaced with something more useful.
  3. Pixel-level alignment off on a couple of information cards — small, but spotted immediately by a trained eye and quietly damages design trust.
  4. Decorative graph sparklines under SOPs and Fundamentals despite those sections being made of text documents with no real data behind them. Mirazur's honest answer when asked why: "I added them because they looked good." Lesson logged: a chart that does not represent real data is decoration pretending to be information.
- **Additional internal think-aloud sessions** on the prototype with the rest of the team observing.
- **Validation report:** Drafted in `/delivery/validation-report.md` with severity ratings and concrete recommendations for HiveMind's MVP.
- **Wed (final class):** Final presentation to Andrei, Madalina and Dr Duraisingam. Each role on the team explained their own contribution. Andrei specifically called out the source-citation pattern on the AI search and the habit of writing scope decisions down.

### Hours

| Member | Hours | Main contribution |
|---|---|---|
| Mirazur Rahman Tonim | 16 | Validation call with Arefin and cousin, validation report, presentation deck, two rehearsals |
| Md Hossain | 16 | Test script, internal think-aloud sessions, findings synthesis |
| Pranish Shrestha | 16 | Recommendations on IA fixes, presentation slides |
| Ibrahim | 16 | Prototype fixes after validation, presentation demo |
| Pritesh Kumar Sah | 16 | Severity ratings, technical recommendations in validation report |
| Nakibul Hasan Alif | 18 | Validation report write-up, evidence pack finalisation, presentation deck |

**Blockers:** Recruiting working professionals on short notice — same issue several other groups raised in the cross-group check-in.

**Wins:** Arefin's bold and honest feedback genuinely changed the final design. The sparkline lesson is the one we will all remember.

---

## Total hours summary

| Member | Pre | Wk 1 | Wk 2 | Wk 3 | Wk 4 | **Total** |
|---|---|---|---|---|---|---|
| Mirazur Rahman Tonim | 2 | 16 | 16 | 22 | 16 | **72** |
| Md Hossain | 2 | 16 | 16 | 14 | 16 | **64** |
| Pranish Shrestha | 2 | 16 | 18 | 16 | 16 | **68** |
| Ibrahim | 2 | 16 | 16 | 18 | 16 | **68** |
| Pritesh Kumar Sah | 2 | 16 | 16 | 14 | 16 | **64** |
| Nakibul Hasan Alif | 2 | 16 | 14 | 14 | 18 | **64** |

> Class-dedicated hours per member: 4h × 4 weeks = **16h**. Remaining hours are independent and team-coordination work.

---

## Sign-off

This log was maintained throughout the sprint and reviewed by the full team before final submission. For role-by-role reflections see each member's individual WBL report.
