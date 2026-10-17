# Research OS Charting & Diagram Standard｜图表与图示标准
**Effective:** 2026-09-17  
**Scope:** All Event Books, daily boards, monitors, company CURRENT_STATE packs, and showcase HTML.

## Purpose｜目的
Diagrams and charts visualize **research logic**, not decoration.
目标：把研究逻辑视觉化，不做装饰。

## Non-negotiables｜硬规则
1. **No invented series.** If a print is unverified → show `N/A` or omit the series; never fake a sparkline.
2. **Bilingual labels** EN + 简体中文 on axes, legends, titles.
3. **Abbreviations:** `Abbrev (Full English｜中文)` on first use in the chart caption.
4. **Claim class** under every chart: CONFIRMED / RELIABLE / INFERENCE / HYPOTHESIS / ILLUSTRATIVE.
5. **Source + as-of timestamp** in the caption.
6. **Thinking caption** (1–3 lines): What to observe → Why it matters → Falsifier or next watch.

## Required diagram types by deliverable｜按交付物的必做图

### A. Every major Event Book
| Diagram | 中文 | When |
|---------|------|------|
| Transmission Chain | 传导链 | Macro/central bank/company material events |
| Expectation Gap | 预期差 | Pre vs Actual |
| Scenario Probability | 情景概率 | Bull/Base/Bear (or 5-way) |
| Reaction Decomposition | 反应分解 | ΔEPS vs ΔMultiple vs Positioning vs Liquidity (conceptual if numbers incomplete) |
| Thinking Tutorial flow | 思维教程流 | Mandatory teaching panel |

### B. Daily Board / AI Factory tape
| Chart | Notes |
|-------|-------|
| Index strip | Verified closes only |
| Watchlist movers | Top ± names with claim class |
| Rates / FX / Oil / VIX strip | Mark N/A gaps |
| Next-catalyst timeline | CONFIRMED vs TENTATIVE |

### C. Company packs (when material)
Revenue/margin bridge, KPI traffic lights, SOTP tree, CapEx→bottleneck map (AI chain).

## Formats｜格式
1. **Mermaid** in markdown Event Books (portable, versionable).
2. **SVG / HTML cards** in Daily Board and showcase (premium look).
3. **PNG export** when sharing externally (from HTML/SVG; never invent pixels).
4. Prefer `research-os/charts/exports/YYYY-MM-DD-*.svg|png` for reusable assets.

## Anti-patterns｜禁止
- Animation with no economic meaning
- Charts that imply precision the data does not have
- Mixing unverified broker “targets” into valuation charts without labeling HYPOTHESIS
- Cloning tip-sheet stock-pick aesthetics without Expectation Gap / claim classes

## Folder
- Templates: `research-os/charts/templates/`
- Exports: `research-os/charts/exports/`
- Event-local: `research-os/events/<event>/charts/`
