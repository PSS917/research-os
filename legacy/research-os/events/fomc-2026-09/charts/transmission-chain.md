# FOMC Sep 2026 — Transmission Chain Diagram｜传导链图示
**As-of:** 2026-09-17  
**Claim class:** CONFIRMED (decision/SEP) + RELIABLE (tape) + INFERENCE (links)  
**Sources:** Fed statement/SEP; Post-Mortem pack under `events/fomc-2026-09/`

```mermaid
flowchart LR
  Oil["Oil / Mid-East<br/>油价/中东<br/>RELIABLE"] --> Inf["Inflation narrative<br/>通胀叙事"]
  Inf --> Fed["FOMC +25bp to 3.75–4.00%<br/>12–0 CONFIRMED"]
  Fed --> SEP["SEP FF 4.1% / 4.1%<br/>更高更久 CONFIRMED"]
  SEP --> Path["Policy path > decision<br/>路径 > 决议"]
  Path --> Y["10Y ~5% / real yields<br/>长端/实际利率 RELIABLE"]
  Y --> WACC["WACC / discount rate ↑<br/>资本成本 INFERENCE"]
  WACC --> Mult["Long-duration multiples<br/>长久期倍数"]
  Mult --> Names["NVDA MU ARM LITE MRVL<br/>AVGO CRWV TSLA SPCX"]
  Fed --> Tone["Warsh press: conditions<br/>not restrictive RELIABLE"]
  Tone --> Fade["Bid then fade<br/>先涨后回落 RELIABLE"]
```

**Thinking caption｜思维说明**
- Observe: path/SEP/dots, not only the 25 bp binary.｜盯路径与点阵，不只盯加息 25bp。
- Why: binary was ~92–93% priced; residual = higher-for-longer WACC.｜二元已定价；残差是更高更久贴现率。
- Alternative: oil/term-premium alone can move 10Y without a hawkish SEP.｜备选：油价/期限溢价也可推高 10Y。
- Falsifier: 10Y falls & AI multiples expand while SEP path still “sticky.”｜证伪：SEP 仍紧但 10Y 下行且 AI 倍数扩张。
- Next: BOJ Fri Sep 18 USDJPY/carry; MU Sep 30.｜下一步：周五日银；美光 9/30。
