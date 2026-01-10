# Prana Health - UI/UX Design Mockups

High-fidelity mobile-first UI mockups for Prana Health, a YC-backed preventive healthcare platform focused on continuous, AI-driven health monitoring and early risk detection.

## Design Philosophy

**Calm, Clinical, Trust-First**
- No gamification noise
- One insight → one consequence → one action per screen
- No dense dashboards; progressive disclosure only
- Default view understandable in <10 seconds

## Screen Overview

### 1. Health Risk Trajectory (Primary Screen)
**File:** `1-risk-trajectory.html`

Visualizes projected 6-12 month risk for key conditions (metabolic, cardiovascular, sleep, inflammation). Shows direction (improving/worsening), not raw metrics. Includes a subtle "if nothing changes" baseline.

**Key Features:**
- Overall health risk summary
- Interactive trajectory visualization
- Risk breakdown by condition (metabolic, cardiovascular, sleep, inflammation)
- Trend indicators with color coding
- Baseline comparison

**Rationale:** Risk visualization increases intervention adherence by ~30-40% vs static metrics. The trajectory chart provides immediate visual feedback on where the user is heading, making abstract health data tangible.

---

### 2. Daily Action Confidence Score
**File:** `2-daily-confidence.html`

Single daily score (0-100) summarizing whether today's behavior helped or hurt long-term health. Shows top 2 contributing behaviors and provides 1 corrective action for tomorrow.

**Key Features:**
- Large confidence score visualization (circular progress)
- Daily summary metrics (steps, sleep, on-track percentage)
- Top contributors (what helped)
- Areas for improvement (what hurt)
- One actionable item for tomorrow

**Rationale:** Closure loops increase habit retention 2-3× (validated across behavior-change products). The single score reduces cognitive load while the one action prevents overwhelm.

---

### 3. Silent Risk Detection
**File:** `3-risk-detection.html`

Background AI flags early risk patterns before symptoms appear. Uses plain language, no medical jargon.

**Key Features:**
- Early detection alerts with severity badges
- Plain language explanations
- Pattern details (metrics, duration, trends)
- Actionable suggestions (3-4 specific steps)
- Historical insights (resolved patterns)

**Rationale:** ~90% of chronic disease progression is asymptomatic early—this builds trust and defensibility. By catching patterns early and explaining them clearly, users feel empowered rather than alarmed.

---

### 4. Doctor-Ready Health Brief
**File:** `4-health-brief.html`

One-click, auto-generated clinical summary (PDF/shareable). Includes trends, anomalies, and suggested questions.

**Key Features:**
- 30-day health summary
- Quick stats overview
- Key trends by category
- Notable patterns/anomalies
- Pre-written questions for doctor visits
- PDF export and sharing

**Rationale:** Reduces consultation time by ~20-30% and increases clinical adoption. Doctors get structured, actionable data instead of fragmented patient reports.

---

## Design System

**File:** `design-system.css`

### Color Palette
- **Primary:** Trust blue (#2563EB) - builds confidence
- **Success:** Subtle green (#10B981) - positive trends
- **Warning:** Gentle amber (#F59E0B) - attention needed
- **Error:** Soft red (#EF4444) - risks
- **Neutrals:** Gray scale (50-900) for text and backgrounds

### Typography
- **Font Family:** System fonts (-apple-system, Segoe UI, Roboto)
- **Sizes:** 12px (xs) to 36px (4xl)
- **Weights:** 400 (normal) to 700 (bold)
- **Line Heights:** 1.25 (tight) to 1.75 (relaxed)

### Spacing
- Consistent 4px base unit
- Scale: 4px, 8px, 16px, 24px, 32px, 48px, 64px

### Components
- Cards (elevated, standard)
- Buttons (primary, secondary, full-width)
- Status indicators (improving, worsening, stable)
- Navigation bar (bottom fixed)
- Progress bars
- Empty states

---

## Usage

1. Open `index.html` in a browser to see the landing page with all screens
2. Navigate to individual screens using the links or bottom navigation
3. All screens are mobile-first (max-width: 428px)
4. Screens are fully interactive with navigation between them

---

## Success Metrics

These designs are optimized for:
- ↑ Weekly active usage
- ↑ Intervention compliance
- ↓ User churn driven by confusion or overwhelm

---

## Microcopy Principles

- **Reassurance over urgency:** "Your trajectory is improving" not "Warning: Risk detected"
- **Plain language:** "Sleep latency increased" not "Polysomnographic latency elevation"
- **Actionable:** "Aim to finish dinner by 8 PM" not "Consider dietary modifications"
- **Empowering:** "Your actions today supported your goals" not "You're doing okay"

---

## Notes

- All screens use the same design system for consistency
- Navigation is persistent across all screens (bottom bar)
- Empty states and loading states are considered but not fully implemented
- Color coding is consistent: green (improving), red (worsening), gray (stable)
- All interactive elements have hover states and transitions
