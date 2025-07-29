# Time_Series_Forecasting_Weekly_Visits
Forecasting Weekly Website Traffic &amp; Conversion Rates to Supercharge Seasonal Campaigns using time series modeling which anaylzes and forecasts future trends in terms of visits and conversions.

 My Data‑Driven Approach
Data Prep:
  • 156 weeks of site visits & conversions, indexed by week_start_date
Baseline ARIMA:
  • Fitted ARIMA(1,1,1) → captured short‑term patterns but missed annual cycles
Seasonal SARIMAX Upgrade:
  • Implemented SARIMAX(1,1,1)(0,1,1,52) to explicitly model weekly and yearly seasonality (seasonal_order=(0,1,1,52))
True Hold‑out Test:
  • Reserved the last 13 weeks as a “future” test set (mirroring quarterly planning)
  • Evaluated forecasts with MAPE (Mean Absolute Percentage Error)

Standout Results
• Weekly Visits MAPE: ARIMA → 11.0 % | SARIMAX → 3.2 %
• Conversion Rate MAPE: ARIMA → 14.2 % | SARIMAX → 9.5 %

Key Takeaways
Seasonality matters: Off‑the‑shelf ARIMA misses annual cycles—SARIMAX nails them with seasonal_order=(0,1,1,52).
Align to business needs: A 13‑week hold‑out mirrors real‑world quarterly planning.
Automate & empower: Embedding these forecasts in Power BI dashboards gives teams the agility to pivot the moment trends shift.
