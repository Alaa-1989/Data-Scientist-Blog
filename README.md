# Business Formation Analysis and Prediction (U.S.)
This repository contains the analysis, modeling, and visualizations for a data science project that explores business formation trends in the United States before, during, and after the COVID-19 pandemic.
The project was completed as part of the Udacity Data Scientist Nanodegree.

## Project Overview
Starting a new business is often considered a signal of economic confidence. This project investigates how business formation activity changed over time, with a particular focus on the COVID-19 period, and whether simple machine learning models can be used to predict future business creation.

The analysis follows the CRISP-DM process and combines exploratory data analysis with a regression-based prediction task.


## Key Questions
- How has business formation activity evolved over time across U.S. states?
- What patterns can be observed before, during, and after the COVID-19 pandemic?
- Can a simple supervised learning model produce a reasonable prediction for a missing future month?

## The Data
The project uses Business Formation Statistics (BFS) published by the U.S. Census Bureau.
- Time span: 2004–2025
- Analysis window: 2013–2025 (approximately six years before and after COVID-19)
- Granularity: Monthly, state and regional level
- Target variable: Number of newly created businesses

The U.S. aggregate level (US) was excluded to focus on state-level patterns.
December 2025 is missing from the dataset and is treated as a future value to be predicted.

## Methods
- Data cleaning and reshaping (wide → long format)
- Exploratory data analysis (distributions, time series, geographic comparisons)
- Feature engineering (time features and COVID-19 indicator)
- Supervised learning using Linear Regression
- Model evaluation using MAE, RMSE, and R²
- Visual validation of predictions

## Key Findings
- Business formation activity varies substantially across states.
- Large states such as California consistently lead in new business creation.
- The COVID-19 period is associated with increased volatility rather than sustained decline.
- Post-2020 business formation shows a strong upward trend.
- The December 2025 prediction aligns with historical December trends, suggesting a plausible continuation of post-pandemic activity.

## Repository Structure
```
       ├── data/
│   └── bfs_monthly.csv
│   └── bfs_monthly_data_dictionary.pdf
├── images/
│   └── exported_charts/
├── business_formation_analysis.ipynb
├── README.md
```

## Tools and Libraries
- Python
- pandas
- numpy
- matplotlib
- scikit-learn

## References

- U.S. Census Bureau. Business Formation Statistics (BFS)
https://www.census.gov/econ/bfs/
- Udacity. Data Scientist Nanodegree
- Pedregosa, F., et al. (2011). Scikit-learn: Machine Learning in Python


## Author

This project was created as part of a learning journey in data science and applied machine learning.
For more details, see the accompanying Medium blog post.









