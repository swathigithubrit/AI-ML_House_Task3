AI-ML_House_Task3
Linear Regression model to predict house prices using Python, pandas, and scikit-learn. Includes data preprocessing, model evaluation, and visualizations.

🏠 Linear Regression on House Price Dataset

Task Overview

This project is part of an internship task focused on implementing Linear Regression using Python and Scikit-learn in a Jupyter Notebook. The goal is to predict house prices based on various numerical and categorical features such as area, number of bedrooms, parking spaces, and more.

---

📂 Dataset Features

| Feature             | Description                            |
|---------------------|----------------------------------------|
| `price`             | Target variable (House price)          |
| `area`              | Total area of the house (in sq ft)     |
| `bedrooms`          | Number of bedrooms                     |
| `bathrooms`         | Number of bathrooms                    |
| `stories`           | Number of stories                      |
| `mainroad`          | Access to main road (yes/no)           |
| `guestroom`         | Has guestroom (yes/no)                 |
| `basement`          | Has basement (yes/no)                  |
| `hotwaterheating`   | Has hot water heating (yes/no)         |
| `airconditioning`   | Has air conditioning (yes/no)          |
| `parking`           | Number of parking spaces               |
| `prefarea`          | Located in a preferred area (yes/no)   |
| `furnishingstatus`  | Furnishing status (furnished/semi/unfurnished) |

---

🧪 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn`

---

📊 Workflow Summary

1. Data Loading & Cleaning
- Loaded the dataset using `pandas`
- Handled missing values and categorical encodings

2. Exploratory Data Analysis (EDA)
- Used histograms, boxplots, and pairplots
- Identified correlations using a heatmap

3. Data Preprocessing
- Converted categorical variables to numerical format (Label Encoding / One-Hot Encoding)
- Selected meaningful features for training

4. Model Training
- Split the data using `train_test_split`
- Trained a **Linear Regression** model using `sklearn.linear_model.LinearRegression`

5. Model Evaluation
- Evaluated using:
  - MAE (Mean Absolute Error)
  - MSE (Mean Squared Error)
  - R² Score

6. Visualizations Included
-  Actual vs Predicted Prices
-  Residual Plot
-  Distribution of Prices
-  Correlation Heatmap
-  Boxplots for categorical impact
-  Pairplot to explore feature relationships

---

Why Pairplot?
> `sns.pairplot()` was used to visually analyze relationships between numerical features like `area`, `bedrooms`, and `stories` with the target variable `price`.  
It helps detect linear trends, feature correlations, and outliers before model training.

---

Overview of Model Evaluation

The performance of the linear regression model on the test set is summarized below:

| Metric | Value | Description |
|--------|-------|-------------|
| **MAE** (Mean Absolute Error) | `1,265,275.67` | On average, the model's predictions are off by about ₹12.6 Lakhs. |
| **MSE** (Mean Squared Error) | `2,750,040,479,309.05` | The average of squared errors; heavily penalizes large errors. |
| **R² Score** | `0.456` | The model explains about 45.6% of the variance in house prices. |

 Interpretation

- 🔸 MAE of ~₹12.6 Lakhs indicates reasonably large deviations between actual and predicted prices.
- 🔸 MSE is high, which is expected due to large price values.
- 🔸 R² Score of 0.456 suggests the model explains about **46%** of the variability in the target — there's room for improvement, possibly by:
  - Adding more relevant features
  - Applying feature engineering
  - Trying more advanced models (e.g., Decision Tree, Random Forest, XGBoost)





