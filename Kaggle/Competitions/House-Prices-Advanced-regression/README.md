# House Prices Prediction

Kaggle competition to predict house prices using 79 features from residential homes in Ames, Iowa.

## Overview

This notebook implements a robust regression analysis with:

- Exploratory Data Analysis (EDA)
- Correlation and Multicollinearity analysis (VIF)
- Influence diagnostics (Cook's Distance)
- Preprocessing pipeline with scikit-learn
- 8 regression models compared using **10 seeds × 5-fold CV = 50 evaluations**

## Results

| Model                      | RMSLE CV   |
| -------------------------- | ---------- |
| Linear Regression          | 0.6750     |
| Weighted Regression        | 0.6021     |
| Without Influential Points | 0.1094     |
| Polynomial (degree 2)      | 0.3557     |
| Cubic Splines              | 0.1399     |
| GAM                        | 0.1447     |
| Without Multicollinearity  | 0.4189     |
| **Combined (Best)**        | **0.1013** |

## Files

- `house-prices.ipynb` - Main analysis notebook
- `data/train.csv` - Training data (1,460 houses)
- `data/test.csv` - Test data for submission
- `submission.csv` - Kaggle submission file

## Requirements

```
pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels
```

## Links

- [Kaggle Competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
