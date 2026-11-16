# Breathing Room Budget workbook (lives in this repo, replaces the Google Sheet)

Everything the weekly tasks need is here, so nothing has to be found elsewhere.

- `weekly-content.csv` — one row per post. Columns: date, platform, format, pillar, hook, caption, cta, product, canva_link, canva_design_id, repo_folder, status, buffer_post_id, sources.
- `roadmap.md`, `lessons.md`, `audit-log.md`, `approvals.md`, `toolkit.md`, `metrics.csv` — the other tabs from the old sheet.

## Status values
`Planned` (date reserved, no content yet) -> `Draft` -> `Ready to post` (Reviewer agent passed it) -> `Scheduled` (in Buffer, buffer_post_id filled) -> `Posted`.
Bob pre-approved everything the content task makes (Nov 16, 2026), so `Ready to post` and `Approved` rows both get scheduled by the scheduler task.

## Standing rules
- CTAs point to the free "Your First $1,000" kit (link in bio) until Bob says otherwise. No prices in captions.
- Never use the "Comment ROOM" keyword.
- Every caption ends with "Educational only, not financial advice."
- Image folders: `week-YYYY-MM-DD/day-NN/slide-NN.png` + `manifest.json` (see top-level README). Week 1 is `week-2026-11-16`, Week 2 is `week-2026-11-16-b`, Week 3 is `week-2026-11-23`.
- Edit this CSV with a script (python csv module) so quoting stays valid, then commit and push to main.
