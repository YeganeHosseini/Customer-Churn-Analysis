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
- **Feature Engineering (Optional)**: Creating new features that may enhance model performance.
- **Predictive Modeling (Optional)**: Using machine learning techniques to predict customer churn.

## Setup and Installation

To run this project on your local machine, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your_username/your_repository_name.git
   cd your_repository_name
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv env
   ```

3. **Activate the Virtual Environment**:
   - On Windows:
     ```bash
     .\env\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source env/bin/activate
     ```

4. **Install the Required Packages**:
   ```bash
   pip install -r requirements.txt
   ```

5. **Run the Jupyter Notebook** (Optional):
   ```bash
   jupyter notebook
   ```

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

## Future Work

- **Feature Engineering**: Create additional features such as tenure groups or charge groups to enhance model predictions.
- **Predictive Modeling**: Build and evaluate a predictive model to identify customers at risk of churning.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your changes. Feedback and improvements are always welcome.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
