# Success Metrics — Group 1

**Sprint week:** Drafted Week 1, refined Week 2
**Leads:** Md Hossain (UX Research and Validation Lead) and Mirazur Rahman Tonim (Project Lead)
**Source brief:** HiveMind × Ravensbourne brief, Section 5

The brief asked us to define success through prototype-level usability testing rather than launched-product metrics, since the HiveMind MVP is pre-launch. The four metrics below are the targets we set, each one mapped to a hypothesis from `/docs/hypotheses.md` and to the pain points named in the brief.

---

## Our four success metrics

### M1 — Time-to-Task

**Definition:** Reduction in the time it takes a new starter to complete their first independent "daily task" using the roadmap.

**Why this metric:** A "Centralized Task Roadmap" only earns its place if it makes the user faster than their current scattered setup. Speed is the cleanest test of whether structure beats noise.

- **Linked hypothesis:** H1 — Centralized Task Roadmap
- **Linked pain point (from brief):** Cognitive load
- **Tested via:** Task B in `/testing/tasks.md` ("see what to work on today")
- **Target:** Visible reduction in time vs. the participant's self-reported baseline of hunting across multiple tools. We measured this directionally in validation rather than with stopwatch precision (see Limitations below).
- **Mapping to brief:** Aligns with the brief's "Time-on-Task: Reduction in time to locate onboarding materials compared to a baseline scenario."

---

### M2 — Information Retrieval Speed

**Definition:** Can users find a specific policy or template in 3 clicks or less using the Knowledge Hub.

**Why this metric:** Comes directly from the brief ("Can a user find specific 'trapped' knowledge in under 3 clicks?"). It is the single hardest test of whether our Knowledge Hub is solving the fragmentation pain point or just adding another surface.

- **Linked hypothesis:** H3 — Unified Knowledge Hub
- **Linked pain point (from brief):** System fragmentation / no single source of truth
- **Tested via:** Task A in `/testing/tasks.md` ("find a specific document")
- **Target:** ≥ 80% of participants complete the task in ≤ 3 clicks
- **Mapping to brief:** Aligns directly with the brief's "Task Success Rate" criterion.

---

### M3 — Trust Rating

**Definition:** Do users report higher trust in AI assistant answers when a source link to a company PDF (or SOP) is provided?

**Why this metric:** The brief's "Trust Perception" criterion asks whether users understand **why** the AI made a recommendation. We translated that into a comparative trust rating with vs. without source attribution, because trust is invisible unless you ask the user to score it.

- **Linked hypothesis:** H2 — Human-in-the-Loop AI Verification
- **Linked pain point (from brief):** Trust and transparency
- **Tested via:** Task C in `/testing/tasks.md` (Part 2 — AI assistant)
- **Target:** Participant trust rating of ≥ 4/5 when an AI reply visibly cites its sources
- **Result observed in validation:** Arefin rated the AI reply 4/5, the corporate cousin rated it 3/5. Both attributed the score directly to the "cites sources" pattern (see `/testing/session-notes/arefin-call.md`).
- **Mapping to brief:** Aligns with "Trust Perception: Do users understand why the AI Assistant made a recommendation?"

---

### M4 — Onboarding Sentiment

**Definition:** A decrease in the number of new starters who describe their first week as "confused" or "lost" in follow-up surveys.

**Why this metric:** Two of our six interview participants used the words "confused" or "lost" unprompted when describing their own first week (see `/research/synthesis.md`). The brief's "Confidence Score" criterion asks whether users feel "more prepared." We extended that by listening for the negative language we'd actually heard in the field, not just the positive reframing.

- **Linked hypothesis:** H4 — Workspace & Culture Setup Guide
- **Linked pain point (from brief):** Cognitive load + first-time-user-experience
- **Tested via:** Closing question in `/testing/test-script.md` ("On a scale of 1 to 5, how prepared would you feel for your first day at a new company if this was their tool?")
- **Target:** Zero participants describe the prototype-walkthrough experience using the words "confused" or "lost," and ≥ 4/5 average preparedness rating.
- **Mapping to brief:** Aligns with "Confidence Score: Do users report feeling more prepared for their job after going through the Onboarding prototype?"

---

## Summary table

| Metric | Hypothesis | Pain point | Target | How measured |
|---|---|---|---|---|
| **M1** Time-to-Task | H1 | Cognitive load | Reduction vs. self-reported baseline | Task B observation |
| **M2** Information Retrieval Speed | H3 | System fragmentation | ≥ 80% in ≤ 3 clicks | Task A observation |
| **M3** Trust Rating | H2 | Trust in AI | ≥ 4/5 with source citations | Task C, post-task rating |
| **M4** Onboarding Sentiment | H4 | First-week disorientation | No "confused" / "lost"; ≥ 4/5 preparedness | Closing question, listened for verbatim language |

---

## How the metrics were measured in practice

- **Task observation** during the validation call (Arefin Shaon and a corporate cousin) and additional internal team think-aloud sessions. Click counts and time-to-task were logged per task.
- **Verbal trust ratings** were captured at the end of Task C, with reasoning recorded verbatim (see `/testing/session-notes/arefin-call.md`).
- **Closing questions** captured preparedness scores and value-clarity sentences ("In one sentence, what is this product for?").
- **System Usability Scale (SUS)** was prepared as a 10-item questionnaire to be administered at the end of each session, but was not fully administered to every participant in the time available. This is a known limitation, recorded below and in the validation report.

---

## Honest limitations

We are flagging these here rather than burying them, because a marker reading this document deserves to know what the numbers do and do not prove.

1. **Sample size is small.** Two directly observed validation participants plus internal team think-aloud sessions. Findings are directional, not statistically meaningful.
2. **Time-to-Task (M1) was directional, not stopwatch-precise.** The "baseline" was self-reported by participants describing their current tool-switching behaviour, not measured against a controlled comparison flow.
3. **SUS was prepared but not fully administered to every participant.** Future validation rounds should make SUS the first question of the close, not the last, so that overruns don't drop it.
4. **M4 (Onboarding Sentiment) is hard to validate with a prototype walk-through.** It really requires a real first-week experience. The closest we got was listening for verbatim "confused" / "lost" language during the session and capturing the preparedness score. A real measurement of this metric needs HiveMind to run it post-MVP with actual new hires over their first week.

These limitations are deliberately documented so the HiveMind team can plan a more rigorous round of testing post-MVP.
