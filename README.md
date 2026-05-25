# Life Expectancy ML Prediction

A machine learning project that predicts global life expectancy using World Bank development indicators. Three regression models are trained, evaluated, and compared to identify the best predictor.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat-square&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

---

## Overview

Using publicly available World Bank data, this project builds a complete ML pipeline — from raw data ingestion and reshaping through EDA, feature engineering, model training, and evaluation. The target variable is **life expectancy at birth (years)**.

---

## Dataset

**Source:** World Bank World Development Indicators

**Features used:**
| Indicator | Description |
|-----------|-------------|
| Mortality rate, adult, female | Per 1,000 female adults |
| Mortality rate, adult, male | Per 1,000 male adults |
| Mortality rate, infant | Per 1,000 live births |
| Mortality rate, under-5 | Per 1,000 live births |
| Diabetes prevalence | % of population ages 20–79 |
| Physicians | Per 1,000 people |
| Hospital beds | Per 1,000 people |
| Health expenditure | % of GDP |
| GDP per capita | Current US$ |
| School enrollment, secondary | % gross |

---

## Features

- Reshape World Bank wide-format data (years as columns) into long format
- Exploratory data analysis — histograms, box plots, correlation heatmaps, pairplots
- Clean pipeline: missing value handling, feature scaling (StandardScaler)
- Three models trained and compared:
  - Linear Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
- Model evaluation with MAE, RMSE, and R²
- Feature importance analysis from Random Forest

---

## Project Structure

```
life_expectancy_prediction.ipynb   # Main Jupyter notebook
data.csv                           # Raw World Bank dataset
metadata.csv                       # Dataset column metadata
life_expectancy_ml_report.pdf      # Full written report
```

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Sparkz691768/Life-Expectancy-ML-Prediction.git
   cd Life-Expectancy-ML-Prediction
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook life_expectancy_prediction.ipynb
   ```

---

## Models & Results

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| Linear Regression | — | — | — |
| Random Forest | — | — | — |
| Gradient Boosting | — | — | — |

> Run the notebook to populate actual metrics.

---

## What I Learned

- Working with real-world open data from the World Bank API
- Reshaping wide tabular data (pivot/melt) for ML use
- Comparing multiple regression models on the same dataset
- Interpreting feature importance to understand which indicators drive predictions
- Building a complete end-to-end ML pipeline

---

## Future Improvements

- Hyperparameter tuning with GridSearchCV / RandomizedSearchCV
- Add more recent data years via World Bank API
- Build an interactive prediction dashboard with Streamlit
- Experiment with XGBoost and neural network regressors
- Add cross-validation for more robust evaluation