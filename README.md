# House Price Prediction Project

This project aims to help a real estate company predict house sale prices based on various property characteristics. The goal is to optimize listing prices, reduce selling time, and improve competitiveness.

## The Problem

A real estate company needs to accurately predict house sale prices to optimize their listings. Using a dataset of previously sold houses, the objective is to build a regression model that can forecast prices with a **Root Mean Square Error (RMSE) not exceeding $30,000**.

## Project Steps

1.  **Data Exploration and Cleaning**:
    * An initial analysis was performed on the `house_sales.csv` dataset to identify data types, anomalies, and missing values.
    * A robust, reusable function was developed to clean the data by handling missing values, fixing data types, and correcting incorrect entries.
    * The cleaned data was saved as `clean_house_sales.csv`.

2.  **Exploratory Data Analysis (EDA)**:
    * A summary of average house prices and their standard deviation relative to the number of bedrooms was created.
    * This summary was saved as `price_by_rooms.csv`.

3.  **Model Building and Evaluation**:
    * A **Linear Regression** model was established as a baseline. It achieved an RMSE of **$23,050**, which already meets the project's target of under $30,000.
    * To improve performance, an advanced **Gradient Boosting Regressor** model was developed and fine-tuned using Grid Search with 4-fold cross-validation.
    * The optimized Gradient Boosting model achieved a significantly lower RMSE of **$15,310**.

## Conclusion

The project successfully delivered two regression models that exceed the accuracy requirements. The advanced **Gradient Boosting model is 33% more efficient** than the baseline model, providing highly accurate price predictions. Both model results have been saved for easy interpretation.

## Files

* `house_sales.csv`: The raw dataset for the project.
* `clean_house_sales.csv`: The cleaned dataset ready for analysis and modeling.
* `price_by_rooms.csv`: A summary of average prices and standard deviations by the number of bedrooms.
* `results.xslx`: An Excel file containing the prediction results from both the Linear Regression and Gradient Boosting models.
