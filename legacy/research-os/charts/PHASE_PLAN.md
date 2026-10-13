# Research OS Charting — Phase Plan｜图表阶段计划
**Updated:** 2026-09-17 (Asia/Singapore)  
**Standard:** `research-os/charts/CHARTING_STANDARD.md`

## Overview｜总览
Three phases take Research OS from **logic-first HTML embeds** → **reusable Event Book diagrams** → **exportable showcase assets**. No invented series at any phase.

---

## Phase 1 — Daily Board chart embeds｜日报看板内嵌图 **DONE**
**Goal:** Embed bilingual (EN+简体中文) chart/diagram blocks into the Daily Board HTML with premium dark-navy cards, self-contained CSS/SVG (no required CDN).

**Deliverables (completed 2026-09-17):**
- Dated board: `/home/box/investment/research-os/dashboard/boards/2026-09-16-post-fomc-board.html`
- Canonical template: `/home/box/investment/research-os/dashboard/boards/template-daily-board.html`
- Chart blocks added:
  1. **Transmission Chain** SVG — FOMC → SEP path → yields → WACC → watchlist
  2. **Expectation Gap** panel — Base 55% HIT vs residual path risk
  3. **Scenario Probability** bars — Bear 25% / Base 55% / Bull 20% (pre) + Actual binary hike marker
  4. **Thinking Tutorial** 7-step horizontal visual strip
  5. **Mini Catalyst Timeline** — BOJ Fri Sep 18 CONFIRMED, AAPL Sep 18, Starship ~Sep 22 TENTATIVE, MU Sep 30
- Every chart: bilingual title, claim class, source/as-of caption, 1-line thinking caption
- SPCX labeled Nasdaq-listed since 2026-06-12 (not private); quote N/A when unverified

**Exit criteria:** File size grew vs pre-Phase-1; HTML parses; aesthetic matches existing navy cards.

---

## Phase 2 — Event Book Mermaid + reusable SVG exports｜事件簿与可复用导出 **DONE** (Transmission poster)
**Goal:** For each major Event Book, version Mermaid diagrams under `events/<event>/charts/` and export matching SVG/PNG to `charts/exports/YYYY-MM-DD-*.svg|png` for reuse across boards/monitors.

**Status:** Transmission Chain premium poster **DONE** 2026-09-17. Remaining Phase-2 diagram types (Expectation Gap SVG, Scenario Probability, Reaction Decomposition, Thinking Tutorial standalone) still planned as follow-ons; Mermaid sources already under `events/fomc-2026-09/charts/`.

**Deliverables (completed 2026-09-17):**
- `events/fomc-2026-09/charts/FOMC-2026-09-transmission-poster.svg` — 1920×1080 bilingual cinematic poster
- `charts/exports/2026-09-17-fomc-transmission-poster.svg` — exports library twin
- `events/fomc-2026-09/charts/FOMC-2026-09-transmission-poster.html` — offline browser wrapper
- Content: Oil→FOMC +25bp 3.75–4.00% 12–0 → SEP 4.1/4.1 → Path>decision → 10Y~5% → WACC↑ → AI duration watchlist; side callout Pre Base 55% BINARY HIT; Warsh tone RELIABLE; 7-step thinking strip; claim classes + sources; as-of 2026-09-17; no invented prices; SPCX Nasdaq since 2026-06-12

**Planned artifacts (broader Phase 2 set):**
- Transmission Chain, Expectation Gap, Scenario Probability, Reaction Decomposition (conceptual if incomplete), Thinking Tutorial flow
- Keep claim classes + sources in caption files alongside exports
- Wire Event Book markdown to the same figures used on Daily Boards (single source of truth)

**Exit criteria (this tranche):** FOMC-2026-09 transmission poster + dated export set — met. Full chart-folder set remains iterative.

---

## Phase 3 — Company packs & showcase polish｜公司包与展示打磨
**Goal:** When material, add company-pack diagrams (revenue/margin bridge, KPI lights, SOTP, CapEx→bottleneck) and a polished showcase HTML that reuses Phase 1–2 assets without tip-sheet aesthetics.

**Planned artifacts:**
- Company CURRENT_STATE chart slots (only verified KPIs)
- Showcase page assembling Event Book + Daily Board chart language
- Optional PNG share pack from HTML/SVG (never invent pixels)

**Exit criteria:** One AI-chain company pack with compliant charts; showcase opens offline (self-contained CSS).

---

## Status snapshot｜状态快照
| Phase | Status | As-of |
|-------|--------|-------|
| 1 Daily Board embeds | **DONE** | 2026-09-17 |
| 2 Event Book exports | **DONE** (transmission poster) | 2026-09-17 |
| 3 Company / showcase | Pending | — |


## Phase 3 status
IN PROGRESS 2026-09-17 — wiring chart pack recipe into AI Factory Morning/Afternoon/Evening routine prompts.


## Phase 3 status
DONE 2026-09-17 — AI Factory Morning/Afternoon/Evening prompts updated to require daily chart packs per DAILY_CHART_PACK_RECIPE.md. All three chart phases complete.
