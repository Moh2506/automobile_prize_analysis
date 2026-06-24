# Automobile Price Data Analysis

## Overview

This project continues the analysis of the UCI Automobile Dataset following a data wrangling and feature engineering phase. After cleaning the dataset, handling missing values, normalizing variables, and creating new features, the focus shifted to exploratory data analysis (EDA) and statistical testing to identify the factors most strongly associated with automobile prices.

The objective of this project is to uncover meaningful relationships between vehicle characteristics and price, validate those relationships statistically, and generate insights that can support future predictive modeling.

### Related Resources

* [Data Wrangling and Feature Engineering for the UCI Automobile Dataset](https://github.com/Moh2506/automobile_data_cleaning)
* [Dataset Source](https://archive.ics.uci.edu/ml/datasets/automobile)

---

## Methodology

The analysis combined data visualization and statistical testing to investigate the relationship between vehicle characteristics and automobile prices.

Techniques used include:

* Descriptive statistics
* Regression plots
* Correlation analysis
* Boxplots for categorical variables
* Grouping and aggregation
* Pivot tables and heatmaps
* Pearson Correlation
* ANOVA testing

---

## Key Findings

### Strongest Numerical Predictors of Price

| Variable        | Pearson Correlation (r) |
| --------------- | ----------------------- |
| Engine Size     | 0.87                    |
| Curb Weight     | 0.83                    |
| Horsepower      | 0.81                    |
| Highway L/100km | 0.80                    |
| City L/100km    | 0.79                    |

Engine size emerged as the strongest predictor of automobile price, exhibiting a very strong positive relationship with vehicle value.

Curb weight and horsepower also showed strong positive correlations, indicating that larger and more powerful vehicles generally command higher prices.

Fuel consumption variables displayed strong associations with price, reflecting differences in vehicle size, engine performance, and market positioning.

### Moderate Predictors

| Variable   | Pearson Correlation (r) |
| ---------- | ----------------------- |
| Width      | 0.75                    |
| Length     | 0.69                    |
| Wheel Base | 0.59                    |
| Bore       | 0.54                    |

Vehicle dimensions demonstrated moderate positive relationships with price, suggesting that larger vehicles tend to be priced higher on average.

### Weak Predictors

| Variable | Pearson Correlation (r) |
| -------- | ----------------------- |
| Peak RPM | -0.10                   |

Peak RPM showed almost no relationship with automobile price, making it a weak predictor of vehicle value.

### Categorical Analysis

Analysis of drive-wheel categories revealed meaningful differences in average vehicle prices.

Key observations:

* Rear-wheel-drive vehicles recorded the highest average prices.
* Front-wheel-drive vehicles were generally less expensive.
* ANOVA confirmed statistically significant price differences across drive-wheel categories.
* The strongest statistical distinction was observed between rear-wheel-drive and front-wheel-drive vehicles.

---

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy

---

## Conclusion

Engine size, horsepower, curb weight, and fuel consumption metrics emerged as the strongest predictors of automobile prices, while Peak RPM showed little explanatory value. Statistical testing also confirmed that drive-wheel configuration significantly influences vehicle pricing, providing a strong foundation for future predictive modeling.

---

## Next Steps

The next phase of this project will focus on:

* Linear Regression
* Multiple Linear Regression
* Model Evaluation
* Automobile Price Prediction
