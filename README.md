# DRC GC8 LLIN Campaign Milestone Tracker (demonstration)

> **Demonstration data.** The milestone statuses in this dashboard are made up to show how the tracker works. They do not report real campaign progress.

A one-page dashboard showing planned milestones for the 11 DRC provinces with GC8 mass LLIN/ITN campaigns scheduled in 2027–2028. It can be filtered by region (the pre-2015 provinces), province, campaign stage and milestone status.

**View it:** open `index.html` in a browser, or use the GitHub Pages site for this repository.

## What's in it
- `index.html`: the dashboard. It's self-contained, and all data is in the `DATA` block at the top of the script.
- `milestones_template.csv`: the 15 milestones and when each is due, counted in days before or after the planned distribution date.
- `assets/path-logo-primary-color.svg`: PATH logo.

## Data and assumptions
- Planned distribution dates, last campaign dates and province indicators come from the *DRC Malaria ITN Campaign Planning* note V1 (GC8 schedule; 2025 Coverage Survey, Kinshasa School of Public Health). RDT prevalence values are approximate.
- Milestone due dates = planned distribution date + offset. The net order offset (−241 days) is the note's average time from order to distribution. The other offsets are typical planning lead times for mass campaigns and still need to be checked with the NMCP.
- Regions group the current provinces by the provinces that existed before 2015 (Orientale, Bandundu, Équateur, Kasaï-Occidental, Bas-Congo, Maniema).
- Statuses are generated for the demo, with 20 Nov 2026 as the "as of" date. To use real data, replace `demoStatus()` with actual statuses.

PATH / MACEPA
