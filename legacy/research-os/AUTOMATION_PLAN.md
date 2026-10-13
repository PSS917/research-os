# Research OS — Automation Plan (PROPOSAL ONLY)
# 研究操作系统 — 自动化方案（仅提议，勿创建例程）

**Path:** `/home/box/investment/research-os/AUTOMATION_PLAN.md`  
**Status:** Proposal — **do not create routines from this file yet**  
**Timezone:** Asia/Kuala_Lumpur (MYT)  
**Last updated:** 2026-09-15

---

## Goal | 目标

Minimum durable automation that covers **events, companies, AI safety, and finite lifecycles** — without tripling the same AI-factory narrative three times a day forever.

---

## Recommendation: fold gradually into Master Event Monitor

**Keep** existing AI Factory Morning / Afternoon / Evening outputs only while the fold-in is incomplete.  
**Recommend:** gradually **fold** the three daily AI Factory reports into a single **Master Event Monitor**, then retire redundant daily sessions.

### Why this avoids redundancy

| Current | Problem |
|---------|---------|
| Morning 08:30 + Afternoon 17:30 + Evening 21:00 AI Factory reports | Three passes over the same universe/transmission story; high overlap when nothing material changed |
| Separate ad-hoc event checks | Easy to miss FOMC/earnings lifecycle stages or double-write the same surprise |

| Proposed | Benefit |
|----------|---------|
| **One** Master Event Monitor (weekday) | Single daily scan: what changed, expectation gap, transmission, alerts only if material to Rev/EPS/FCF/WACC/multiple/scenario/KPI/thesis/vol |
| Company Event Monitor (3×/week) | Deeper IR/SEC/catalyst pass without bloating every morning |
| AI Safety Watch (2×/week) | Governance/safety thread without polluting market tape |
| Finite FOMC / MU routines | High-intensity only when verified events are live — then stop |

Quiet when nothing material. Daily AI Factory triple-cadence becomes optional archive/export from Master Event Monitor, not three independent research runs.

---

## MINIMUM proposed routines (DO NOT CREATE YET)

### Standing

| Routine | Cadence (MYT) | Role |
|---------|---------------|------|
| **Master Event Monitor** | Daily **08:00 MYT**, weekdays | Primary daily: calendar + macro/liquidity + universe surprises + transmission alerts; eventually absorbs Morning/Afternoon/Evening substance |
| **Company Event Monitor** | **Mon / Wed / Fri 09:00 MYT** | IR, filings, guidance, segment KPIs for core universe |
| **AI Safety & Governance Watch** | **Tue / Fri 10:00 MYT** | Model/policy/safety/governance items material to AI CapEx, regulation, or thesis falsifiers |

### Finite / event-lifecycle (verified dates only)

| Routine | When | Role |
|---------|------|------|
| **FOMC Sep 2026 lifecycle** | Finite window around Sep 15–17 MYT | Pre-snapshot → statement/SEP → press → reaction → post-mortem → feedback; then **end** |
| **MU pre-earnings** | **Sep 29, 2026** | Lock pre-event thesis, expectation map, scenarios, falsifiers |
| **MU post-event** | **Sep 30 / Oct 1, 2026** | Actual vs expected, reaction, elasticity, feedback (call ~04:30 MYT Oct 1 **calculated** from 2:30pm Mountain Sep 30) |

Do **not** schedule rumor dates.

---

## Fold plan (gradual)

1. **Phase A:** Run Master Event Monitor at 08:00 MYT weekdays **in parallel** with existing AI Factory trio; tag overlap.  
2. **Phase B:** Afternoon/Evening become thin “tape append” only if Master flagged material US-session items.  
3. **Phase C:** Retire Morning/Afternoon/Evening as separate research jobs; keep `/home/box/investment/reports/` as export path from Master + lifecycle routines.  
4. User approval required before deleting or disabling any existing AI Factory routine.

---

## Alert discipline

Alert only when material to: Revenue / EPS / FCF / WACC / multiple / scenario / KPI / thesis / volatility.  
Classify claims; never invent prices.

---

## Explicit non-actions

- This document **proposes** only.  
- **Do not create** cron jobs, workflow schedules, or bot routines until the user approves.  
- **Do not** invent additional daily report slots beyond the minimum above.
