# Customer Churn Analysis

## Project Overview

This project aims to analyze customer churn data from a telecommunications company to identify key factors influencing customer churn. The analysis involves data cleaning, exploratory data analysis (EDA), and visualization to uncover patterns in customer behavior. Insights derived from this analysis can help the company develop strategies to reduce churn and improve customer retention.

## Dataset

The dataset used in this project is the **Telco Customer Churn** dataset, which contains information about customers, their demographics, services they have subscribed to, and whether they have churned. The dataset includes the following key features:
- `customerID`: Unique identifier for each customer.
- `tenure`: Number of months the customer has stayed with the company.
- `MonthlyCharges`: The amount charged to the customer monthly.
- `TotalCharges`: The total amount charged to the customer.
- `Churn`: Indicates whether the customer has churned (`Yes`) or not (`No`).

## Project Structure

- **Data Cleaning**: Handling missing data and converting data types.
- **Exploratory Data Analysis (EDA)**: 
  - Analyzing the distribution of churn.
  - Investigating relationships between tenure, charges, and churn.
  - Visualizing the data using histograms, box plots, and scatter plots.
- **Feature Engineering**: Creating new features that may enhance model performance.
- **Predictive Modeling**: Using machine learning techniques to predict customer churn.


## Analysis and Results

### Data Cleaning

- Missing values were found in the `TotalCharges` column, which were handled by dropping rows with missing values.
- The `TotalCharges` column was converted from an object to a numeric data type.

### Exploratory Data Analysis (EDA)

- **Churn Distribution**: The dataset shows an imbalance in the churn classes, with fewer customers having churned.
- **Tenure Analysis**: Customers with shorter tenure are more likely to churn.
- **Charges Analysis**: Higher monthly charges appear to correlate with a higher likelihood of churn.

### Visualizations

The project includes several key visualizations:
- Distribution of churn across the dataset.
- Tenure distribution and its relationship to churn.
- Monthly and total charges and their impact on churn.
- 
### Feature Engineering
- Create additional features that could improve model performance.
- Examples include categorizing tenure into groups, calculating the average monthly charges per tenure, or combining categorical features to create interaction terms.
### Predictive Modeling

- A Logistic Regression model was trained to predict customer churn.
- The model achieved an overall accuracy of 80%.

### Classification Report Analysis

- **Class 0 (Non-Churn)**: 
  - **Precision**: 0.84 - The model correctly identified 84% of the non-churn predictions.
  - **Recall**: 0.90 - The model captured 90% of actual non-churn customers.
  - **F1-Score**: 0.87 - Indicates strong overall performance in predicting non-churn.
  
- **Class 1 (Churn)**: 
  - **Precision**: 0.66 - The model correctly identified 66% of the churn predictions.
  - **Recall**: 0.52 - The model captured 52% of actual churned customers, indicating room for improvement.
  - **F1-Score**: 0.58 - The model struggles more with predicting churn compared to non-churn.

- **Macro Average**:
  - **Precision**: 0.75 - Reflects moderate performance across both classes.
  - **Recall**: 0.71 - Indicates the model's overall ability to capture both churn and non-churn.
  - **F1-Score**: 0.73 - Balances precision and recall across both classes.
  
- **Weighted Average**:
  - **Precision**: 0.79, **Recall**: 0.80, **F1-Score**: 0.79 - Weighted by support, showing that the model performs better overall on the majority class (non-churn).

### Future Work

- **Improving Churn Prediction**:
  - Implement resampling techniques to address class imbalance.
  - Explore alternative models such as Random Forest, Gradient Boosting, or ensemble methods.
  - Conduct further feature engineering to enhance model performance.


## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your changes. Feedback and improvements are always welcome.
