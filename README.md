# Oil Production Forecasting & Operational Insight

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Libraries](https://img.shields.io/badge/Libraries-pandas%2C%20XGBoost%2C%20scikit--learn-orange)

A machine learning-driven analysis and forecasting system for mature oil wells, focusing on production decline trends, water-cut behavior, and operational optimization.

## 📋 Project Overview
This Jupyter Notebook provides a data-driven workflow to:
- Analyze historical oil/water production trends for the **Volve field**.
- Forecast production rates for **180 days** using XGBoost (oil) and Linear Regression (water).
- Generate strategic insights for reservoir management and operational decision-making.

### Key Features
- **Time-series analysis** with anomaly detection and feature engineering.
- **Scenario-based simulations** (e.g., choke size adjustments).
- **Confidence intervals** via bootstrapping for uncertainty quantification.
- **Cumulative volume forecasts** and sensitivity analysis.

### Install dependencies:
- pip install -r requirements.txt
- (Create requirements.txt with: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, missingno)


## 📊 Usage

- Place the dataset `Volve production data.xlsx` in the project directory.

- Run the Jupyter Notebook

- Key sections:
  - **Data preprocessing (load_and_preprocess())**
  - **Feature engineering (engineer_features())**
  - **3Model training (ProductionForecaster())**
  - **Forecast generation (generate_forecast())**

## 📈 Results
- Declining oil production (R² > 0.85) and rising water rates (R² ~ 0.70).

- Forecasts with 90% confidence intervals for risk-aware decision-making.

- Strategic recommendations:

  - Optimize choke sizes for delayed water breakthrough.
  - Scale water-handling infrastructure.
  - Implement real-time surveillance.

## 🌟 Highlighted Visualizations
- Production rate trends over time.
- Correlation matrices for feature analysis.
- Scenario-based forecasts under varying choke settings.

## 🤝 Contributing
Contributions are welcome! Open an issue or submit a PR for:
- Enhanced water rate modeling (e.g., LSTM).
- Dynamic reservoir coupling for choke sensitivity.
- Code optimizations.

## 📧 Contact
For questions or feedback, feel free to reach out:

<p align="center"> <strong>📬 Let’s Connect!</strong> <br> <a href="https://www.linkedin.com/in/rishikesh-borah-3b245284/" target="_blank" style="display: inline-block; background-color: #0077B5; color: #fff; padding: 8px 16px; margin: 5px 10px; text-decoration: none; border-radius: 4px;">LinkedIn</a> | <a href="mailto:rishikesh.borah4@gmail.com" target="_blank" style="display: inline-block; background-color: #D44638; color: #fff; padding: 8px 16px; margin: 5px 10px; text-decoration: none; border-radius: 4px;">Email</a> </p>




