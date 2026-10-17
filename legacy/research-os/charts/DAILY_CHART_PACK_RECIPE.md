# Daily Chart Pack Recipe｜日报图表包配方
Used by AI Factory Morning / Afternoon / Evening routines.

## Output
For each session run, create folder:
`/home/box/investment/research-os/charts/exports/YYYY-MM-DD-<session>/`

Session tags: `morning` | `afternoon` | `evening`

Minimum files:
1. `transmission.md` — Mermaid transmission chain for the dominant material theme that session (or "no material chain" stub if quiet).
2. `expectation-gap.md` — if a major event is in lifecycle; else skip with note.
3. `catalyst-timeline.md` — next CONFIRMED/TENTATIVE catalysts (7-day).
4. `board-notes.md` — 5–10 line bilingual caption for Daily Board refresh.
5. Optionally refresh/copy HTML board from template if enough verified prints exist:
   `/home/box/investment/research-os/dashboard/boards/YYYY-MM-DD-<session>-board.html`

## Rules
Follow `CHARTING_STANDARD.md`. No invented prices. SPCX = Nasdaq-listed SpaceX. Bilingual. Claim classes. Thinking captions.
If No Material Information for charts beyond tape strip, still produce catalyst-timeline only and stay quiet on extra alerts.
