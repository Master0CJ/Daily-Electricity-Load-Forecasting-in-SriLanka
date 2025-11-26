# Daily-Electricity-Load-Forecasting-in-SriLanka

ML project that forecasts daily electricity demand in Sri Lanka, using Facebook Prophet model, with SHAP analysis for model explainability.

##  1. Objectives

- **Dataset**: Synthetic Sri Lankan load forecasting dataset
- **Goal**: Forecast daily electricity demand for the next 30 days
- **Model**: Facebook Prophet with seasonality components
- **Explainability**: SHAP analysis for feature importance

##  2. Technologies Used
**Python3 , numpy,  pandas,  matplotlib,  scikit-learn, Prophet, SHAP Analysis**

### About Facebook's Prophet

Prophet is an open-source forecasting tool developed by Facebook's Core Data Science team, designed for making accurate time series predictions with minimal manual effort.

### Key Features of Facebook Prophet
- **Handles Missing Data**: Automatically manages missing values and outliers
- **Seasonal Patterns**: Captures daily, weekly, and yearly seasonality automatically
- **Holiday Effects**: Built-in support for custom holiday calendars and events
- **Trend Changes**: Detects and adapts to trend shifts in your data
- **Fast Performance**: Uses Stan for efficient model fitting

### Best Use Cases of Facebook Prophet
- Anomaly detection in time series data
- Data with strong seasonal patterns
- Datasets with historical trend changes

Prophet works best with **time series data that has at least several months of historical data** and displays clear seasonal patterns.

##  3. Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/electricity-load-forecasting.git
cd electricity-load-forecasting
```

2. Install required packages:
```bash
pip install pandas numpy matplotlib prophet scikit-learn shap
```

## 4. Dataset
- **File**: `forecasting_dataset.csv`

## 5. Use
```bash
jupyter notebook daily-electricity-load-forecasting-in-sriLanka.ipynb
```

## 6. Workflow Steps in ipynb

1. **Setup and Imports**: Load required libraries
2. **Load Data**: Import and parse the dataset
3. **Preprocessing**: Resample to daily frequency
4. **Train/Test Split**: 80/20 chronological split
5. **Model Training**: Fit Prophet model
6. **Predictions**: Generate forecasts
7. **Visualization**: Plot forecasts vs actuals
8. **Component Analysis**: Analyze trend and seasonality
9. **Evaluation**: Calculate RMSE, MAE, MAPE
10. **Future Forecasting**: Predict next 30 days
11. **SHAP Analysis**: Explain model predictions

## 7. Model Performance

- **RMSE** = 20.96
- **MAE** = 16.84
- **MAPE** = 1.13%

## 8. Key Features
### Prophet Components
- **Trend**: Long-term demand pattern
- **Yearly Seasonality**: Annual variation patterns
- **Weekly Seasonality**: Day-of-week effects

### SHAP Analysis
- **Summary Plots**: Visualizes feature contribution to predictions
- **Feature Importance**: Ranks components by impact
- **Interpretability**: Explains which components drive predictions


## 9. Future Improvements

- [ ] Add weather features (temperature, humidity)
- [ ] Incorporate holiday effects
- [ ] Experiment with other forecasting models (LSTM, ARIMA, SARIMA, XGBoost)
- [ ] Hyperparameter tuning
- [ ] Add external regressors

## 10. Author

- GitHub: [@Master0CJ](https://github.com/Master0CJ)
  
**Note**: This project uses synthetic data for demonstration purposes. Real-world deployment would require actual load data and additional validation.
