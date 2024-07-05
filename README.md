---

# Weather Forecasting with TBATS Models

This repository contains code and models for weather forecasting using TBATS (Trigonometric seasonality, Box-Cox transformation, ARMA errors, Trend, and Seasonal components) models. TBATS models are particularly effective for time series forecasting with complex seasonal patterns.

## Dataset

The dataset used in this project can be downloaded from [Kaggle](https://www.kaggle.com/datasets/safdar712/temperature-pk). It comprises daily weather data with 12,784 entries, spanning from January 2, 1980, to January 1, 2015.

## Models

Two TBATS models were trained for this project:

### Model Y (Yearly Seasonality)

- **Mean Squared Error**: 1.8585
- **Mean Absolute Error**: 1.0448
- **Root Mean Squared Error**: 1.3632

### Model YM (Yearly and Monthly Seasonality)

- **Mean Squared Error**: 1.8529
- **Mean Absolute Error**: 1.0437
- **Root Mean Squared Error**: 1.3632

These metrics indicate the accuracy achieved by each model in forecasting the weather based on the dataset.

## Code

The repository includes a Jupyter notebook `TBATS.ipynb` that contains the complete pipeline for data preprocessing, model training (TBATS), evaluation, and forecast analysis for the next 15 years.

### Contents of `TBATS.ipynb`:

- **Data Preprocessing:** Steps for cleaning, transforming, and preparing the dataset.
  
- **Model Training:** Implementation of TBATS models for both yearly and yearly-monthly seasonality.

- **Evaluation:** Assessing model performance using various metrics and visualizing forecast results against actual data.

- **Forecast and Analysis:** Generating forecasts for the next 15 years based on trained models and analyzing the predictions.

## Getting Started

To get started with using the code and models in this repository, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ahmedshahwar/weather-forecast.git
   cd weather-forecast
   ```

2. **Install dependencies:**
   Ensure you have Python 3.x installed along with necessary libraries like `numpy`, `pandas`, `tbats`, `matplotlib`, `scikit-lean`, and `pickle`.

3. **Run the `TBATS.ipynb` notebook:**
   - Use this notebook to replicate the preprocessing, model training, evaluation, and forecasting steps on your dataset.
   
4. **Explore and analyze results:**
   - Modify the notebook as needed to fit your specific forecasting requirements and data characteristics.
