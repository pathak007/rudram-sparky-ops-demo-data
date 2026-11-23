# Sparky Ops demo data (synthetic)

Live data for the Sparky Ops Dashboard, a public Power BI demo by Zirrell, the data and AI arm of Rudram.

**Everything here is synthetic.** Tuart Line Electrical is a fictional Perth electrical contractor. No real customers, staff or businesses are represented. Suburb names and coordinates are public geography.

| Path | What it is |
|---|---|
| `data/electrical/*.csv` | The star schema Power BI reads (over raw.githubusercontent.com, no gateway) |
| `data/metrics.json` | Every dashboard figure recomputed in Python; the source for the weekly narrative |
| `data/reconciliation_report.txt` | The reconciliation rules (R1 to R7) and story checks from the latest run |

The data is generated once a day, at about 04:30 Perth time, by a private repo. A day is only published if every reconciliation rule passes, and history never changes once published: each run adds yesterday.
