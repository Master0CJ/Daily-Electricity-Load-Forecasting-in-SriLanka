# Daily-Electricity-Load-Forecasting-in-SriLanka

A ML project that forecasts daily electricity demand in Sri Lanka, using Facebook Prophet, with SHAP analysis for model explainability.

## 🎯 Objectives

- **Dataset**: Synthetic Sri Lankan load forecasting dataset
- **Goal**: Forecast daily electricity demand for the next 30 days
- **Model**: Facebook Prophet with seasonality components
- **Explainability**: SHAP analysis for feature importance

## 🔧 Technologies Used

- **Python 3.x**
- **numpy**: Numerical computations
- **pandas**: Data manipulation and preprocessing
- **matplotlib**: Data visualization
- **scikit-learn**: Model evaluation metrics
- **Prophet**: Time series forecasting
- **SHAP**: Model explainability

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/electricity-load-forecasting.git
cd electricity-load-forecasting
```

2. Install required packages:
```bash
pip install pandas numpy matplotlib prophet scikit-learn shap
```

## 📊 Dataset

The dataset contains electricity load measurements at 15-minute intervals with the following characteristics:

- **Time Range**: from 01-01-2020 to 31-05-2025
- **Frequency**: 15-minute intervals (I later aggregated this to daily)
- **Target Variable**: Load Demand (kW)
- **File**: `forecasting_dataset.csv`

### Data Preprocessing

- Timestamps converted to datetime objects
- 15-minute intervals resampled to daily frequency using mean aggregation
- Chronological 80/20 train-test split

## 🚀 Usage

Run the Jupyter notebook:

```bash
jupyter notebook daily-electricity-load-forecasting-in-sriLanka.ipynb
```

### Workflow Steps

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

## 📈 Model Performance

The model is evaluated using:

- **RMSE** = 20.96
- **MAE** = 16.84
- **MAPE** = 1.13%

## 🔍 Key Features

### Prophet Components

- **Trend**: Long-term demand pattern
- **Yearly Seasonality**: Annual variation patterns
- **Weekly Seasonality**: Day-of-week effects

### SHAP Analysis

- **Summary Plots**: Visualizes feature contribution to predictions
- **Feature Importance**: Ranks components by impact
- **Interpretability**: Explains which components drive predictions


## 🧪 Results

The SHAP analysis reveals:

- **Trend component** has the largest impact on predictions (≈1400 SHAP value)
- **Seasonal components** (weekly/yearly) have minimal impact (between -50 and +50)
- Model predictions are primarily driven by long-term demand patterns

## 📝 Future Improvements

- [ ] Add weather features (temperature, humidity)
- [ ] Incorporate holiday effects
- [ ] Experiment with other models (LSTM, ARIMA)
- [ ] Hyperparameter tuning
- [ ] Add external regressors

## 👤 Author

- GitHub: [@Master0CJ](https://github.com/Master0CJ)
  
**Note**: This project uses synthetic data for demonstration purposes. Real-world deployment would require actual load data and additional validation.
