Advanced Forecasting Project  
Author: Nguyễn Đàm Phúc Anh  



Project Overview  
This project applies time series forecasting techniques to predict U.S. Retail Sales for Building Materials and Supplies Dealers. The data was taken from the U.S. Census Bureau  

The goal was to identify the most accurate, interpretable, and statistically valid model to support strategic business planning through within-sample (WS) and out-of-sample (OOS) forecasts.  

---
`Advanced Forecast Final Powerpoint Nguyen Dam Phuc Anh 24116258 ID 6.pptx` Final presentation summarizing methods, analysis, and results.
`Bài AvdForecast.RPF` R project file containing scripts for time series modeling, data processing, and visualizations.
---

##Dataset Summary  
- Source: U.S. Census Bureau  
- Variable: Retail Sales: Building Materials and Supplies Dealers  
- Period Covered: January 1992 – July 2025  
- Focus Window: July 2020 – July 2025  
- Forecast Horizon: 6-step WS forecast, 18-month OOS forecast  

The dataset captures long-term retail sales dynamics, post-COVID recovery, and cyclical behavior in the construction materials sector.  

---

##Methodology  

###Models Evaluated
1. Exponential Smoothing (ES) – Emphasizes recent trends; smooths randomness but underrepresents seasonality.  
2. Box–Jenkins (ARIMA) – Utilizes autoregressive and moving average terms for temporal dependency modeling.  
3. Metronome Model – Combines a quadratic trend with a five-month seasonal pattern, balancing trend and cyclical effects.  

###Evaluation Metrics
- RMSE (Root Mean Square Error)  
- MAE (Mean Absolute Error)  
- MAPE (Mean Absolute Percentage Error)  

---

## Results & Model Selection  
| Model | RMSE | MAE | MAPE | Notes |

| Exponential Smoothing | Moderate | Moderate | Moderate | Captures short-term trend only |
| Box–Jenkins (ARIMA) | Higher | Higher | Higher | Fails to capture structural shifts |
| Metronome Model | Lowest| Lowest | Lowest | Chosen model for forecasting |

Selected Model:Metronome Model  
Reason: Demonstrated superior accuracy, interpretability, and structural consistency across both WS and OOS forecasts.

---

##Key Findings  
- The forecast projects a short-term decline in sales between late 2025 and early 2027.  
- Businesses should prepare by optimizing inventory, production, and expenditures.  
- 95% prediction intervals indicate increasing uncertainty in long-term projections.  

---

##Insights & Skills Demonstrated  
| Skill | Application |
| Time Series Modeling | Implemented ES, ARIMA, and custom Metronome model |
| Econometric Forecasting | Conducted WS and OOS evaluations using real data |
| Statistical Testing | Used RMSE, MAE, and MAPE for model comparison |
| Data Visualization | Created trend, residual, and forecast plots in R |
| Analytical Reasoning | Interpreted forecast implications for strategic planning |

##How to Reproduce  
1. Open `Bài AvdForecast.RPF` in RStudio.  
2. Load the retail sales dataset.  
3. Run each forecasting model (ES, ARIMA, Metronome).  
4. Compare model performance using RMSE, MAE, and MAPE.  
5. Visualize WS and OOS forecasts using provided scripts.  

---

## 🧾 Citation  
> Nguyễn Đàm Phúc Anh (2025). Advanced Forecasting Project: U.S. Retail Sales Forecasting Analysis.

---

## 🌟 About the Author  
🎓 Nguyễn Đàm Phúc Anh — Financial analytics student with strong interests in quantitative modeling, econometrics, and data-driven decision-making.  
📍 Based in Vietnam | 💼 Open to opportunities in data analysis, forecasting, and financial modeling.  
---
