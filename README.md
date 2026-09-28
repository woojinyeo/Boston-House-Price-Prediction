# Boston House Price Prediction

## Project Overview

This project develops a linear regression model to predict median house values in the Boston housing dataset.

The analysis focuses on identifying factors associated with housing prices, preparing the data for regression modeling, addressing multicollinearity, validating regression assumptions, and evaluating the model's ability to generalize to unseen data.

A detailed project report is included in this repository.

## Dataset

The dataset contains 506 observations and 13 housing-related variables, including:

- Crime rate
- Residential land proportion
- Non-retail business acreage
- Charles River proximity
- Nitric oxide concentration
- Average number of rooms
- Property age
- Distance to employment centers
- Highway accessibility
- Property tax rate
- Pupil-teacher ratio
- Population status
- Median home value

`MEDV`, the median value of owner-occupied homes, was used as the target variable.

## Analysis Approach

The project included:

- Exploratory Data Analysis (EDA)
- Distribution and skewness analysis
- Log transformation of the target variable
- Correlation analysis
- Multicollinearity analysis using Variance Inflation Factor (VIF)
- Train-test splitting
- Linear regression modeling
- Regression assumption testing
- Model evaluation using RMSE, MAE, and MAPE
- 10-fold cross-validation

## Key Findings

### Feature Relationships

The correlation analysis showed that the average number of rooms (`RM`) had a strong positive relationship with median house value, while `LSTAT` had a strong negative relationship with house value.

### Multicollinearity

High multicollinearity was identified between several predictors. `TAX` was removed after VIF analysis, reducing the VIF of `RAD` and improving the suitability of the predictors for linear regression.

### Model Performance

The linear regression model achieved similar performance on the training and test datasets.

| Dataset | RMSE | MAE | MAPE |
| --- | ---: | ---: | ---: |
| Training | 0.196 | 0.144 | 4.98% |
| Test | 0.198 | 0.151 | 5.26% |

The initial model score was approximately **0.769**.

After 10-fold cross-validation, the estimated model score was approximately **0.729**, providing a more conservative estimate of performance on unseen data.

## Featured Visualizations

### Correlation Heatmap

![Correlation Heatmap](images/Correlation%20Heatmap.png)

The heatmap was used to examine relationships between housing variables and identify potential multicollinearity.

---

### Multicollinearity Analysis

![VIF Analysis](images/VIF%20Analysis.png)

Variance Inflation Factor analysis was used to identify highly correlated predictors and guide feature removal.

---

### Regression Diagnostics

![Regression Diagnostics](images/Regression%20Diagnostics.png)

Regression diagnostics were used to evaluate assumptions such as residual behavior, homoscedasticity, and normality.

## Skills Demonstrated

- Python
- Exploratory Data Analysis
- Data preprocessing
- Statistical analysis
- Correlation analysis
- Linear regression
- Multicollinearity detection
- Variance Inflation Factor (VIF)
- Regression diagnostics
- Train-test evaluation
- Cross-validation
- Model interpretation

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- Jupyter Notebook / Google Colab

## Project Files

- `Boston House Price Prediction.pdf` – Full project report
- Python notebook – Data analysis and regression modeling
- Dataset – Boston housing data
- `images/` – Selected project visualizations

## Full Report

For the complete methodology, analysis, model evaluation, and recommendations, see:

**[Boston House Price Prediction Report](Boston%20House%20Price%20Prediction.pdf)**
