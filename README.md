# AI-Powered Credit Card Recommendation Engine

A full-stack product concept — from PRD to interactive prototype — demonstrating how intelligent, contextual data collection can replace rigid financial questionnaires and deliver personalised credit card recommendations.

**[Live Demo →](https://SaiAjay29.github.io/creditcard-prototype)**

---

## Overview

Most credit card discovery journeys suffer from information overload, rigid forms, and poor personalisation — leading to 70%+ drop-off rates. This project reimagines that journey with an AI-driven recommendation engine that:

- Collects context through a **conversational 4-step micro-survey** instead of a 15-field form
- Uses **multiple data signals** (spend categories, income, preferences) to score and rank cards
- Surfaces a **personalised recommendation** with a match score and human-readable reasoning
- Keeps the user **in control** with swappable alternatives and transparent data consent

---

## What's Included

| File | Description |
|------|-------------|
| `index.html` | Fully interactive prototype — 6 screens, working recommendation engine |
| `prd.html` | Complete PRD — 11 sections including personas, architecture, user stories, RICE prioritization |

---

## Prototype Walkthrough

```
Hero Screen → Data Consent → 4-Step Survey → AI Loading → Recommendation → Apply
```

1. **Hero** — Value prop + card gallery before any data is asked
2. **Consent** — Modular opt-in for SMS, bureau pull, bank statement
3. **Survey** — Spend categories (chip select) → Monthly spend (slider) → Income range → Priority
4. **Loading** — Animated steps simulating real ML pipeline stages
5. **Recommendation** — Match score, personalised "why this card" reasoning, benefit chips, swappable alternatives
6. **Apply** — Success screen with reference number

---

## Recommendation Engine

Built entirely in vanilla JS — no backend required for the demo. The scoring logic:

```js
score = Σ (spend_category_weight × card_score)
      + preference_match_bonus
      + spend_threshold_bonus
      - income_ineligibility_penalty
```

Cards are ranked by score and the top match is surfaced with dynamically generated reasoning tied to the user's actual inputs — not static copy.

---

## PRD Highlights

- **Problem Statement** — 6 root causes of broken card discovery journeys
- **User Personas** — 4 archetypes: Daily Commuter, Frequent Flier, Online Shopper, SME Owner
- **Technical Architecture** — 6-layer stack: Client → API Gateway → Recommendation Engine → Integrations → Data → Security
- **Data Strategy** — 6 input signals with quality ratings; v1 rule-based → v2 ML model roadmap
- **10 User Stories** — With full acceptance criteria across 4 epics
- **MoSCoW + RICE** — Prioritization framework with scored feature backlog
- **4-Sprint MVP Plan** — 8-week delivery roadmap with story points
- **Success Metrics** — 8 KPIs with baselines and funnel tracking strategy

---

## Tech Stack

- **Frontend** — Vanilla HTML, CSS, JavaScript (zero dependencies)
- **Styling** — CSS custom properties, responsive grid, smooth transitions
- **Logic** — Client-side scoring engine, state machine for screen navigation
- **Hosting** — GitHub Pages

---

## Skills Demonstrated

`Product Thinking` `PRD Writing` `User Research` `Information Architecture` `Conversion Optimisation` `Frontend Prototyping` `Recommendation Systems` `Data Strategy` `Agile / Sprint Planning`

---

## Running Locally

No build step needed — just open the file:

```bash
git clone https://github.com/SaiAjay29/creditcard-prototype.git
cd creditcard-prototype
open index.html   # or double-click the file
```
