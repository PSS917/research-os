# CHANGELOG v20261015-2156-post — US Retail Sales (Sep 2026) post-event
- 2026-10-15 21:56 SGT: post-event book built by pipeline/build_post_macro.py from locked v20261015-1805 (integrity checked, not rewritten).
- Actual: Census MARTS advance (CB26-165) Table 1 SA levels via FRED; control group = total − autos(441) − gas(447) − building(444) − food services(722), OS-calculated.
- Market snapshot intraday 09:57 ET; Kalshi 2026-10-15 21:56 SGT.
- Classification (locked rule) strong; quality bucket inline; Brier OS/base/uniform 1.005/0.724/0.667.
- Close-of-day rebuild: `python3 pipeline/build_post_macro.py --event us-retail-2026-09 --close-check`.
