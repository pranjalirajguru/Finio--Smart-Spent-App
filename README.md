# Finio — Smart Spending & Financial Insights App
### A Portfolio-Ready UX Case Study + Fintech Product UI

---

## Overview

**Finio** is a complete, single-page UX case study and product prototype for a smart spending and financial insights application. Built as a portfolio artifact, it demonstrates both **UX/UI design thinking** and **data analysis capability** — the kind of work expected from a senior product designer or data analyst at a top consulting firm.

Inspired by products like Google Pay, CRED, and Mint, but designed with a distinct aesthetic — minimal, dark-mode-forward mobile screens combined with a clean white analytical case study.

---

## What's Inside

### 7 Structured Sections

| # | Section | What it demonstrates |
|---|---------|----------------------|
| 1 | **Hero** | Product positioning, brand identity, fintech aesthetic |
| 2 | **Problem Statement** | Design thinking, user pain point articulation |
| 3 | **User Persona** | Research synthesis, empathy mapping |
| 4 | **Data Analysis** | Chart literacy, financial data visualisation |
| 5 | **Smart Insights** | AI-driven product feature design |
| 6 | **App UI Screens** | Mobile UI design, 4 complete product screens |
| 7 | **Design System** | Colour palette, typography, component library |

---

## App Screens Included

### Dashboard Screen
- Total balance card with income / spent / saved breakdown
- Weekly bar chart with Friday spending peak highlight
- 4 quick-insight metric cards

### Transactions Screen
- Categorised transaction list (Swiggy, Amazon, Salary, Bills, Netflix, Ola, etc.)
- Category filter pills
- Colour-coded debit/credit amounts

### AI Insights Screen
- Financial Health Score ring gauge (74/100)
- 4 actionable insight cards with severity tags (Action Needed, Quick Win, Goal Alert)
- Behaviour-specific recommendations

### Budget Tracker Screen
- Overall budget utilisation bar (76%)
- 5 category progress bars with real-time overspend detection
- Food category shown as over-budget (103%) with red indicator

---

## Data Analysis Features

### Charts Used
- **Bar Chart** — Category-wise monthly spend (Food, Shopping, Bills, Travel, Health, Subscriptions)
- **Donut Chart** — Proportional spend distribution (5 segments)
- **Line Chart** — 18-day daily spending trend with peak detection
- **Grouped Bar Chart** — April vs March comparison across all categories

### Summary Metrics (April 2025 Mock Data)
- Total Spent: ₹38,240 (↑12% vs March)
- Total Saved: ₹15,600
- Budget Used: 76% of ₹50,000
- Top Category: Food at ₹12,400 (32%)

### Smart Insights Shown
- "You spent 35% more on food this week"
- "Your highest spending day is Friday (2.4× daily avg)"
- "Save ₹2,000/month by cancelling overlapping subscriptions"
- "3 late-night shopping purchases above ₹1,500 detected"
- "Savings goal at risk — ₹3,400 short this month"
- "Electricity bill 18% lower — positive streak"

---

## Animation System

Every section features purpose-built motion design using pure CSS animations and vanilla JS IntersectionObserver — no animation libraries needed.

### Page Load Animations
| Element | Animation | Duration |
|---------|-----------|----------|
| Navigation bar | Slide down from top | 0.6s |
| Hero badge | Fade up | 0.7s |
| Hero headline | Fade up with stagger | 0.8s |
| Hero description | Fade up | 0.8s |
| CTA buttons | Fade up | 0.8s |
| Hero stat numbers | Animated number counter (0 → value) | 1.4s |
| Hero visual (SVG card) | Slide in from right | 1.0s |

### Continuous Animations
| Element | Animation | Details |
|---------|-----------|---------|
| Hero SVG mockup | Gentle float up/down | 6s loop |
| Hero background orb | Slow drift + scale | 14s loop |
| Hero floating particles (5) | Independent float paths | 7–12s loops |
| Hero accent word ("Effortlessly") | Gradient colour shift | 5s loop, green→blue→purple |
| Nav CTA button | Shimmer sweep on hover | 0.5s |
| Insight "Save" badges | Glow pulse ring | 2.5s loop |
| App UI section background | Radial gradient drift | 12s loop |

### Scroll-Triggered Animations (IntersectionObserver)
All elements below the fold animate in when they enter the viewport at 12% threshold:

| Section | Animation | Stagger |
|---------|-----------|---------|
| All section headers | Label slides left, title fades up, sub fades up | 0.1s / 0.2s offset |
| Section label underline | Width draws from 0 to 32px | 0.3s delay |
| Problem cards (×3) | Fade + translateY up | 0.1s each |
| Problem icons | Bounce scale on hover | Trigger on hover |
| Persona card | Fade + translateY | Single entrance |
| Persona tags (×6) | Pop in with spring (scale 0→1) | 0.08s each |
| Summary metric cards (×4) | Fade + scale + translateY | 0.1s each |
| Chart cards (×4) | Fade + translateY | 0.05–0.2s stagger |
| Insight cards (×6) | Fade + translateY | 0.1s row stagger |
| Insight icon wraps | Spin + scale in | 0.3s after card |
| Phone frames (×4) | Fade + translateY + scale | 0.12s each |
| Phone frame labels | Fade + translateY | Matches frame |
| Phone frames on hover | Float up + slight scale | 0.3s ease |
| UX decision cards (×3) | Fade + translateY | 0.12s each |
| Design system blocks (×4) | Fade + translateY | 0.06–0.18s stagger |
| Color swatches | Slide in from left | 0.08s each |

### Interactive Animations
| Interaction | Effect |
|-------------|--------|
| Insight card mouse move | Radial glow follows cursor (CSS custom properties) |
| Primary button click | Ripple expand + fade |
| Transaction list hover | Background highlight + indent slide |
| Nav links | Active section highlight in emerald (IntersectionObserver) |
| Scroll progress bar | Gradient bar (green→purple) across top of page |
| Budget bars | Width animates from 0 to final value on page load |

---

## Tech Stack

| Layer | Choice |
|-------|--------|
| Structure | Semantic HTML5 |
| Styling | Embedded CSS (zero frameworks) |
| Charts | Chart.js 4.4.1 via CDN |
| Animations | Pure CSS keyframes + JS IntersectionObserver |
| Fonts | Sora (display/UI) + DM Mono (data/numbers) via Google Fonts |
| Layout | CSS Grid + Flexbox |
| Responsive | Media queries at 900px breakpoint |

**File count:** 1 HTML file, self-contained  
**Dependencies:** Chart.js (CDN), Google Fonts (CDN)  
**Backend required:** None — all static/mock data  
**Animation library:** None — pure CSS + ~60 lines of vanilla JS

---

## Design System

### Colours
| Token | Hex | Usage |
|-------|-----|-------|
| Emerald | `#00C97A` | Primary actions, savings, success |
| Ink | `#0D0D0D` | Headlines, high-contrast text |
| Rose | `#FF4E6A` | Overspend, warnings, food category |
| Amber | `#F5A623` | Caution, near-limit states |
| Lavender | `#7C5CFC` | AI score, insights, intelligence |
| Teal | `#00BCD4` | Travel category |
| Surface | `#F5F5F5` | Background, card fills |

### Typography
- **Display/UI:** Sora (weights 300–700) — distinctive, modern, legible at all sizes
- **Data/Numbers:** DM Mono — monospaced for financial figures, prevents layout shift

### Component Tokens
- Card radius: `20px` (desktop), `26px` (phone screens)
- Phone frame radius: `40px`
- Shadow scale: `sm` / `md` / `lg`
- Button shape: `border-radius: 100px` (pill style throughout)

---

## UX Rationale

1. **Charts over tables** — Visual processing of spend categories is 60% faster than scanning numbers
2. **Minimal dark UI on mobile** — Reduces visual noise; one action per screen drives 3× engagement
3. **Contextual insights** — Transaction-specific nudges create emotional resonance and behaviour change
4. **Colour semantics** — Rose = danger, Amber = caution, Emerald = positive; no legend needed
5. **Progress bars for budgets** — Proportional fill creates immediate understanding of budget health
6. **Purposeful motion** — Animations guide attention, confirm interactions, and make the product feel alive without being distracting; all respect `prefers-reduced-motion` best practices

---

## File Structure

```
smart-spending-app.html     ← Complete single-file application (with animations)
README.md                   ← This file
```

---

## How to Use

1. Open `smart-spending-app.html` in any modern browser
2. No build step, no npm install, no server required
3. Internet connection needed only for CDN fonts and Chart.js
4. Scroll through the page to trigger all entrance animations

### Customisation
- All mock data is in the `<script>` block at the bottom of the HTML
- CSS custom properties (variables) at the top of `<style>` control all colours
- Animation durations and delays are in the `/* ANIMATIONS & MOTION SYSTEM */` CSS block
- Add real API data by replacing the static arrays in the Chart.js initialisations

---

## Portfolio Usage

This project is designed to demonstrate:
- **UX Design Thinking** — Problem → Persona → Solution → Rationale
- **Data Visualisation** — 4 distinct chart types with real financial context
- **UI Craft** — 4 fully designed mobile screens with realistic mock data
- **Motion Design** — 25+ distinct animations across load, scroll, hover, and interaction states
- **Systems Thinking** — Consistent design system across all components
- **Fintech Domain Knowledge** — Realistic metrics, Indian market context (₹), UPI-era spending patterns
- **Frontend Engineering** — Zero-dependency animation system, IntersectionObserver, CSS keyframes, counter animation

---

*Designed and built as a consulting-grade portfolio artifact · 2025*

