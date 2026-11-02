# Time Series Analysis of Housing Loans in France

## Overview

This project focuses on the analysis and forecasting of monthly housing loan volumes granted to households in France.

The objective is to apply **Time Series Analysis methodologies** on a real financial dataset published by the **Banque de France**, studying the evolution of new housing loans and identifying trend, seasonal patterns, and forecasting capabilities.

The project follows a complete time series workflow:
- Dataset understanding and preparation
- Time series decomposition
- Seasonality and trend analysis
- Model selection
- Forecasting evaluation

## Dataset

The dataset contains the **monthly flow of new housing loans granted to households in France**, expressed in millions of euros.

Source:
- Banque de France Webstat database

The cleaned dataset contains monthly observations from **June 2010 to August 2026**.

## Objectives

The main objectives of this project are:

- Understand the structure of a financial time series
- Clean and prepare real-world economic data
- Analyze trend and seasonal components
- Determine the appropriate decomposition model
- Build forecasting models
- Evaluate forecasting performance on unseen data

## Methodology

### 1. Data Cleaning and Preparation

The initial dataset required several preprocessing steps:

- Removal of metadata rows
- Conversion of dates and numerical values
- Chronological sorting
- Setting monthly frequency
- Creation of a clean time series ready for analysis

## 2. Time Series Decomposition

The series was analyzed through:

- Visual examination
- Band method
- Buys-Ballot table analysis
- Autocorrelation analysis

These methods were used to identify:
- Trend component
- Seasonal patterns
- Residual behavior

The analysis suggested a **multiplicative decomposition model**, as seasonal variations increase with the level of the series.

## 3. Forecasting Models

Two forecasting approaches were implemented:

### Decomposition-based forecasting

A decomposition model using trend and seasonal components was applied to predict future loan volumes.

### ARIMA Model

An ARIMA model was developed based on the time series structure and evaluated on the test period.

## Results

Both forecasting approaches provided similar performances:

- The models successfully captured the seasonal behavior of housing loan volumes.
- Forecast errors were around **8%** on the 2026 test period.
- The models tended to slightly overestimate the market level because they only relied on historical values.

## Limitations and Future Improvements

The project highlights several possible improvements:

- Include external economic variables such as interest rates or inflation indicators
- Use longer validation periods
- Integrate additional financial and macroeconomic features
- Explore more advanced forecasting approaches

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Scikit-learn

## Project Structure

```text
.
├── Loan_TSA_project_HIJAZI.ipynb
├── README.md
└── dataset/
    └── Webstat_export_file.csv
```

## Installation

Clone the repository:

```bash
git clone https://github.com/username/repository-name.git
```

Install dependencies:

```bash
pip install pandas numpy matplotlib statsmodels scikit-learn jupyter
```

## Usage

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Loan_TSA_project_HIJAZI.ipynb
```

and run the cells sequentially.

## AI Assistance Disclosure

This project was developed with limited AI assistance.

AI was mainly used for:
- Supporting code implementation for some visualizations
- Clarifying methodological interpretations
- Improving English phrasing

All methodological choices, analyses, and conclusions were independently reviewed and validated.

## Author

**Inès Hijazi**

