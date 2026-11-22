## Project Title
**Smart City Mobility: Bicycle Rental Demand Prediction Using Multiple Linear Regression**

## 1. Activity Description
The objective of this activity is to predict a continuous target value using two or more input features through Multiple Linear Regression.

In this project, bicycle rental demand is predicted using weather conditions, time and seasonal factors. A single-feature regression model is first developed as a baseline and then compared with a Multiple Linear Regression model to determine whether using additional features improves prediction performance.

The activity also includes manual regression calculations on a small sample, coefficient interpretation, multicollinearity analysis, residual analysis, model evaluation and prediction for a new example.

## 2. Dataset Information
- **Dataset Name:** Seoul Bike Sharing Demand Dataset
- **Source:** UCI Machine Learning Repository
- **Dataset Link:** https://archive.ics.uci.edu/dataset/560/seoul+bike+sharing+demand
- **Original Dataset Size:** 8,760 records and 14 columns
- **Records Used:** 8,465 records after excluding non-functioning days
- **Target Variable:** `Rented_Bike_Count`

The dataset contains hourly bicycle rental records along with weather information, time, seasons and holiday details.

## 3. Input Features and Target
**Input Features (X):**
- Hour
- Temperature
- Humidity
- Wind Speed
- Visibility
- Dew Point
- Solar Radiation
- Rainfall
- Snowfall
- Season (One-Hot Encoded)
- Holiday (One-Hot Encoded)

**Target Variable (y):** `Rented_Bike_Count`

The target represents the number of bicycles rented during an hour.

## 4. Work Completed
The following steps were performed as part of the activity:

1. Selected and explored the Seoul Bike Sharing Demand Dataset.
2. Inspected the dataset structure, data types, missing values and duplicate records.
3. Cleaned and prepared the dataset for modelling.
4. Performed Exploratory Data Analysis using statistical summaries and visualisations.
5. Examined feature relationships using correlation analysis.
6. Prepared a small sample and design matrix for manual regression calculations.
7. Implemented a Single Linear Regression model using Temperature as the input feature.
8. Implemented a Multiple Linear Regression model using multiple input features.
9. Used an 80:20 chronological train-test split.
10. Applied feature scaling using StandardScaler.
11. Interpreted regression coefficients while keeping other features constant.
12. Checked multicollinearity using Variance Inflation Factor (VIF).
13. Analysed residuals using residual plots and a residual distribution histogram.
14. Evaluated and compared model performance.
15. Predicted bicycle rental demand for a new sample.

## 5. Model Evaluation and Results

The models were evaluated on the testing dataset.

| Metric | Multiple Linear Regression |
|---|---:|
| MAE | 317.29 |
| MSE | 187977.36 |
| RMSE | 433.56 |
| R² Score | 0.4767 |
| Adjusted R² | 0.4726 |

### Comparison of Models

| Model | Testing R² |
|---|---:|
| Single Linear Regression | 0.0442 |
| Multiple Linear Regression | 0.4767 |

Multiple Linear Regression performed better than the single-feature model, indicating that using multiple input features improved the model's ability to explain bicycle rental demand.

## 6. New Sample Prediction
The trained Multiple Linear Regression model was used to predict bicycle rental demand for a new example containing weather and time-related features.

**Predicted Bicycle Rental Count:** Approximately 1,227 bicycles.

## 7. Conclusion
The activity demonstrates how Multiple Linear Regression can be used to predict bicycle rental demand using multiple input features.

The model achieved an R² score of 0.4767 and an Adjusted R² score of 0.4726. Compared with Single Linear Regression, the Multiple Linear Regression model showed better performance.

The analysis also highlighted multicollinearity among some input features, showing the importance of checking model assumptions and interpreting results carefully.

## 8. Project Files
This repository contains:
- **Jupyter Notebook:** Complete implementation, calculations, visualisations and model evaluation.
- **Prepared Dataset:** CSV file used for modelling.
- **README.md:** Activity description, dataset information, workflow and results.

## 9. Faculty GitHub ID
##Submission GitHub ID: [https://github.com/complexiota](https://github.com/complexiota)
##Student project url: https://github.com/Anushree-Gire/RCA_CIE2_Activity1_Linear_Regression_AD3356
---

**Activity:** Multiple Linear Regression  
**Domain:** Machine Learning – Supervised Learning  
**Algorithm:** Single Linear Regression and Multiple Linear Regression
