# Case Study — FOMC September 2026 Lifecycle
# 案例研究 — 美联储 2026年9月会议全生命周期

**As-of packaging:** Thu 2026-09-17 ~08:45 MYT  
**Path:** `/home/box/investment/research-os/case-studies/FOMC-2026-09-CASE.md`  
**Purpose:** Historical replay pack for Research OS training / showcase (logic, not decoration).

---

## 1. Case ID | 案例编号

| Field | Value |
|-------|-------|
| Case ID | FOMC-2026-09 |
| Event type | Central bank SEP meeting + first hike since 2023 (Warsh era) |
| Geography | US macro → global AI/semis duration |
| Coverage touch | NVDA AAPL MU SPCX TSLA ARM QCOM CRWV MRVL INTC UMC LITE PLTR AVGO |
| Lifecycle complete? | Pre → Decision → Post-Mortem → Feedback → Stock Revisit → Scorecard append |

---

## 2. Artifact map | 产物地图（replay order）

| Stage | Path | Status |
|-------|------|--------|
| Pre-Event Snapshot | `../events/fomc-2026-09/PRE_EVENT_SNAPSHOT.md` | **LOCKED** (do not edit) |
| Pre-Event Exec | `../events/fomc-2026-09/EXEC_SUMMARY.md` | **LOCKED** |
| Statement snippet | `../events/fomc-2026-09/STATEMENT_SNIPPET.txt` | Archive |
| Decision Analysis | `../events/fomc-2026-09/DECISION_ANALYSIS.md` | Interim (press incomplete) |
| Decision Exec | `../events/fomc-2026-09/DECISION_EXEC_SUMMARY.md` | Interim |
| Press PDF archive | `../events/fomc-2026-09/FOMCpresconf20260916.pdf` | CONFIRMED primary |
| Post-Mortem | `../events/fomc-2026-09/POST_MORTEM.md` | Complete |
| Post-Mortem Exec | `../events/fomc-2026-09/POST_MORTEM_EXEC_SUMMARY.md` | Complete |
| Stock Revisit | `../events/fomc-2026-09/STOCK_REVISIT.md` | Complete |
| Feedback Loop | `../feedback/FOMC-2026-09-FEEDBACK.md` | Complete |
| Scorecard period | `../scorecard/RESEARCH_SCORECARD.md` → period `FOMC-2026-09` | Appended |

---

## 3. Timeline (MYT) | 时间线

| When (MYT) | Milestone |
|------------|-----------|
| 2026-09-15 ~10:00–11:00 | Pre-Event Snapshot locked |
| 2026-09-17 ~02:00 | Statement + SEP (~2:00pm ET Sep 16) |
| 2026-09-17 ~02:30 | Press starts; Decision Analysis cut with press **INCOMPLETE** |
| 2026-09-16 US session close | Two-phase equity digestion complete |
| 2026-09-17 ~08:30–09:00 | Post-Mortem + Feedback + Stock Revisit + Scorecard |

---

## 4. Teaching points | 教学要点

### EN
1. **Price what was priced.** With FedWatch ~90%+, decision surprise ≈ 0; elasticity on the binary is N/A.  
2. **Name the real gap.** Path / SEP / communication — not hike vs hold.  
3. **Split path into count vs level.** Dots can be **less hawkish on count** and **more hawkish on HFL level** simultaneously.  
4. **Two-phase reaction.** Statement bid ≠ session close after hawkish press.  
5. **Idiosyncrasy hygiene.** LITE/INTC day moves are not Fed elasticity.  
6. **Preserve thesis history.** Pre-event files untouched; feedback appends learning without rewriting the past.  
7. **Private names.** SPCX: proxies only; never invent valuation.

### 简体中文
1. **先问已定价什么。** FedWatch约90%+时，二元决议惊喜≈0。  
2. **正确命名预期差。** 路径/SEP/沟通，而非加息vs按兵。  
3. **路径拆成次数与水平。** 点阵可同时“次数不如叙事鹰、水平更高更久更鹰”。  
4. **两阶段反应。** 声明后上涨 ≠ 鹰派记者会后收盘。  
5. **个股卫生。** LITE/INTC异动不是Fed弹性。  
6. **保留命题史。** 会前文件不改写；反馈只追加学习。  
7. **私营标的。** SPCX仅代理，禁止编造估值。

---

## 5. Central equation replay | 核心等式回放

| Component | Value | Class |
|-----------|-------|-------|
| Actual decision | +25 bp, 12–0 | CONFIRMED |
| Priced decision | ~92–93% | RELIABLE pre |
| Decision repricing | ≈ 0 | INFERENCE |
| Actual path | +1 more 2026; 4.1% through 2027 | CONFIRMED |
| Loudest priced narrative | ~100 bp cumulative | RELIABLE of narrative |
| Path-count repricing | Relief vs narrative | INFERENCE |
| Path-level / HFL | Hawkish vs June | INFERENCE |
| Press | Hawkish FC framing | CONFIRMED |
| Net for AI duration | Structural WACC lid **on**; decision-day crash **off** | INFERENCE |

---

## 6. Scenario realization | 情景实现

| Scenario | Pre prob | Realized? |
|----------|----------|-----------|
| Bear | 25% | Not fully |
| **Base** | **55%** | **Primary match** |
| Bull | 20% | Partial on hike-count only |

---

## 7. Scorecard snapshot | 记分卡快照

See `RESEARCH_SCORECARD.md` period **FOMC-2026-09**:
- Scenario discipline: **HIT**
- Forecast accuracy (binary): **HIT**
- Expectation-gap quality: **HIT/PARTIAL**
- Market-reaction: **PARTIAL** (Timing/Reaction)
- Probability calibration: **supportive** (n=1)

---

## 8. Replay checklist | 回放检查清单

- [ ] Read Pre-Event without peeking at Actual  
- [ ] Write your own Actual vs Expected table  
- [ ] Only then open Decision Analysis / Post-Mortem  
- [ ] Score your own error classes  
- [ ] Compare to Feedback Loop  
- [ ] Attempt elasticity with honest N/A where factor model missing  

---

## 9. One-paragraph case moral | 案例寓意

**EN:** FOMC-2026-09 is a clean Research OS specimen of a **priced binary + two-sided path surprise + hawkish communication completion**. Judgment quality lived in gap location and scenario discipline; residual learning lived in reaction-window timing and narrative-vs-dots path proxies.

**ZH:** FOMC-2026-09是研究系统的典型样本：**已定价二元决议 + 双向路径惊喜 + 沟通偏鹰补全**。判断质量体现在预期差定位与情景纪律；残留学习在反应窗口时序，以及“叙事路径 vs 点阵路径”的代理选择。

---

**End of Case Study.**
