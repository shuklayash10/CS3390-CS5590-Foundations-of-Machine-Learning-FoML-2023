# Readme File

## Data Collection and Analysis for Food Consumption Time

### Introduction
This project aims to collect and analyze data on the time taken to finish food consumption in a mess, including waiting time, for various meal categories such as breakfast, lunch, tea, and dinner over a period of two weeks. The dataset will consider various features like the day of the week, time of the day, holidays, and meal category. The goal is to prepare the data, perform exploratory data analysis (EDA), create a model to predict food consumption time, and evaluate its performance.

### Data Collection
- Data for this project has been collected and stored in a CSV file named `as1.csv`.
- The dataset includes columns like `Category`, `Starting time`, `Ending time`, `Day`, `Holiday`, and `Time Taken`.

### Data Preprocessing
- The `Starting time` and `Ending time` columns have been converted to time format using the `pd.to_datetime` function.
- A scaled starting time column, `Scaled Starting Time`, has been created to normalize the starting time within specified time windows for each meal category.

### Exploratory Data Analysis
- Exploratory data analysis has been performed to understand the relationship between the scaled starting time and the time taken for each meal category.
- A polynomial regression model has been used to fit the data, and parameters have been estimated using Maximum Likelihood Estimation (MLE).

### Model Development
- A polynomial regression model has been chosen to fit the data, as the relationship between the scaled starting time and time taken is not linear.
- The negative log-likelihood function for polynomial regression has been defined to estimate the parameters using MLE.
- The model has been trained on 80% of the data.

### Model Evaluation
- The trained model has been used to make predictions on 20% of the collected data.
- Mean Squared Error (MSE) and R-squared (R2) score have been used as evaluation metrics.
- The performance of the polynomial regression model has been compared with a linear regression model implemented using scikit-learn.

### Code Structure
The code is divided into several sections:
1. Data loading and preprocessing.
2. Polynomial regression model definition and parameter estimation.
3. EDA and plotting of the fitted curves.
4. Model training and evaluation.
5. Plotting the combined fitted curve for all categories.

### Usage
To run the code:
1. Ensure that you have the necessary Python libraries installed, including pandas, matplotlib, seaborn, numpy, and scipy.
2. Make sure you have the `as1.csv` dataset in the same directory as the code.
3. Execute the code in a Python environment.

### Conclusion
This project provides insights into the time taken for food consumption in a mess and offers a polynomial regression model to predict consumption time based on the scaled starting time. The model's performance has been evaluated, and it outperforms a linear regression model, highlighting the non-linear nature of the data.

Sl-6 , cs23mtech

Raj Popat cs23mtech14009

Yash Shukla cs23mtech14018



