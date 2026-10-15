# Feedback Loop — FOMC September 2026
# 反馈环 — 美联储 2026年9月会议

**As-of:** Thu 2026-09-17 ~08:45 MYT  
**Path:** `/home/box/investment/research-os/feedback/FOMC-2026-09-FEEDBACK.md`  
**Locked pre-event:** `/home/box/investment/research-os/events/fomc-2026-09/PRE_EVENT_SNAPSHOT.md`  
**Actuals:** `DECISION_ANALYSIS.md` + `POST_MORTEM.md`  
**Governing equation:** Actual Fundamental Outcome − Priced Expectations = Repricing Potential

---

## 0. Claim classes | 证据分级

CONFIRMED FACT | RELIABLE REPORTING | INFERENCE | HYPOTHESIS | SPECULATION | N/A

---

## 1. Original Thesis | 原命题

### EN (locked pre-event, HYPOTHESIS)
Base **55%**: +25 bp to 3.75%–4.00%; SEP revises inflation up / path modestly hawkish vs June but roughly consistent with market’s multi-hike narrative; Warsh light on explicit FG → limited decision surprise; residual path/communication volatility.  
**Expectation gap is NOT hike vs hold** (mostly closed). Gap = **terminal path, SEP inflation dots, dissent optics, Warsh oil framing**.

### 简体中文
基准55%：加息25bp；SEP通胀上修、路径偏鹰但大体匹配多段加息叙事；沃什少给明确前瞻指引。  
**预期差不在加息vs按兵不动，而在终端路径、SEP点阵、异议结构、油价框架。**

---

## 2. Forecast | 预测（会前登记）

| Item | Forecast | Prob / note |
|------|----------|-------------|
| Decision | +25 bp | Base 55%; FedWatch ~92–93% |
| Bear / Bull | Hawkish path shock 25% / Dove vs path fears 20% | EVENT matrix |
| Statement | Short; resolve language; limited FG | Style call |
| Surprise channel | SEP / dots / press | Core OS call |
| Tape | Choppy; AI still rate-sensitive | Base |

---

## 3. Actual | 实际

| Item | Actual | Class |
|------|--------|-------|
| Decision | +25 bp to 3.75–4.00%, **12–0** | CONFIRMED |
| Statement | Short; no FG; dropped supply-shock attribution (RELIABLE Reuters) | CONFIRMED + RELIABLE |
| SEP FF | **4.1% / 4.1%** (2026/2027) | CONFIRMED |
| Dots | 16/18 ≥ one more 2026 hike; 4 want two; 2 stop; Warsh no dot | CONFIRMED |
| Press | Standard unmet; too high too long; FC not restrictive → remove accommodation; inflation risks upside | CONFIRMED (PDF) |
| Reaction | Two-phase: post-statement bid → hawkish-press fade to S&P −0.4%, Dow −1.2%, Nasdaq flat; SOX +0.63% | CONFIRMED / RELIABLE |

---

## 4. Surprise | 惊喜/意外

| Surprise | Sign | Size (HYPOTHESIS 0–3) | Notes |
|----------|------|------------------------|-------|
| Binary decision | None | 0 | Fully priced |
| Unanimous vote | Mild hawkish optics | +0.5 | vs dissent chatter |
| Dropped supply-shock language | Hawkish framing | +1 | RELIABLE |
| Dots vs ~100 bp narrative | Fewer hikes than loudest narrative | −1 | Median = one more then HFL |
| HFL level vs June | 2027 median +50 bp vs June | +1 | Restrictive |
| Press FC “not restrictive” | Hawkish communication | +1.5 | Stronger than “ambiguous” Base sketch |
| Index two-phase fade | Timing | +1 on press window | Decision Analysis only saw first phase |

---

## 5. Reaction | 市场反应（观测）

- Equities: **sell-the-news bid then press fade** (RELIABLE/CONFIRMED).  
- Front end: 2Y firmer (~4.74% Reuters).  
- Long end: 10Y ~5.01% (Yahoo); not a >5.10% disorder spike.  
- Semis: SOX green; several coverage names green with **idiosyncratic contaminants** (LITE/INTC).  
- Elasticity vs decision surprise: **N/A** (surprise≈0). Qualitative elasticity vs press surprise: negative during press window.

---

## 6. Error | 误差

| Dimension | Error? | Class |
|-----------|--------|-------|
| Binary forecast | **No** | — |
| Scenario assignment | **No** — Base primary match | — |
| Expectation-gap location | **No** — correctly path/comms | — |
| Path narrative sizing (~100 bp) | **Partial** — overstated hike **count** vs median | Expectation-Pricing |
| Press hawkish intensity | **Partial** — Base allowed residual noise; underestimated FC “remove accommodation” bite | Expectation-Pricing / Transmission |
| Market reaction timing | **Yes (small)** — marked post-statement bid; underweighted press-fade close | Market-Reaction / Timing |
| Probability (55% Base) | **Supportive** (n=1) | Probability Calibration |
| Fundamental company EPS | N/A this event | — |

---

## 7. Root Cause | 根因

### EN
1. **Process success:** Locking pre-event and refusing to treat the binary as the gap prevented classic “good news = up” confusion.  
2. **Narrative contamination:** Using strategy-desk “~100 bp cumulative hikes” as a market-implied path proxy without a scraped CME path distribution inflated hike-**count** expectations.  
3. **Lifecycle cut timing:** Decision Analysis correctly labeled press INCOMPLETE; the residual error was treating the immediate equity bid as the reaction summary before session close.  
4. **Idiosyncrasy:** Semis day strength (LITE/INTC) can fool Fed-elasticity measurement if not tagged.

### 简体中文
1. **流程成功：** 锁定会前、不把二元决议当预期差，避免“利好就涨”误判。  
2. **叙事污染：** 用策略台“约100bp累计加息”代理市场路径、却无CME路径分布抓取，夸大了加息**次数**预期。  
3. **时点切割：** 决议分析正确标注记者会不完整；残留误差是把声明后瞬时上涨当最终反应。  
4. **个股异动：** LITE/INTC等未标记会污染Fed弹性测量。

---

## 8. Logical Rectification | 逻辑纠偏

1. Split every FOMC post-mortem into **T+0 statement window** and **T+0 press-to-close window**.  
2. Split path surprise into **hike count** vs **terminal / HFL level** vs **communication**.  
3. Prefer scraped FedWatch path or futures strips over strategy narrative when citing “priced path.”  
4. Tag idiosyncratic movers before computing sleeve elasticities.  
5. Never overwrite pre-event files (honored).

---

## 9. Model Recalibration | 模型再校准

| Model element | Before | After (HYPOTHESIS update) |
|---------------|--------|---------------------------|
| EVENT Base definition | Priced hike + residual path noise | Keep; add explicit **two-phase reaction** checklist |
| Path proxy | Multi-hike narrative ~100 bp | Use **SEP median / dots** as primary path anchor; narrative as secondary color only |
| Warsh press prior | Ambiguous / light FG | Prior for **hawkish FC framing** when inflation sticky + growth solid |
| Elasticity | Decision-centric | Decision elasticity often **N/A** when FedWatch >90%; measure vs path/press surprise |
| Coverage WACC | Higher real yields compress AI multiples | **Reinforced** — 4.1% through 2027 |

---

## 10. New Thesis | 新命题

### EN (HYPOTHESIS)
The first Warsh hike was a **priced binary**. The live debate is whether markets price **“one more then hold at 4.1%”** or keep October live under upside inflation risks and non-restrictive FC language. AI-duration multiples remain capped by **HFL + real yields** until one of those legs breaks. Next fundamental checkpoint inside coverage: **Micron Sep 30**.

### 简体中文（假设）
沃什首次加息是**已定价二元事件**。活辩论在于市场定价“再加一次后维持4.1%”还是在通胀上行风险与“金融条件不算紧缩”口径下继续交易10月加息。AI长久期倍数仍被**更高更久+实际利率**压制，直至其中一条腿打破。覆盖内下一基本面检查点：**美光9月30日**。

---

## 11. Error-class scorecard (this event) | 误差类别记分

| Error class | Hit? | Weight |
|-------------|------|--------|
| Fundamental | No material miss | — |
| Expectation-Pricing | **Partial** (100 bp count) | Medium |
| Transmission | Mild (press FC bite) | Low–Medium |
| Market-Reaction | **Yes (small)** press fade | Medium |
| Timing | **Yes (small)** | Medium |
| Probability Calibration | Supportive of 55% | Positive |

---

## 12. Linkage | 链接

- Post-Mortem: `../events/fomc-2026-09/POST_MORTEM.md`  
- Stock Revisit: `../events/fomc-2026-09/STOCK_REVISIT.md`  
- Case Study: `../case-studies/FOMC-2026-09-CASE.md`  
- Scorecard: `../scorecard/RESEARCH_SCORECARD.md`

---

**End of Feedback Loop.**  
**Do not rewrite** `PRE_EVENT_SNAPSHOT.md`.
