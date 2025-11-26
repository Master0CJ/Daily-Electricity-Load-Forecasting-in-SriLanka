# Daily-Electricity-Load-Forecasting-in-SriLanka

ML project that forecasts daily electricity demand in Sri Lanka, using Facebook Prophet model, with SHAP analysis for model explainability.

##  Objectives

- **Dataset**: Synthetic Sri Lankan load forecasting dataset
- **Goal**: Forecast daily electricity demand for the next 30 days
- **Model**: Facebook Prophet with seasonality components
- **Explainability**: SHAP analysis for feature importance

##  Technologies Used
**Python 3.x, numpy,  pandas,  matplotlib,  scikit-learn, Prophet, SHAP Analysis**

##  Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/electricity-load-forecasting.git
cd electricity-load-forecasting
```

2. Install required packages:
```bash
pip install pandas numpy matplotlib prophet scikit-learn shap
```

##  Dataset
- **File**: `forecasting_dataset.csv`

##  Usage
```bash
jupyter notebook daily-electricity-load-forecasting-in-sriLanka.ipynb
```

## Workflow Steps

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

##  Model Performance

- **RMSE** = 20.96
- **MAE** = 16.84
- **MAPE** = 1.13%

##  Key Features
### Prophet Components
- **Trend**: Long-term demand pattern
- **Yearly Seasonality**: Annual variation patterns
- **Weekly Seasonality**: Day-of-week effects

### SHAP Analysis
- **Summary Plots**: Visualizes feature contribution to predictions
- **Feature Importance**: Ranks components by impact
- **Interpretability**: Explains which components drive predictions


##  Future Improvements

- [ ] Add weather features (temperature, humidity)
- [ ] Incorporate holiday effects
- [ ] Experiment with other models (LSTM, ARIMA)
- [ ] Hyperparameter tuning
- [ ] Add external regressors

##  Author

- GitHub: [@Master0CJ](https://github.com/Master0CJ)
  
**Note**: This project uses synthetic data for demonstration purposes. Real-world deployment would require actual load data and additional validation.
