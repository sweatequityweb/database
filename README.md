# Ugnayan Gulayan / Sweat Equity Portal

A static site for GitHub Pages. No backend, no build step. All data lives in the Excel files in `data/`.

## Publishing
1. Put everything in this folder at the **root** of the repository (keep `.nojekyll`).
2. Repo **Settings > Pages**: deploy from the `main` branch, `/ (root)`.

## Updating data (non-technical staff)
1. Open the repo on GitHub, go into the `data` folder.
2. **Add file > Upload files**, drop in the updated Excel file. **Keep the exact same file name** and keep the column headers and sheet name.
3. Commit. The site shows new data after GitHub Pages redeploys (usually a minute or two).

Tips
- Dates: either Excel dates or text like `2026-10-21` both work.
- Fund expenses can be entered as positive numbers; the site subtracts them.
- Attendance: enter total points per household (Work Day = 8, Care Slot = 4). Put `Solo Parent` or `OFW` in *Hardship Adjustment* for the 90-point target.
- If a file is missing or broken, the page shows a yellow warning banner and an offline fallback.
- The files in `data/` currently contain SAMPLE rows. Replace them with your real data.

## Roles (people.xlsx > Role)
Staff (all modules): committee, liaison, coordinator, documentation, treasurer, logistics, shift_lead.
Parent / student (Hub, Farm Points, Sweat Equity only). Any unrecognised role is treated as parent.
Parents and students are matched to their records by **Household ID**.
