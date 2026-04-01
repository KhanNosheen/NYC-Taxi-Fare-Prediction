# Regression Model for Predicting Taxi Fare Amount

## 📌 Project Overview
This project focuses on building a multiple linear regression model to predict taxi fare amounts using the NYC TLC Trip Record dataset. By following the **PACE (Plan, Analyze, Construct, Execute)** framework, I developed a model that helps estimate costs for passengers and provides predictable earning insights for drivers.

## 🚀 Key Findings & Model Performance
The model was evaluated using standard regression metrics. The results indicate a strong predictive capability:

| Metric | Value |
| :--- | :--- |
| **R² (Coefficient of Determination)** | **0.7477** |
| **MAE (Mean Absolute Error)** | **1.6166** |
| **MSE (Mean Squared Error)** | **5.0287** |
| **RMSE (Root Mean Squared Error)** | **2.2425** |

* **Accuracy:** The model explains approximately **74.77%** of the variance in fare amounts.
* **Reliability:** With an **MAE of 1.6166**, the model's predictions are, on average, within **$1.62** of the actual fare.

## 🛠️ Methodology: The PACE Framework

### 1. Plan
* **Goal:** Predict the `fare_amount` based on trip features.
* **Data Source:** NYC Taxi and Limousine Commission (TLC) Trip Record Data.
* **Success Metrics:** MAE, RMSE, and R².

### 2. Analyze
* Identified and handled significant outliers (e.g., maximum fare amounts exceeding $1,200 and tip amounts of $200).
* Performed Exploratory Data Analysis (EDA) to understand the distribution of fares and trip distances.
* Verified data integrity, ensuring no missing values or duplicates remained.

### 3. Construct
* **Feature Engineering:** Extracted time-based features and handled categorical variables.
* **Pre-processing:** Applied `StandardScaler` to ensure all features were on the same scale for the linear regression model.
* **Modeling:** Utilized `scikit-learn` to build a multiple linear regression pipeline.

### 4. Execute
* Evaluated the model against training and testing datasets.
* **Business Impact:** The model provides a dependable price range for passengers, improving pricing transparency and operational predictability.

## 📂 Project Structure
* `regression_model_taxi_fare.ipynb`: The main Jupyter Notebook containing the full analysis and model.
* `dataset/`: Folder containing the NYC TLC trip data used for training and testing.

## 📦 Requirements
* Python 3.x
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
