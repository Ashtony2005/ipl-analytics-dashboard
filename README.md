# IPL Performance Analytics Dashboard
**Tools:** Python (Pandas) · Tableau · Microsoft Excel
**Data:** 636 matches · 150,460 ball-by-ball deliveries · 2008–2017

## Live Dashboard
[View on Tableau Public →]((https://public.tableau.com/app/profile/ashton.yesudasan/viz/Book1_17769292326330/Dashboard1#1))

## Project Overview
An end-to-end data analytics project built on IPL match and
delivery data. Cleaned and aggregated raw data using Python,
then built an interactive 5-view Tableau dashboard to surface
player performance insights and team win patterns.

## Key Findings
- Toss outcome predicted match result only ~52% of the time
  across all seasons — barely better than a coin flip
- SP Narine and R Ashwin are the most economical high-wicket
  bowlers in the dataset (economy under 7, 100+ wickets)
- Elite batters cluster in the top-right quadrant of the
  strike rate vs batting average scatter — high on both axes

## File Structure
| File | Description |
|------|-------------|
| clean_deliveries.py | Python script — cleans deliveries.csv and produces all summary CSVs |
| batting_summary.csv | Aggregated batting stats per player (200+ balls faced) |
| bowling_summary.csv | Aggregated bowling stats per bowler (300+ balls bowled) |
| season_totals.csv | Total runs, wickets, fours, sixes per season |
| team_season_stats.csv | Win %, wins, losses per team per season |
| matches_clean_csv.csv | Cleaned match-level data with toss outcome column |

## How to Run the Cleaning Script
```bash
# Place deliveries.csv and matches_clean_csv.csv in the same folder
pip install pandas
python clean_deliveries.py
```
This produces all 4 summary CSV files used in the Tableau dashboard.

## Dashboard Views
1. **Team Wins Bar Chart** — total wins per franchise with average reference line
2. **Season Trend** — dual-axis combo chart of runs and wickets per season
3. **Player Value Scatter** — strike rate vs batting average, sized by total runs
4. **Win % Heatmap** — team win percentage by season with interactive filter
5. **Bowler Economy** — economy rate ranking with 7.0 benchmark line

---
*Built by Ashton Yesudasan · B.Tech Computer Engineering · NMIMS Navi Mumbai*
*[LinkedIn](https://www.linkedin.com/in/ashtonyesudasan17/) · [Tableau Public](https://public.tableau.com/app/profile/ashton.yesudasan/viz/Book1_17769292326330/Dashboard1#1)*
