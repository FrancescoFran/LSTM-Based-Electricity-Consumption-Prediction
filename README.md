# LSTM Based Electricity Consumption Prediction
### A deep‑learning model that predicts future electricity consumption using LSTM‑based time‑series analysis.
<p align="left">
  <img alt="Python" src="https://img.shields.io/badge/Python-3.10-blue?logo=python">
  <img alt="TensorFlow" src="https://img.shields.io/badge/TensorFlow-2.x-FF6F00?logo=tensorflow&logoColor=white">
  <img alt="License" src="https://img.shields.io/badge/License-MIT-green">
  <img alt="Status" src="https://img.shields.io/badge/Status-Active-success">
</p>

<p align="center">
  <p align="center">
  <img src="images/banner.svg" alt="Project Banner" width="100%">
</p>
</p>

## Table of Contents
- [About](#about)
- [Features](#features)
- [Installation](#installation)
- [Usage](#️usage)
- [Screenshots](#screenshots)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Support](#️support)

---

## About
LSTM-Based-Electricity-Consumption-Prediction is a machine learning project designed to forecast future household electricity usage using Long Short‑Term Memory (LSTM) neural networks. Electricity consumption naturally varies due to daily routines, weekends, weather changes, and holidays. Traditional forecasting methods struggle with these irregular patterns—this project uses deep learning to model them more accurately.
The goal is to provide a reliable system that predicts energy demand ahead of time, helping users better understand consumption behavior, optimize usage, and potentially reduce energy costs.

### Quick start / Dataset download  
A preprocessed CSV snapshot of the household_power_consumption dataset is available as a release asset.

- Latest release (CSV): https://github.com/FrancescoFran/LSTM-Based-Electricity-Consumption-Prediction/releases/latest
- Direct download (curl):
  curl -L -o household_power_consumption.csv "https://github.com/FrancescoFran/LSTM-Based-Electricity-Consumption-Prediction/releases/latest/download/household_power_consumption.csv"

---

## Features
- **Comprehensive Data Pipeline**  
  Automatic loading, cleaning, type conversion, datetime indexing, and exporting of processed datasets.

- **Advanced Exploratory Data Analysis**  
  Interactive visualizations, consumption‑pattern analysis, temporal trend inspection, and PACF‑based time‑series diagnostics.

- **Robust Preprocessing & Feature Engineering**
  Missing‑value imputation, outlier handling, hourly resampling, correlation analysis, VIF checks, and creation of temporal features (Hour, DayOfWeek, IsWeekend).

- **Deep Learning Forecasting Framework**
  Multiple LSTM architectures (stacked, dropout‑regularized, high‑capacity, long‑sequence models), TensorFlow dataset pipelines, evaluation metrics (MAE, RMSE, MAPE, SMAPE), prediction plots, error analysis, and model comparison.

---

## Installation
1. **Clone the repository**  
   git clone https://github.com/FrancescoFran/LSTM-Based-Electricity-Consumption-Prediction.git  
   cd project-name
   
3. **Install dependencies**  
   pip install -r requirements.txt

---

## Usage
  1. **Dataset:** Place CSV in `data/`.
  2. **Preprocess:**
     - Interactive: Open and "Run All" for: notebooks/preprocessing.ipynb
     - Headless (optional): jupyter nbconvert --to notebook --execute notebooks/preprocessing.ipynb --output notebooks/preprocessing_ran.ipynb
       ExecutePreprocessor.timeout=600
  4. **Train, Evaluate, Visualize results:**
     - Interactive: Open and "Run All" for: notebooks/lstm_training_evaluation.ipynb  
     - Headless (optional): jupyter nbconvert --to notebook --execute notebooks/lstm_training_evaluation.ipynb --output notebooks/lstm_training_ran.ipynb --
       ExecutePreprocessor.timeout=3600
     
---

## Screenshots
<p align="center">
  <table style="width:100%; border-collapse:collapse;">
    <tr>
      <td style="width:50%; padding:0;">
        <img src="images/Analysis_monthly.png" alt="Analysis_monthly" style="width:100%; display:block;" />
      </td>
      <td style="width:50%; padding:0;">
        <img src="images/Analysis_daily.png" alt="Analysis_daily" style="width:100%; display:block;" />
      </td>
    </tr>
    <tr>
      <td style="width:50%; padding:0;">
        <img src="images/Prediction.png" alt="Prediction" style="width:100%; display:block;" />
      </td>
      <td style="width:50%; padding:0;">
        <img src="images/Error_analysis.png" alt="Error_analysis" style="width:100%; display:block;" />
      </td>
    </tr>
  </table>
</p>
---

## License
This project is under the **MIT License**.  
