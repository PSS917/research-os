# PLTR 初学者教学版 (中文) v20261017-0755
## ① 一句话
Palantir Technologies Inc. 是一家 AI software platform AI软件平台 公司。现在股价 $186.03。我们的Base模型认为每股价值约 $69（-63.2%）。

## ② 发生了什么
最近一季财报EPS实际 vs 预期: ['2026-06-30', '0.41', '0.34596', '0.1851']（实际、预期、超预期%）。下次财报约 2026-11-03。

## ③ 术语 Glossary
- DCF (Discounted Cash Flow｜现金流折现): 把未来每年能拿到的现金，按"时间成本"折回今天加总。
- FCF (Free Cash Flow｜自由现金流) = 经营现金流 − 资本开支。
- WACC (Weighted Average Cost of Capital｜加权平均资本成本): 投资人要求的年回报率，用作折现率。
- Reverse DCF (反向DCF): 反过来问"现价要求公司增长多快"。
- Consensus (一致预期): 分析师预测的平均值。
- Falsifier (证伪指标): 一旦出现就说明论点错了的信号。

## ④ 生活比喻
买这家公司股票≈买一棵果树。DCF就是估算果树未来每年结多少果(FCF)，再考虑"明年的一斤果不如今天的一斤果值钱"(WACC折现)。

## ⑤ 因果箭头
AI software platform AI软件平台 需求 → 收入增长 (g) → 自由现金流 (FCF = 收入 × FCF率) → 折现 (÷(1+WACC)^t) → 每股价值 → 与股价比较 → 预期差

## ⑥ 数字例题（符号定义）
设 R₀ = 过去12个月收入 = 6.2 bn USD；g₁ = 第一年增速 = 50.1%；m = 长期FCF率 = 45.0%；W = WACC = 13.1%。
第一年收入 R₁ = R₀ × (1+g₁) = 9.2 bn USD。
若第5年FCF率达到 m，则第1年FCF ≈ R₁ × m₁（m₁ 由当前 54.6% 向 45.0% 线性过渡）= 4.9 bn USD；
折现到今天: FCF₁ ÷ (1+W)¹ = 4.3 bn USD。十年加总 + 终值 = EV 155.5 bn USD。

## ⑦ 事实 / 预测 / 市场预期
- 事实: 过去财务数据(第4节)、现价。
- 预测(我们的假设): 长期FCF率 45.0%、三情景。
- 市场预期: 一致预期增速 50.1%；价格隐含增速 83.3%。

## ⑧ 三情景
Bear $24 / Base $69 / Bull $138；概率加权 $75。

## ⑨ 反方观点与失效条件
反方: Multiple compression; gov budget delays (shutdown/CR); competition｜估值压缩；政府预算延迟；竞争
失效条件: US commercial growth decelerates sharply; net dollar retention falls; RPO stalls｜美国商业增速骤降；净留存率下降；RPO停滞

## 自我检验题
1. 如果WACC上升1个百分点，价值会升还是降？为什么？（提示：分母变大）
2. 反向DCF隐含增速高于一致预期意味着什么？


---

# PLTR Beginner Teaching Edition (English) v20261017-0755
## ① In one line
Palantir Technologies Inc. is a AI software platform AI软件平台 company. Price $186.03; our Base model value ≈ $69 (-63.2%).
## ② What happened
Last quarter EPS actual vs consensus: ['2026-06-30', '0.41', '0.34596', '0.1851']. Next earnings ≈ 2026-11-03 (TENTATIVE).
## ③ Glossary
DCF (Discounted Cash Flow｜现金流折现); FCF (Free Cash Flow｜自由现金流) = operating cash flow − capex; WACC (Weighted Average Cost of Capital｜加权平均资本成本) = the yearly return investors demand; Reverse DCF (反向DCF) = what growth the price requires; Consensus (一致预期); Falsifier (证伪指标).
## ④ Analogy
Owning the stock ≈ owning a fruit tree: DCF estimates future fruit (FCF) and discounts it because fruit next year is worth less than fruit today.
## ⑤ Causal arrows
Demand → revenue growth (g) → FCF (= revenue × FCF margin) → discounting ÷(1+WACC)^t → value/share → compare with price → expectation gap
## ⑥ Worked example (symbols)
R₀ = TTM revenue = 6.2 bn USD; g₁ = 50.1%; m = long-run FCF margin = 45.0%; W = 13.1%.
R₁ = R₀×(1+g₁) = 9.2 bn USD; FCF₁ = 4.9 bn USD; PV = FCF₁/(1+W) = 4.3 bn USD; 10 years + terminal → EV 155.5 bn USD.
## ⑦ Fact vs forecast vs market expectation
Facts: reported financials, price. Forecast: our margin/scenario assumptions. Market: consensus growth 50.1%; price-implied growth 83.3%.
## ⑧ Three scenarios
Bear $24 / Base $69 / Bull $138; weighted $75.
## ⑨ Counterview & failure conditions
Multiple compression; gov budget delays (shutdown/CR); competition｜估值压缩；政府预算延迟；竞争 — Falsifiers: US commercial growth decelerates sharply; net dollar retention falls; RPO stalls｜美国商业增速骤降；净留存率下降；RPO停滞
## Self-check
1. WACC +1pp → value up or down? 2. What does price-implied growth > consensus mean?


![logic](images/PLTR_5_logic_map.png)
