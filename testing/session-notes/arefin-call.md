# Session Notes — Validation Call

**Date:** Week 4 (April 2026)
**Format:** Video call, ~60 minutes
**Moderator:** Mirazur Rahman Tonim (Project Lead)
**Notetaker:** Md Hossain (UX Research and Validation Lead) — notes consolidated within 24 hours
**Prototype version shown:** Final Figma high-fidelity build (https://www.figma.com/design/AihgLBor13wrL6hCALjg16/Hivemind-Final-Dashboard)

---

## Participants

**P1 — Arefin Shaon**
- Role: Co-founder, BaseTop IT (Bangladesh)
- Relevance: Senior practitioner with years of experience hiring and onboarding designers and engineers. Mirazur previously worked at BaseTop IT as a Frontend Developer, which is how the contact was established. Asked in advance to be blunt rather than polite.

**P2 — Corporate cousin**
- Role: Office worker in a corporate environment (sector withheld for anonymity)
- Relevance: Working professional in the target audience the brief specified.

---

## Format

The session was structured in three parts:
1. Walk-through of the prototype with think-aloud commentary
2. Open feedback discussion
3. Specific probes on AI trust and information density

This was a richer format than a strict task-based test because the goal was to surface design issues a senior practitioner would spot, not just task success rates.

---

## Findings (the four called out by Arefin)

These map directly to F7–F10 in `/delivery/validation-report.md`.

### Finding 1 — Too many small text labels (Severity: High)

**Quote (Arefin, paraphrased):** "Every card has three or four tiny labels stacked at the top. After two minutes my eyes hurt. On a dark background it's worse."

**What he was looking at:** Dashboard home, Resources, Tasks card metadata.
**Recommendation logged:** Reduce stacked metadata. One primary line, hover or click-to-expand for secondary detail. (R1 in validation report.)

### Finding 2 — Right-rail panels repeat unnecessarily (Severity: Medium)

**Quote (Arefin, paraphrased):** "I get why Quick Contacts is on the home screen. Why is it on Settings? Why is it on Resources? It's the same panel six times."

**What he was looking at:** Right-rail panels (Quick Contacts, Deep Work Hours, Up Next) appearing on every screen.
**Recommendation logged:** Make the right rail context-aware. Different panels per screen, or remove on inner pages. (R4.)

### Finding 3 — Pixel-level alignment off on a couple of cards (Severity: Medium)

**Quote (Arefin, paraphrased):** "Look at this card. The title is two pixels lower than the title on the card next to it. A user might not say the word 'misalignment' but they'll feel that the design is sloppy and they'll trust it less."

**What he was looking at:** Card grid on the Dashboard home, specifically the stats row.
**Recommendation logged:** Full alignment QA pass before MVP. Snap to grid. (R5.)

### Finding 4 — Decorative sparklines under SOPs / Fundamentals (Severity: High)

**Quote (Arefin, paraphrased):** "Why is there a graph under SOPs? What data is that? Tell me what those squiggles represent."

**Mirazur's reply (recorded honestly):** "I added them because they looked good."

**Arefin's response (paraphrased):** "Right, but on a product whose entire job is to be a single source of truth, decoration that looks like data is the worst kind of trust break. People will think it means something. When they realise it doesn't, they'll trust the rest of the product less."

**Recommendation logged:** Remove decorative sparklines. Replace with plain-text metadata where useful (e.g. "12 docs · 5d ago"). (R2.)

This was the single most useful piece of feedback in the entire sprint. It is the lesson the team will remember longest.

---

## Positive feedback

For balance — Arefin and the cousin were not only critical:

- **Hexagon visual motif** — "Branded without being heavy-handed." (Arefin)
- **AI search "cites sources" label** — "This is the right move. Most products bury this or skip it entirely." (Arefin)
- **Information density on Dashboard home** — The cousin understood what the product did within ~30 seconds of opening it. Value clarity target met.

---

## Probes on AI trust (specific to H3)

When asked directly: *"On a scale of 1 to 5, how much would you trust the AI assistant's reply?"*

- **Arefin:** 4. Reason: "I can see the source. I can verify it. That makes a 1 into a 4."
- **Cousin:** 3. Reason: "I'd want to click through and read the source before I acted on it. But the option is there, which is the main thing."

This is the strongest validation signal we received for any single hypothesis (H3).

---

## Limitations of this session

- Two participants only. Sample is too small to generalise.
- Both participants were recruited from Mirazur's personal network. Acknowledged bias.
- Arefin is a senior practitioner, not the target user. His feedback is weighted toward design quality, less toward the new-hire experience.
- The cousin is closer to the target user but is not technically a software engineer (the persona).

These limitations are recorded transparently in `/delivery/validation-report.md`, Section 7.

---

## What we did with the findings

Within 24 hours of the call:
- All four findings logged with severity ratings (above and in the validation report).
- Decorative sparklines flagged in `/docs/decisions.md` (D15) for removal in MVP.
- Recommendations R1–R5 drafted into the validation report.
- Findings folded into the final-presentation walk-through.
