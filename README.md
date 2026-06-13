# TrackSmart AI — Performance Reports

This repository hosts client performance reports for TrackSmart AI, served at
**reports.tracksmartracing.com**.

## What's in here

- `index.html` — the landing page (the directory of all reports). Served as the
  homepage automatically.
- One `.html` file per client report (e.g. `alexander-bosse.html`).

## Posting a new report

1. Add the new report's `.html` file to this repo (root level), next to
   `index.html`.
2. Open `index.html`, find the block marked **"ADD A NEW REPORT HERE"** near the
   bottom, and paste a new line at the top of the list:

   ```js
   { client:"Jane Smith", desc:"5 cards · Jul 4, 2026",
     stat:"79%", statLabel:"Top-4 hit rate", file:"jane-smith.html" },
   ```

   - `client` — customer name
   - `desc` — short summary (cards, date range)
   - `stat` — the headline number on the right (use `""` to hide it)
   - `statLabel` — tiny caption under the stat
   - `file` — the report's filename in this repo

3. Commit. The new entry appears on the landing page automatically. Newest goes
   on top.

## Notes

- Filenames are case-sensitive: `alexander-bosse.html`, lowercase, hyphens.
- This repo is public — anyone with a filename can open a report directly.
- The report each line points to must exist in the repo, or the link will 404.
