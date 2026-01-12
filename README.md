# Automotive EBIT Margin Prediction (Orbis)

Predicting firm profitability (EBIT margin) using financial ratios and ML models in R (tidymodels).

## Files
- `monte_carlo_simulation_project.Rmd` – full analysis pipeline (data cleaning → feature engineering → modeling)
- `monte_carlo_simulation_report.pdf` – final project report
- `automotive_industry_orbis_data.xlsx` – raw dataset (Orbis export)

## Methods (high level)
- Reshaped wide financial statements into tidy format (long → wide)
- Engineered profitability & financial ratios (EBIT margin, revenue growth, leverage, liquidity, etc.)
- Time-aware split: train on years < latest, test on latest year
- Models compared: Linear Regression, Random Forest, XGBoost
- Tuning: cross-validation + random grid search
- Metrics: RMSE, MAE, R²
- Interpretation: variable importance + diagnostics plots

## How to run
### 1) Install packages
Run in R:
```r
source("requirements.R")
```

### 2) Knit the report

Open `monte_carlo_simulation_project.Rmd` in RStudio and click **Knit**.

The result is shown in `monte_carlo_simulation_result.pdf`.