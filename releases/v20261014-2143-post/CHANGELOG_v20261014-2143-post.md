# Changelog v20261014-2143-post
- Generated 2026-10-14 21:44 MYT. US CPI (Sep 2026) post-event review, built from LOCKED pre-event book v20261013-1803 (sha256 35/35 verified, not modified).
- Actual (BLS API): headline +0.6% m/m / 3.7% y/y; core +0.3% (0.335) / 2.6%. Class HOT. Market data = intraday snapshot (≈09:15–09:43 ET), close review pending.
- New: enriched post-event book (chain post-mortem, components, T+45 cross-asset, Kalshi, scenario check, A1–A5, calibration/Brier, steelman, watchlist, watch-next) + news-explainer infographic us-cpi-sep2026-hot v20261014-2140-news (2 pages PNG/JPG/PDF/HTML).
- Superseded same-day thin build v20261014-2131-post (kept, never overwritten).
- Pipeline fixes: publish_pages.sh makes pages_build writable (read-only locked files broke offload.py link rewrite); build_post_event.py --extra/--images + intraday labelling; events.html now lists Event Books.
