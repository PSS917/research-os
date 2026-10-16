# CHANGELOG v20261015-2158-post — US PPI (Sep 2026) post-event
- 2026-10-15 21:58 SGT: post-event book built by pipeline/build_post_macro.py from locked v20261014-1806 (integrity checked, not rewritten).
- Actual: BLS public API v1: SA indexes for MoM (WPSFD4, WPSFD49104, WPSFD49116), NSA for YoY (WPUFD4…); * = NSA series (no SA published).
- Market snapshot intraday 09:59 ET; Kalshi 2026-10-15 21:58 SGT.
- Classification (locked rule) hot; quality bucket hot; Brier OS/base/uniform 0.875/1.261/0.667.
- Close-of-day rebuild: `python3 pipeline/build_post_macro.py --event us-ppi-2026-09 --close-check`.
