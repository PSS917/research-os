# 研究体系审核 System Review & Audit — v20261015-0757
> 回答你在第10点提出的审核问题。生成于 2026-10-15 08:02 SGT。

## 1. 研究范围是否正确？遗漏模块 Scope gaps
已覆盖: 宏观政策、利率、通胀、就业、流动性、套息、跨资产、AI供应链、台日韩雷达、27家个股、事件生命周期。
**建议新增 (缺口)**:
1. **信用与私募信贷 Private credit / AI 融资链**: CRWV、Oracle、数据中心ABS/项目债——AI Capex 越来越依赖债务，是反身性风险源。
2. **财政与国债供给 Fiscal & Treasury supply**: 再融资季度公告(QRA)、拍卖尾差、期限溢价——10Y 已在5%以上，此项对估值影响大。
3. **中国变量 China**: 出口管制、稀土/镓锗、国产替代(CXMT/华为昇腾)、中国需求。
4. **能源/电力价格**: 天然气、PJM容量价格、核电/SMR、变压器交期——AI电力瓶颈的价格信号。
5. **持仓/资金面数据源**: CFTC COT、EPFR流向、期权偏度/Gamma、卖空比例——v1 未接入，因此"机构定位"只给框架不下结论。
6. **元器件价格源**: DRAM/NAND合约价与现货价(TrendForce/DRAMeXchange)、光模块与EML价格、ABF/CCL价格——需付费或手工录入。

## 2. 是否扩展观察名单 Watchlist expansion (建议，非必须)
- AI 网络/互连: ANET, CRDO, ALAB, FN (Fabrinet), APH (Amphenol)
- 存储: SNDK, WDC, STX；HBM 设备: 韩美(042700.KS, 已在雷达)
- 半导体设备/EDA: LRCX, ASML, CDNS, SNPS, TER (测试)
- 电力/散热: VRT (Vertiv), GEV (GE Vernova), ETN, CEG/VST (电力)
- 云/AI 平台: MSFT, GOOGL, AMZN, META, ORCL (资本开支来源——Capex 指引是整个AI链的上游信号)
- 自动驾驶: UBER, WAYMO(未上市, 通过GOOGL), MBLY
优先级建议: 先加 **云厂4家+ORCL** (Capex源头) 与 **VRT/GEV/ANET/LRCX/ASML**。

## 3. 台日韩题材分类是否细到技术/制程/产品
v1 采用 L1 题材 (如 Optical 光通信) + L2 技术/产品 (如 InP 磊晶、EML、CPO、ABF 载板、高速CCL M8/M9、TC Bonder、HBM测试)。共 48 档标的。
**下一步**: 增加 L3 制程/规格 (例如 CoWoS-S/L/R、HBM3E 12-Hi vs HBM4、800G vs 1.6T、M8 vs M9 CCL)，并对每档标注"美股锚点"(read-across)。每月复核成分。

## 4. 个股报告: 更好的财务/估值分析
- 已有: 10年DCF三情景、反向DCF、ROIC-WACC、2/4/6/8季度检验、同业、敏感度。
- **改进**: (a) 分部SOTP——需从10-K录入分部收入(v1留空以免编造)；(b) 按行业换主估值法: 存储/设备用周期中值P/B与EV/EBITDA；软件用EV/NTM收入 vs 增速(Rule of 40)；CRWV用合约积压折现+资产回收；SPCX/RKLB用分部+期权；(c) EPS桥(收入×毛利×费用×股本)而非仅FCF；(d) 管理层指引录入与"指引可信度"历史评分；(e) 一致预期修正动量(eps_trend 已抓取，下一版纳入图)。
- 注意: v1 的统一假设 (ERP 5%、β夹在0.8–1.6、长期FCF率按框架) 对高成长股给出偏低的Base价值；这正是用反向DCF呈现"价格隐含了什么"的原因，不应读作目标价。

## 5. 三情景与Excel公式可审计性
- 每个模型 ~2,400 条实时公式；黄色=假设、蓝色=数据；Sources 与 Assumptions 表逐项列出来源/理由。
- 自动核验: LibreOffice 重算结果与 Python 镜像逐一比对 (容差1e-4)。本次结果见下表 `xlsx_recalc_match`。
- 待改进: 情景概率目前固定 25/50/25 (ASSUMPTION)；下一版应按证据调整并记录调整理由。

## 6. 初学者教学是否足够
每个个股/宏观有独立中英文教学版，遵循九步阶梯 + 自测题。不足: 例题目前以DCF为主；下一版每次事件后加入"本次事件的例题"(如CPI超预期0.1pp → 2Y 变动 → 成长股估值影响)。

## 7. 图片报告结构完整性
每家公司5张 2400×1350 PNG + JPG: ①股价vs三情景 ②季度财务 ③三情景 ④2/4/6/8季度检验 ⑤研究逻辑图；每张含声明类别、来源、思考提示。宏观5张、雷达3张、日报2张。不足: 尚无供应链地图与KPI红绿灯图 (需结构化KPI数据)。

## 8. 历史版本与全部文件能否真正打开 (实测)
| 检查项 | 通过 | 失败 |
|---|---|---|
| pdf | 343 | 0 |
| docx | 338 | 0 |
| zip | 247 | 0 |
| html_links | 16840 | 0 |
| xlsx_recalc_match | 108 | 0 |
| png_hd>=2000px | 943 | 109 |
方法: pdfinfo 解析每个PDF；python-docx 打开每个DOCX；openpyxl 读取 + LibreOffice 重算每个XLSX；zipfile.testzip 校验每个ZIP；解析每个HTML的本地链接是否存在；检查PNG分辨率。旧档案(9月)以原样复制到 legacy/ 可浏览。

## 9. 更新频率矩阵 Update cadence
| 模块 | 每日 | 每周 | 每月 | 每次财报/事件 |
|---|---|---|---|---|
| Dashboard / 行情 / 异动 | ✔ | | | |
| 宏观跨资产 | ✔快照 | ✔专题 | ✔深度 | ✔数据发布 |
| 台日韩雷达 | ✔ | ✔排名 | ✔分类复核 | |
| 事件日历 | ✔ | | | ✔ |
| 个股估值快照 | ✔(价格) | | | |
| 个股深度(假设) | | | ✔轻更新 | ✔完整重跑 |
| Excel模型 | ✔输入 | | | ✔假设 |
| 产业链(AI Capex/HBM/光/电力) | | ✔ | ✔ | ✔云厂Capex |
| 专题(Robotaxi/AI生产率) | | | ✔ | ✔重大法规 |
| Master Prompt | | | 视需要 | 重大升级 |

## English summary
Scope gaps: private credit/AI financing, fiscal/Treasury supply, China, power prices, positioning feeds, component price feeds. Suggested adds: MSFT/GOOGL/AMZN/META/ORCL (capex source), VRT, GEV, ANET, LRCX, ASML. Radar is L1 theme + L2 technology/product; add L3 process/spec. Valuation upgrades: segment SOTP inputs, sector-appropriate primary methods, EPS bridge, guidance-credibility scoring, revision momentum. Excel: ~2,400 live formulas per model, recalculation verified against Python mirror. File-open tests shown above.
