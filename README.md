# Workforce Engagement Metrics (Work in Progress)

This project builds **workforce planning guardrails** implemented as **data checks and alerts** to help managers spot risks early and keep operations on track. 
The goal is to create **early-warning KPIs** that highlight problems like understaffing, unfair scheduling, burnout risk, or declining employee engagement **before they impact employees or customers**.

Each notebook contains **analyst-style prompts** with space for code answers, demonstrating how data can be used to:
- Validate data quality and scheduling accuracy
- Compare forecast demand vs. actual staffing
- Monitor fairness in shift distribution and weekly workload
- Track engagement trends using ADKAR and eNPS survey data
- Connect staffing gaps to customer experience outcomes (CSAT)

This is a **work-in-progress portfolio project** answers will be added incrementally. 
The repo is structured so each section can stand alone but also builds into a full workforce analytics story.

## Notebooks
1. `01_data_quality.ipynb` — missing values, duplicate shifts, hours vs FTE.
2. `02_coverage_vs_demand.ipynb` forecast vs staffed, gaps, store ranking.
3. `03_fairness_volatility.ipynb` close-shift share, weekly volatility, histograms.
4. `04_engagement_adkar.ipynb` — ADKAR averages, adoption trends, intent-to-leave.
5. `05_customer_impact.ipynb` — CSAT vs understaffing, simple hypothesis test.

## Data (cleaned)
Sample CSVs live in `./data/`:
- `employees.csv`, `schedule.csv`, `demand_forecast.csv`
- `survey.csv` (ADKAR + eNPS + intent_to_leave)
- `csat.csv`


## How to run
```bash
pip install pandas numpy matplotlib scipy
# then open notebooks in Jupyter / VSCode and run cells in order
```

## Future Work
- Expand fairness (rotation rules, rest windows) and burnout risk.
- Add forecasting (ARIMA/Prophet) for labour demand.
- Turn plots into a small **dashboard** (Power BI / Looker / Streamlit).
- Add unit tests and data-quality checks (e.g., Great Expectations).

## Status
Work in progress — answers will be committed incrementally.
