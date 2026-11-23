# DRC GC8 LLIN Campaign Milestone Tracker (demonstration)

> **Demonstration data.** The milestone statuses in this dashboard are made up to show how the tracker works. They do not report real campaign progress.

A one-page dashboard showing planned milestones for the 11 DRC provinces with GC8 mass LLIN/ITN campaigns scheduled in 2027–2028. It can be filtered by region (the pre-2015 provinces), province, campaign stage and milestone status.

**View it:** open `index.html` in a browser, or use the GitHub Pages site for this repository.

**Languages:** the page opens in French by default. Use the **FR | EN** switch at the top right to change language; the choice is remembered in that browser. You can also link straight to a language with `?lang=en` or `?lang=fr`. All page text is in the `T` block of `index.html` (French and English side by side), and milestone names in the `MILESTONES` block.

## What's in it
- `index.html`: the dashboard. It's self-contained, and all data is in the `DATA` block at the top of the script.
- `milestones_template.csv`: the 15 milestones and when each is due, counted in days before or after the planned distribution date.
- `assets/path-logo-primary-color.svg`: PATH logo.

## Updating with real progress data
1. Fill in the **DRC GC8 LLIN Milestone Update Sheet**: set Status (Not started / In progress / Done) and the actual completion date for each milestone. Planned due dates are worked out from the distribution dates on its Provinces tab and the offsets on its Milestones tab.
2. Open the sheet's **Milestone status** tab and download it as CSV.
3. Rename the file to `milestone_status.csv` and upload it to the `data/` folder of this repo (Add file → Upload files), replacing any old copy.
4. Fill in **Last updated** on each row you change. Each province's last update on the dashboard is the most recent of these dates; provinces with no update in 30 days (or none at all) are flagged in red.
5. The dashboard reads it automatically. A milestone is shown as **Late** when its planned date has passed and it isn't marked Done. While `data/milestone_status.csv` is missing, the dashboard shows demonstration data.

## Data and assumptions
- Planned distribution dates, last campaign dates and province indicators come from the *DRC Malaria ITN Campaign Planning* note V1 (GC8 schedule; 2025 Coverage Survey, Kinshasa School of Public Health). RDT prevalence values are approximate.
- Milestone due dates = planned distribution date + offset. The net order offset (−241 days) is the note's average time from order to distribution. The other offsets are typical planning lead times for mass campaigns and still need to be checked with the NMCP.
- Regions group the current provinces by the provinces that existed before 2015 (Orientale, Bandundu, Équateur, Kasaï-Occidental, Bas-Congo, Maniema).
- Without `data/milestone_status.csv`, statuses are generated for the demo, with 20 Nov 2026 as the "as of" date.

PATH / MACEPA
