### 🛢️ Oil & Water Production Forecasting & Analytics

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Libraries](https://img.shields.io/badge/Libraries-pandas%2C%20XGBoost%2C%20scikit--learn-orange)

A comprehensive machine-learning pipeline and interactive notebook for analyzing and forecasting production dynamics in mature wells (Volve field), with actionable insights for operational optimization and risk-aware planning.


## 📋 Project Overview

This Jupyter Notebook implements a structured, end-to-end workflow to:

1. **Ingest & Clean** raw Volve field production data  
2. **Engineer** advanced time-series features (rolling means, lags)  
3. **Train & Compare** multiple models:  
   - **XGBoost** (oil rate)  
   - **Linear Regression** (water rate)  
   - **Decision Tree & Random Forest** (oil rate benchmarking)  
4. **Quantify Uncertainty** via bootstrapped 90 % confidence intervals  
5. **Simulate Scenarios** (e.g. choke‐size adjustments)  
6. **Forecast** 180-day rates and cumulative volumes  
7. **Export** results for downstream reporting



## 🔑 Key Features

- **Time-series anomaly handling** & outlier capping  
- **Feature engineering**: rolling averages, multi-horizon lags  
- **Model performance comparison** (MAE, R²) across algorithms  
- **Bootstrapped CI** for robust uncertainty estimates  
- **Scenario analysis**: operational lever (choke size) sensitivity  
- **Cumulative volume projection** for economic cut-off evaluation  



### Install dependencies:
- pip install -r requirements.txt 
- (Create requirements.txt with: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, missingno, plotly-express)


## 📊 Usage

- Place the dataset `Volve production data.xlsx` in the project directory.

- Run the Jupyter Notebook

- Key sections:
    1. **Imports & Config**
    2. **Data Preprocessing (load_and_preprocess())**
    3. **Feature Engineering (engineer_features())**
    4. **Model Training & Evaluation (ProductionForecaster and comparative models)**
    5. **Forecast Generation (generate_forecast() + CI plotting)**
    6. **Scenario Simulation (simulate_choke_scenarios())**
    7. **Cumulative Volume Forecast & Export**



## 📈 Highlights & Results

- Oil decline trends captured with R² > 0.85 (XGBoost)
- Water rate forecasts with R² ≈ 0.70 (Linear Regression)
- Decision Tree & Random Forest models benchmarked via MAE/R² bar charts
- 90 % CI bands reveal forecast uncertainty for both oil and water
- Choke-size scenarios demonstrate production sensitivity to valve settings
- 180-day cumulative volumes inform economic cut-off and water-handling planning

## 🌟 Visualizations

- Time-series plots: oil vs. water rates
- Correlation heatmaps & pairplots for feature insights
- Model comparison charts (MAE, R²)
- Forecast vs. historical overlays with CI shading
- Scenario curves under different choke configurations
- Cumulative volume trajectories for next 180 days

## 🤝 Contributing
Contributions are welcome! Open an issue or submit a PR for:
- Enhanced water rate modeling (e.g., LSTM).
- Dynamic reservoir coupling for choke sensitivity.
- Code optimizations.

## 📧 Contact
For questions or feedback, feel free to reach out:

<p align="center"> <strong>📬 Let’s Connect!</strong> <br> <a href="https://www.linkedin.com/in/rishikesh-borah-3b245284/" target="_blank" style="display: inline-block; background-color: #0077B5; color: #fff; padding: 8px 16px; margin: 5px 10px; text-decoration: none; border-radius: 4px;">LinkedIn</a> | <a href="mailto:rishikesh.borah4@gmail.com" target="_blank" style="display: inline-block; background-color: #D44638; color: #fff; padding: 8px 16px; margin: 5px 10px; text-decoration: none; border-radius: 4px;">Email</a> </p>




