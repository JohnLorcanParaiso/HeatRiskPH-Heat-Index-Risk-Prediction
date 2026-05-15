# HeatRisk PH

## Project Overview
HeatRisk PH is a predictive analytics project designed to analyze, classify, and forecast heat index risks in Metro Manila, Philippines using historical weather data.

The project combines:
- Regression Analysis
- Classification Modeling
- SARIMAX Time-Series Forecasting

to generate actionable heat-risk insights for:
- Local Government Units (LGUs)
- Schools and universities
- Workplaces
- Public health planners
- Disaster risk reduction offices

The project follows the CRISP-DM framework and transforms historical weather data into practical heat-risk intelligence for proactive planning and decision-making.

---

# Objectives

The project aims to:

- Predict daily heat index values
- Identify key weather variables affecting heat conditions
- Classify heat-risk levels
- Forecast future heat-risk periods
- Support climate resilience and public safety planning

---

# Models Used

## 1. Regression Model
Predicts daily `heat_index_mean` values and identifies the strongest weather-related drivers of heat.

### Purpose
- Understand drivers of heat
- Quantify variable influence
- Analyze heat sensitivity patterns

### Target Variable
```python
heat_index_mean
```

### Example Features
- temperature_2m_mean
- apparent_temperature_mean
- humidity
- wind speed

---

## 2. Classification Model
Classifies daily heat conditions into predefined risk levels.

### Risk Categories
- Safe
- Caution
- Extreme Caution

### Purpose
- Convert numerical heat index values into understandable risk levels
- Support easier interpretation for decision-makers

---

## 3. SARIMAX Time-Series Forecasting
Forecasts future heat index trends for the next 14 days.

### Purpose
- Predict future heat-risk periods
- Support early warning and planning
- Enable proactive intervention strategies

---

# Dataset Information

## Data Source
Open-Meteo Historical Weather API

## Location
Metro Manila, Philippines

## Period Covered
January 2019 – May 2026

## Variables Used

| Variable | Description |
|---|---|
| `temperature_2m_mean` | Average air temperature |
| `temperature_2m_max` | Maximum air temperature |
| `temperature_2m_min` | Minimum air temperature |
| `apparent_temperature_mean` | Average apparent temperature |
| `apparent_temperature_max` | Maximum apparent temperature |
| `apparent_temperature_min` | Minimum apparent temperature |

---

# Project Structure

```bash
HeatRiskPH/
│
├── data/
│   ├── heat_index_metro_manila_2019_2025
│
├── notebooks/
│   ├── HeatRiskPH_Final_Notebook.ipynb
│
├── README.md
└── requirements.txt
```

---

# Requirements

- Python 3.10+
- Jupyter Notebook or Google Colab

Install required packages:

```python
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
```

---

# Execution Instructions

1. Open `HeatRiskPH_Final_Notebook.ipynb` using Jupyter Notebook or Google Colab.  
2. Ensure the dataset file is placed in the correct directory/path specified in the notebook.  
3. Run the notebook cells sequentially from top to bottom to reproduce:
   - Regression analysis
   - Classification modeling
   - SARIMAX forecasting
   - Visualizations and evaluation metrics

---

# Evaluation Metrics

## Regression Metrics
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score

## Classification Metrics
- Accuracy
- Precision
- Recall
- F1-Score

## Forecasting Metrics
- AIC
- BIC
- Forecast Error Analysis

---

# Key Features

- Heat Index prediction
- Heat-risk classification
- Time-series forecasting
- Climate risk analytics
- Data visualization dashboards
- Decision-support insights

---

# Potential Applications

- Heat advisory systems
- School suspension planning
- Workplace heat safety monitoring
- Public health preparedness
- Urban climate resilience planning

---

# Sustainable Development Goals (SDGs)

This project supports:

- SDG 3 — Good Health and Well-Being
- SDG 11 — Sustainable Cities and Communities
- SDG 13 — Climate Action
- SDG 17 — Partnerships for the Goals

---

# Researchers

## John Lorcan E. Paraiso
**Project Lead / Data & Design Coordinator**

### Contributions
- Topic selection and project direction
- Dataset preprocessing setup
- Notebook organization and CRISP-DM structure
- Whitepaper design and layout
- References compilation and final organization
- Co-developed coding and model analysis

---

## Jezrev Daniel R. Labay
**Data Visualization & Findings Interpretation Lead**

### Contributions
- Visualization of model results
- Interpretation and discussion of findings
- Supported review and validation of outputs
- Assisted in final checking and refinement
- Co-developed coding and model analysis

---

# References

- Open-Meteo Historical Weather API
- PAGASA Heat Index Data
- IPCC Climate Reports
- UNDRR Heat Exposure Reports
- World Weather Attribution Studies

---

# License

This project is intended for academic and research purposes only.

---

# HeatRisk PH Whitepaper
ThermaSense Analytics — 2026
