# Model Evolution — SPCX Listing Status Correction
# 模型进化 — SPCX 上市状态纠正

**Date:** 2026-09-17 MYT  
**Trigger:** User challenge — "SPCX is already listed on US"  
**Class:** Fact / coverage-status error (not a forecast miss)

## What we wrongly believed
SPCX was marked **private / proxy only / no public print** across watchlist, CURRENT_STATE, daily AI Factory reports, FOMC materials, and the Daily Board.

## Evidence that corrected it (CONFIRMED)
- Nasdaq Trader Data Technical News DTN2026-8: Space Exploration Technologies Corp. Class A to trade Nasdaq Global Select + Nasdaq Texas under **SPCX**, first trade **2026-06-12**.
- SEC 424B4 prospectus (CIK 0001181412): approved listing under symbol **SPCX**.
- SpaceX pricing announcement PDF: IPO priced 2026-06-11; trading expected 2026-06-12 under SPCX.

## Decision
**Promote corrected fact to Core Model:** SPCX is a **public US equity** in the Research OS universe. Stop proxy-only framing. Still require verified quotes for price cells (no invention).

## Living files updated
- `/home/box/investment/WATCHLIST.md`
- `/home/box/investment/research-os/companies/SPCX/CURRENT_STATE.md`
- `/home/box/investment/research-os/dashboard/boards/2026-09-16-post-fomc-board.html`

## Historical reports
Prior daily/evening reports that said "SPCX private" are left as **timestamped artifacts of the error** (no hindsight rewrite of whole tapes). Future reports must use the corrected status.

## Lesson
Listing status is a CONFIRMED-FACT check against exchange/SEC — never carry forward an unverified "private" assumption once the ticker is on the coverage list.
