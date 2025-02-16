# Project Overview

## Objective: Predict laptop prices using the following features:

- RAM (GB): Amount of memory in gigabytes
- Resolution: Screen resolution (e.g., 1920x1080)
- Processor: Type of processor (e.g., Intel i5, AMD Ryzen)
- Screen Size (inch): Display size in inches

#### Tech Stack:  Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

### Models Used:

- Random Forest
- XGBoost
- K-Nearest Neighbors (KNN)

#### Hyperparameter Tuning: GridSearchCV was used for model optimization.

#### Outcome: Accurate price predictions with insights into feature importance.

# Project Workflow

### 1) Summary Statistics

- Calculated basic statistics to understand the distribution and central tendency of each feature.

### 2) Data Preprocessing

- Handled missing values and outliers.
- Categorical encoding for the 'Processor' feature.
- Scaled numerical features where necessary.

### 3) Exploratory Data Analysis (EDA)

- Univariate Analysis: Examined individual features to understand their distribution.
- Bivariate Analysis: Analyzed the relationship between each feature and the target variable (Price).
- Multivariate Analysis: Explored interactions between multiple features.
- Correlation Matrix: Visualized correlations to identify highly correlated features.

### 4) Feature Importance

The importance scores of the features, calculated using the best-performing model, are shown below:

| Column               | Feature Importance (%) |
|----------------------|-------------------------|
| RAM (GB)             | 45.49                   |
| Processor            | 27.50                   |
| Resolution           | 24.38                   |
| Screen Size (inch)   |  2.63                   |

### 5) Model Building and Evaluation

Implemented the following models:

- Random Forest
- XGBoost
- K-Nearest Neighbors (KNN)
- Used GridSearchCV for hyperparameter tuning.
- Evaluated model performance using R² and RMSE for both training and test datasets.

### Model Performance

The model performance metrics are summarized in the table below:

| Model          | Train R² (%) | Test R² (%) | Train RMSE | Test RMSE |
|----------------|--------------|-------------|------------|-----------|
| Random Forest  | 84.35        | 80.80       | 519.53     | 583.31    |
| XGBoost        | 84.46        | 80.85       | 517.58     | 582.56    |
| KNN            | 83.74        | 80.10       | 529.44     | 593.83    |

### Key Takeaways

- RAM (GB) and Processor are the most influential features for predicting laptop prices.
- XGBoost outperformed other models, making it the best choice for this problem.
- The model can help customers and retailers make data-driven pricing decisions.






