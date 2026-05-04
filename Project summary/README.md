# HiveMind × Ravensbourne — Group 1 (Area A: "Christoph" Dashboard)

> Work-Based Learning sprint, 16 March – 24 April 2026
> Ravensbourne University London × HiveMind Academy

This repository is the evidence pack for **Group 1's** four-week Product Discovery sprint with HiveMind Academy. We were assigned **Area A — the "Christoph" Dashboard**: designing a unified, role-aware dashboard that reduces cognitive load and stops new joiners from hunting for company information across Slack, Drive and Notion.

---

## The team

| Role | Name |
|---|---|
| Project Lead / Client Communications | Mirazur Rahman Tonim |
| UX Research & Validation Lead | Md Hossain |
| UX / IA Designer | Pranish Shrestha |
| UI / Prototype Designer | Ibrahim |
| Technical Feasibility & QA Lead | Pritesh Kumar Sah |
| Documentation Lead | Nakibul Hasan Alif |

**Liaison for HiveMind:** Mirazur Rahman Tonim
**Mentors at HiveMind:** Andrei Tapurin, Madalina Mihailescu
**Module lead:** Dr Aruna Duraisingam

---

## The problem we were asked to solve

Christoph is HiveMind's persona for a new engineering hire in his first two weeks at a new company. He is dealing with three pain points the brief asked us to validate:

1. **Cognitive load** — too much information thrown at him at once
2. **System fragmentation** — onboarding info scattered across Slack, Drive, Notion and email
3. **No single trustworthy place for company knowledge**

Our job was to act as a Product Discovery Squad: research the pain points with real working professionals, design a high-fidelity prototype, validate it, and write up findings that could feed into HiveMind's MVP roadmap.

---

## What we built

A six-screen high-fidelity Figma prototype of the "Christoph" Dashboard:

- **Dashboard (home)** — welcome header, active project card with progress %, milestone phase indicator, velocity sparkline, upcoming meetings, Knowledge Hub previews
- **Tasks** — four-column kanban (To do, In progress, Review, Done) with task cards
- **Directory** — team cards with member hexagons, role tags, and quick-open actions
- **Resources** — Knowledge Hub split into SOPs, Fundamentals and Weekly Handbook, with an inline AI search that **cites its sources**
- **Announcements** — pinned company-wide messages (e.g. CEO updates) with comment and RSVP
- **Settings** — profile, working style, role, time zone

**Visual motif:** the hexagon, because the company is HiveMind. Avatars, status pills and category icons are all hexagonal.

**Inspirations:** Carbon Design System (layout, components), Dribbble and Mobbin (dark-mode dashboards), and GitHub's contribution graph (reused as the "Deep work hours" panel on the right rail).

---

## What we found in research

- 6 interviews with working professionals across retail, hospitality, junior software, NHS admin, accounting and customer service
- "I can never find anything" appeared in 4 of 6 transcripts in some form
- Two participants said they had stopped asking questions in their first month because they didn't want to look stupid
- Strongest hypothesis: a single, role-aware dashboard reduces time-to-find for onboarding documents because it removes the need to switch between Slack, Drive and Notion

Full transcripts: [`/research/transcripts`](./research/transcripts)

---

## What validation told us

We ran a deep validation call with **Arefin Shaon** (co-founder of BaseTop IT, Bangladesh) and a cousin who works in a corporate office. We also ran additional internal think-aloud sessions on the prototype.

The four sharpest pieces of feedback we acted on:

1. **Too many small text labels** stacked on every information card — eye strain on dark backgrounds
2. **Right-rail panels (Quick Contacts, focus grid) repeated on every screen** even when not relevant — wasted real estate
3. **Pixel-level alignment issues** on a couple of cards — small, but visibly damages design trust
4. **Decorative graph sparklines under SOPs / Fundamentals** that did not represent real data — decoration pretending to be information

Full write-up with severity ratings and recommendations: [`/delivery/validation-report.md`](./delivery/validation-report.md)

---

## Repository structurehivemind-ravensbourne-team-1/
├── README.md
├── weekly-log.md
├── docs/
│   ├── research-plan.md
│   ├── hypotheses.md
│   ├── success-metrics.md
│   └── decisions.md
├── research/
│   └── transcripts/        (6 interview transcripts)
├── design/
│   ├── journey-maps/
│   ├── ia-sitemap/
│   ├── wireframes/         (bento-box low-fidelity)
│   └── hi-fi-screens/      (6 screens, PNG exports)
├── testing/
│   ├── tasks.md
│   ├── test-script.md
│   └── session-notes/
└── delivery/
├── validation-report.md
└── final-presentation.pdf

---

## How we worked

- **Tuesday-evening team call (every week)** to review the previous week, agree what was needed, and split the tasks
- **Wednesday class session (4 hours)** with Andrei and Madalina from HiveMind
- **WhatsApp group** for day-to-day coordination
- **Single liaison** (Mirazur) consolidated questions to HiveMind into one weekly email per the project setup document
- **Worked together rather than alone** — even when one person led a piece, two or three of us would sit on the call while it was being made

Madalina specifically called out our communication as the cleanest of the six groups in Week 3.

---

## Tools

- **Figma** — research board, IA, wireframes, hi-fi screens, prototype
- **GitHub** — this repo, evidence pack
- **WhatsApp** — internal coordination
- **Email** — official channel with HiveMind
- **Carbon Design System** — component reference

---

## Links
- 🎨 **Figma prototype:** https://www.figma.com/design/AihgLBor13wrL6hCALjg16/Hivemind-Final-Dashboard?node-id=0-1
- 📝 **Validation report:** [`/delivery/validation-report.md`](./delivery/validation-report.md)
- 🌐 **HiveMind Academy:** https://www.hivemindacademy.com
---

## Acknowledgements

Huge thanks to **Andrei Tapurin** and **Madalina Mihailescu** at HiveMind Academy for the brief, the weekly mentor sessions, and honest feedback throughout the sprint. Thanks to **Dr Aruna Duraisingam** for the module lead and the Week 2 wireframe critique. And thanks to **Arefin Shaon** at BaseTop IT for the bold and honest validation call that genuinely changed our final design.

