# Used Car Price Analysis

This project analyzes a dataset of over 34,000 used car listings to uncover the key factors that influence vehicle resale price. By applying the CRISP-DM framework and machine learning models, we provide actionable recommendations for a used car dealership seeking to optimize inventory and pricing strategy.

---

## Objective

- **Business Goal**: Identify what drives used car prices.
- **Audience**: Used car dealerships.
- **Deliverable**: Data-driven insights and a deployable pricing model based on vehicle attributes such as age, mileage, transmission, drivetrain, and regional data.

---

## Tools and Technologies

- **Language**: Python
- **Data Handling**: `pandas`, `numpy`
- **Visualization**: `seaborn`, `matplotlib`
- **Modeling**: `scikit-learn`, `RandomForestRegressor`
- **Workflow**: CRISP-DM Framework

---

## Project Structure

AI-ML-Assignment-11/
├──src/
│   ├── data/
│   │   └── vehicles.csv
│   ├── images/
│   │   └── crisp.png
│   │   └── kurt.png
│   └── prompt_II.ipynb
└── README.md

---

## Key Findings

- **Car Age & Mileage**: Newer cars with lower mileage consistently command higher prices.
- **Transmission**: Automatic vehicles tend to fetch better resale value.
- **Drive Type**: AWD/4WD vehicles often have regional demand premiums.
- **Location Matters**: States like CA and NY show higher resale values, while others like MI and IA trend lower.
- **Condition & Fuel Type**: Better-condition vehicles and hybrid/electric types show stronger market value.

---

## Model Evaluation

| Model             | R² Score (Test)  | Notes                       |
|-------------------|------------------|-----------------------------|
| Linear Regression | Broken           | Multicollinearity/outliers  |
| Ridge             | 0.37             | Regularized linear baseline |
| Lasso             | 0.03             | Over-penalized features     |
| Random Forest     | **0.43**         | Best performance & insights |

---

## Recommendations

- Stock newer vehicles with lower mileage.
- Prioritize automatic, AWD/4WD, and hybrid/electric vehicles.
- Adjust pricing based on regional trends and demand.
- Focus on excellent or like-new condition cars for better returns.

---

## Next Steps

- Integrate external data (e.g., vehicle history, time-on-market).
- Explore boosting models (e.g., XGBoost) for additional lift.
- Develop a dashboard for real-time pricing and inventory strategy.

---

## Source Code
- [Data](https://github.com/kloudingenuity/AI-ML-Assignment-11/blob/main/src/data/vehicles.csv)
- [Jupyter Notebook](https://github.com/kloudingenuity/AI-ML-Assignment-11/blob/main/src/prompt_II.ipynb)

--- 