# US CPI Sep 2026 — Post-Event Review (English) v20261015-0800-post
> Final (close-of-day) | Locked pre-event book: v20261013-1803 (2026-10-13T18:03:00+08:00) | Data: BLS API; markets yfinance (session 2026-10-14) | **Not investment advice**

## 1. Actual vs consensus vs our hypothesis
| Metric | Actual | Consensus (locked) | OS hypothesis | Surprise |
|---|---|---|---|---|
| headline_mom | 0.6% | 0.6% | 0.58% | +0.0pp |
| headline_yoy | 3.7% | 3.6% | 3.6% | +0.1pp |
| core_mom | 0.3% | 0.2% | 0.22% | +0.1pp |
| core_yoy | 2.6% | 2.5% | 2.4% | +0.1pp |

Classification: **HOT**. Prior probabilities cool/in-line/hot: 25%/50%/25%.

## 2. Market reaction (release-day close vs prior close)
| Asset | Close | Prior | Change |
|---|---|---|---|
| 10Y | 5.19 | 5.22 | -2.7bp |
| S&P500 | 7,718.94 | 7,805.45 | -1.11% |
| NDX | 29,950.82 | 30,569.48 | -2.02% |
| SOX | 11,684.38 | 12,208.79 | -4.30% |
| USDJPY | 158.32 | 158.52 | -0.12% |
| VIX | 16.87 | 15.27 | +10.48% |

Kalshi (public API, 2026-10-15 08:00 MYT, last trade): October-meeting hike 31% (prior day 20%; locked pre-event 20%); December-meeting hike 83%.

## 3. Rate-sensitivity prediction vs actual
| Ticker | Sensitivity per +10bp | Predicted | Actual | Error |
|---|---|---|---|---|
| CCL | -2.59% | +0.70% | +0.94% | +0.24pp |
| ARM | -2.56% | +0.69% | +0.06% | -0.63pp |
| SPCX | -2.56% | +0.69% | -4.21% | -4.90pp |
| MRVL | -1.84% | +0.50% | +1.08% | +0.58pp |
| RKLB | -1.77% | +0.48% | -2.27% | -2.75pp |
| INTC | -1.53% | +0.41% | +1.44% | +1.03pp |
| GLW | -1.49% | +0.40% | +0.86% | +0.45pp |
| KLAC | -1.21% | +0.33% | -3.22% | -3.55pp |
| CIEN | -1.18% | +0.32% | -1.14% | -1.46pp |
| QCOM | -1.16% | +0.31% | +1.39% | +1.08pp |
| AMD | -1.05% | +0.28% | +1.90% | +1.62pp |
| NDX | -0.67% | +0.18% | -2.02% | -2.20pp |
| SOX | -0.89% | +0.24% | -4.30% | -4.54pp |


## 4. Probability calibration vs base rate
Rule: when our/consensus probability differs from the base rate by >20pp, shrink toward the base rate by ≥50%.
| Scenario | Prior | Base rate (36m core m/m) | Calibrated | Outcome |
|---|---|---|---|---|
| cool | 25% | 14% | 22% |  |
| inline | 50% | 33% | 44% |  |
| hot | 25% | 53% | 34% | ✔ |


## 5. Source ledger
| Item | Value | Source | Time |
|---|---|---|---|
| CPI 实际（核心/整体 环比、同比） | {'headline_mom': 0.6, 'headline_yoy': 3.7, 'core_mom': 0.3, 'core_yoy': 2.6} | BLS API（SA 算环比，NSA 算同比） | 2026-10-14 20:30 SGT |
| 共识 | 核心环比 0.2%、同比 2.5% | 事前书 v20261013-1803（锁定） | 2026-10-13T18:03:00+08:00 |
| 10Y 变动 | -2.7bp | yfinance ^TNX | 2026-10-14 收盘 |
| Kalshi 10 月加息 | 0.31 | Kalshi 公开 API KXFEDDECISION-26OCT | 2026-10-15 08:00 MYT |
| Kalshi 12 月会议加息 | 0.8300000000000001 | Kalshi 公开 API KXFEDDECISION-26DEC | 2026-10-15 08:00 MYT |
| 利率敏感度 | 13 只 | 事前书 §利率敏感度（过去一年回归，R² 低） | 2026-10-13T18:03:00+08:00 |
| 基础概率 | 偏冷/符合/偏热 14%/33%/53% | FRED CPILFESL 过去 36 个月 | 本次运行 |
| 个股/指数涨跌 | 17 项 | yfinance | 2026-10-14 |


## 6. Assumption register
| # | Assumption | Type | Test / failure condition |
|---|---|---|---|
| 1 | 偏热阈值：核心环比 ≥0.25% 或意外 ≥+0.1pp | ASSUMPTION | 若市场对 0.25% 无反应，阈值需上调 |
| 2 | 利率敏感度在事件日仍成立 | HYPOTHESIS | 偏差 MAE > 1.5pp 视为失效（Excel Sensitivity!MAE） |
| 3 | Kalshi 最新成交价≈市场概率 | ASSUMPTION | 成交稀薄/价差 >5c 时不可靠 |
| 4 | 36 个月基础概率代表当前通胀体制 | ASSUMPTION | 若体制切换（如连续加息周期），基础概率需重算 |
| 5 | 概率校准规则：差 >20pp 收缩 ≥50% | RULE (master prompt v2026-10-14) | 累计 Brier 若校准后更差则复核规则 |


## 7. Chain post-mortem
The detailed link-by-link reasoning review is in the Chinese edition (§4). Summary: core surprise +0.1pp, 10Y -2.7bp.
