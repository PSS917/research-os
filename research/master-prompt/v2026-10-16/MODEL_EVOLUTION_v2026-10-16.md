# Model Evolution — Regime-aware probability calibration (v2026-10-16)
# 模型进化 — 波动率体制下的概率校准

**Date:** 2026-10-16 MYT · **Status:** PROMOTED to Core Model (user-approved) · **Master prompt:** v2026-10-16 Part G (extends v2026-10-14 Part F)

## What we believed before｜之前的做法
Scenario probabilities were centred on "in-line" (typically 50–55%), scenarios were often described on the headline print, and the earnings "Beat" case assumed a positive reaction.

## Evidence that tested it｜检验证据（本系统事后复盘）
- **US CPI Sep-26 (10/14):** core HOT (core m/m 0.3% vs 0.2% consensus). Locked prior 25/50/25 scored Brier 0.875 vs base rate (36m core m/m) 0.353 — worse than the base rate.
- **US PPI Sep-26 (10/15):** landed HOT (tail).
- **US Retail Sales Sep-26 (10/15):** landed STRONG (tail).
- **TSM Q3-26 (10/15):** revenue beat, but ADR −1.8% vs the pre-event Beat playbook (+3% to +7%); the semiconductor sector was de-crowding (AMAT −10.2% over two days). Error class: probability calibration (main) + market-reaction (secondary).
- **Regime at adoption (2026-10-16):** VIX 16.46 (not high); MOVE 102.49 > its 1-year P80 80.54 (high); last 3 macro releases all in tails (high) → regime HIGH.

## Decision｜决定
1. Concrete high-volatility regime: VIX > 20 OR MOVE > 110 / > 1-year P80 OR last 3 macro releases all in tails.
2. In a HIGH regime cap the middle scenario at 45%, redistribute to the tails, renormalise (after the Part F base-rate shrink).
3. Define scenarios on decision-relevant variables (core, control group, PCE-relevant components, guides), not the headline.
4. Earnings: split Beat into sector-tailwind vs sector-headwind using sector momentum (SOX 5-day).

## Variable record｜变量档案
| Variable | First discovered | Event that tested it | Effect | Status |
|---|---|---|---|---|
| Base-rate shrink (gap >20pp → ≥50%) | 2026-10-14 (CPI post) | CPI Sep-26 | Strengthened | Core (v2026-10-14) |
| High-vol middle cap 45% | 2026-10-16 | CPI/PPI/Retail Sep-26 tails | New | Core (v2026-10-16) |
| Decision-relevant scenario variable | 2026-10-16 | CPI (core vs headline), Retail (control group) | New | Core |
| Beat × sector momentum split | 2026-10-16 | TSM Q3-26 | New | Core |

## Falsifier / review｜复核条件
Review after the next 6 tier-1 events: if cumulative Brier with the cap is worse than without it, downgrade the cap to Observation Zone.

## Files updated
`pipeline/calibration.py` (old rule kept in `calibration_v2026-10-14.py`), `build_ppi_pre.py`, `build_tsm_pre.py`, `build_1015_pre.py`, master prompt v2026-10-16, skill file.
