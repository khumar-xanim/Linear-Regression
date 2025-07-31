#  House Price Prediction (Kaggle Dataset)

This project uses the famous **Kaggle House Prices** dataset to demonstrate a full data preprocessing and modeling pipeline with a focus on linear regression.

##  Objective

Predict the `SalePrice` of houses based on various features.

##  Workflow Overview

### 1. Data Preparation
- Split the dataset into train and test sets
- Save processed files for reuse
- Drop uninformative columns:
  - Columns with too many nulls
  - Columns with all unique values
  - Columns with low variance (over 99% same value)

### 2. Data Cleaning
- Detect and remove outliers
- Impute missing values (numeric and categorical)

### 3. Feature Engineering
- Create new informative features

### 4. Encoding and Scaling
- Encode categorical features
- Standardize numeric features using `StandardScaler`

### 5. Feature Selection
- Drop columns with low correlation to target
- Remove multicollinear and redundant features

### 6. Modeling
- Train a linear regression model on `log(SalePrice)`
- Evaluate performance using metrics like RMSE (with unlogged predictions)

##  Main File

Notebook: `0 usul.ipynb`

##  Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
