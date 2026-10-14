# Master Research OS Dashboard — Architecture
# 主研究操作系统仪表盘 — 架构

**Path:** `/home/box/investment/research-os/dashboard/ARCHITECTURE.md`  
**Last updated:** 2026-09-15  
**Governing:** User master instruction + skill **Global Investment Research OS**  
**Principle:** Visualize **RESEARCH LOGIC** — not decorative boxes.

---

## EN — Purpose

A **cinematic research terminal**: one surface that makes the Research OS architecture chain *operable and inspectable*.

```
Macro → Industry → Company → Fundamentals → Market Expectations → Market-Implied
  → Expectation Gap → Catalyst → Actual → Surprise → Market Reaction
  → Event Elasticity → KPI → Scenario → Probability → Valuation → Portfolio → Feedback
```

Central equation (always on-screen when relevant):

> **Actual Fundamental Outcome − Priced Expectations = Repricing Potential**

Never imply: good news = up / bad news = down. Always ask what was priced.

---

## 简体中文 — 目的

**电影感研究终端**：把研究操作系统的逻辑链变成可操作、可审查的界面，而不是装饰性看板。

中心等式：

> **实际基本面结果 − 已定价预期 = 重定价潜力**

禁止默认：利好=上涨 / 利空=下跌。永远先问市场已定价什么。

---

## Modes | 模式

| Mode | Audience | Behavior |
|------|----------|----------|
| **Private / Research** | User + agents | Full theses, falsifiers, scorecard, errors, raw sources, drafts |
| **Presentation / Showcase** | External review | Sanitized narrative; logic still visible (chains, waterfalls, KPI lights); no private sizing/notes |

Data never invents prices; show `N/A (unverified)` when live quotes/fundamentals are missing.

---

## Data sources | 数据源

All modules read from `/home/box/investment/research-os/*` (and pointers under `/home/box/investment/`):

| Source tree | Feeds |
|-------------|--------|
| `companies/{TICKER}/` | Universe, CURRENT_STATE, expectation maps, KPI seeds |
| `calendar/` | Event Timeline, FOMC desk, earnings lifecycle |
| `events/` | Pre/post snapshots, reaction tapes |
| `scenarios/` | Scenario panels & probabilities |
| `valuation/` | Waterfalls, method fit, reverse DCF stubs |
| `kpi/` | Traffic lights |
| `feedback/` | Feedback loop records |
| `scorecard/` | Research Scorecard |
| `macros/` | FOMC / liquidity / Asia FX monitors |
| `case-studies/` | Historical event replays |
| `/home/box/investment/WATCHLIST.md` | Core universe + sleeve mapping |
| `/home/box/investment/reports/` | Archived daily tapes (e.g. afternoon 2026-09-15) |

---

## Pages / modules | 页面与模块

Each page must expose **logic edges** (arrows, gaps, falsifiers), not card grids alone.

### 1. Universe | 覆盖宇宙
- Core tickers + AI factory **sleeve / transmission position**
- Link into company CURRENT_STATE
- SPCX = SpaceX Nasdaq-listed (since 2026-06-12, CONFIRMED); CRWV = CoreWeave public

### 2. Event Timeline | 事件时间线
- Verified calendar (CONFIRMED vs UNVERIFIED)
- Lifecycle strip: Calendar → Pre → Actual → Reaction → Post-Mortem → Feedback

### 3. Expectation Maps | 预期地图
- Street Consensus → Market-Implied → Our Fundamentals → **Expectation Gap**
- Known / Underappreciated / Needs Evidence / Falsifiers
- Expectations ladder: Low-Bar / Consensus / Whisper / Structural Beat-Miss vs **price-required**

### 4. Transmission Chains | 传导链
- AI factory chain visualization (demand → compute → memory → optical → foundry → edge → space)
- Macro → industry → company edges for live events (e.g. FOMC → WACC/multiple → semis)

### 5. Scenarios | 情景
- EVENT: Bear/Base/Bull  
- RESEARCH: Bear / Low-Base / Base / High-Base / Bull  
- Probabilities sum 100%; Rev, Margin, EPS, FCF, Multiple, Range, Assumptions, Catalyst, Falsifier

### 6. Valuation Waterfalls | 估值瀑布
- Method fit (DCF, reverse DCF, SOTP, multiples, FCF yield, PEG, unit economics, optionality)
- Separate **Fundamental Value** vs **Market-Implied**
- Paths 2027–2030 when useful; no false precision

### 7. KPI Lights | KPI 信号灯
- GREEN / YELLOW / RED on **measurable evidence only**
- Default seed: YELLOW — insufficient evidence

### 8. Feedback / Scorecard | 反馈与记分卡
- Feedback loop: Original Thesis → Forecast → Actual → Surprise → Reaction → Error → Root Cause → Rectification → Recalibration → New Thesis
- Error classes: Fundamental / Expectation-Pricing / Transmission / Market-Reaction / Timing / Probability Calibration
- Links to `scorecard/RESEARCH_SCORECARD.md`

### 9. Thesis Versions | 论点版本
- Versioned theses; **never overwrite** pre-event / past theses
- Diff view: what changed and why

### 10. FOMC Desk | FOMC 工作台
- Schedule, SEP meetings, statement vs press, 2Y/10Y/30Y interpretation hooks
- Sep 2026 lifecycle controls

### 11. Tesla Module | 特斯拉模块
- Physical AI / AV / robotics / energy; dedicated falsifiers

### 12. SPCX Module | SPCX / SpaceX 模块
- Private/proxy handling; orbital / satellite / compute adjacency
- No invented listing or valuation

### 13. Convergence Module | 收敛模块
- Tesla × SpaceX (SPCX) convergence
- **Falsification rule** for merger / structural-link probability (probability must be falsifiable)

---

## Visual grammar | 视觉语法（研究逻辑，非装饰）

| Element | Means |
|---------|--------|
| Arrow / edge | Transmission or causal claim (must cite class: FACT / REPORTING / INFERENCE / HYPOTHESIS) |
| Gap bar | Expectation Gap magnitude (direction + uncertainty) |
| Waterfall step | Valuation bridge with assumption tags |
| Traffic light | KPI evidence state only |
| Timeline node | Event lifecycle stage; lock pre-event snapshot |
| Probability chips | Scenario weights summing to 100% |
| Version stamp | Thesis ID + timestamp — immutable history |

**Forbidden:** orphan KPI tiles, stock tickers as wallpaper, charts without expectation or transmission context.

---

## Terminology block pattern | 术语块

When introducing important terms on the dashboard:

| English | Chinese | Simple Explanation | Investment Meaning |
|---------|---------|--------------------|--------------------|
| Expectation Gap | 预期差 | Difference between what happened (or will) and what price embeds | Drives repricing potential |
| Event Elasticity | 事件弹性 | Abnormal return per unit surprise | How hard price moves for a given surprise |
| Falsifier | 证伪条件 | Observation that kills the thesis | Discipline against narrative lock-in |

---

## Implementation note | 实现说明

This file is **architecture only**. No app code is required here. Future showcase UI should consume the paths above and preserve bilingual EN → 简体中文 for substantive panels.
