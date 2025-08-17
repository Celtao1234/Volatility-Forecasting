# Volatility Forecasting & Option Pricing on Gold ETF

📊**Independent Quant Research Project**  
This project implements volatility forecasting models and applies them to option pricing of **SPDR Gold ETF (GLD)**.  
It combines econometrics and machine learning with practical options pricing models.

---

##  Project Workflow

1. **Data Collection & Preprocessing**
   - Historical GLD prices from Yahoo Finance.
   - Computed daily log returns:
     \[
     r_t = \ln\!\left(\tfrac{P_t}{P_{t-1}}\right)
     \]

2. **Volatility Forecasting**
   - Models:
     - Naïve (Squared Returns)
     - Rolling Average
     - GARCH(1,1)
     - Random Forest
     - XGBoost
     - LSTM
   - Evaluated with **RMSE, MAE, $R^2$**.

3. **Options Pricing**
   - Forecasted volatility plugged into **Black–Scholes** model.
   - Call prices computed for maturities: **Sep 2025, Nov 2025, Feb 2026**.

---

## Results (Highlights)

- **Volatility Forecasting**
  - LSTM and XGBoost achieved superior accuracy (lower RMSE/MAE, higher $R^2$).
  - Classical GARCH benchmark included.

- **Options Pricing**
  - Forecasted volatilities led to diverse option valuations across models.
  - Pricing table compares call values from each method.

---



