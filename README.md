# Customer Churn Analysis and Prediction

## Introduction

Customer churn refers to customers discontinuing their relationship or subscription with a company, impacting revenue and growth. In this dataset, churn is labeled to show whether a customer has left or stayed. Analyzing churn helps businesses identify patterns and factors contributing to customer loss and develop strategies to retain them.

## Project Objective

The main objective of this project is to understand the factors contributing to customer churn and to develop a predictive model to identify customers at risk of churning. By leveraging statistical methods and machine learning techniques, we aim to provide actionable insights for business strategies to improve customer retention.

## Business Objective

Customer churn prediction is crucial for businesses to maintain and grow their customer base. By predicting which customers are likely to leave, companies can take proactive measures to improve customer satisfaction, offer targeted incentives, and ultimately reduce churn rates, leading to sustained revenue and growth.

## Dataset Description

The dataset contains information about customers and their interactions with the company. It is used to analyze customer churn and build predictive models.

**Dataset Source:** [Kaggle Customer Churn Dataset](https://www.kaggle.com/datasets/muhammadshahidazeem/customer-churn-dataset?resource=download)

### Training Data

- **Rows:** 440,833
- **Columns:** 17

| Column                     | Description                                                                                       |
|----------------------------|---------------------------------------------------------------------------------------------------|
| `CustomerID`               | Unique identifier for each customer.                                                             |
| `Age`                      | Age of the customer.                                                                              |
| `Tenure`                   | Duration (in months) the customer has been with the company.                                     |
| `Usage Frequency`         | How frequently the customer uses the company’s services.                                         |
| `Support Calls`           | Number of support calls made by the customer.                                                     |
| `Payment Delay`           | Indicator of whether the customer has delayed payments.                                           |
| `Total Spend`             | Total amount of money spent by the customer.                                                      |
| `Last Interaction`        | Type of the customer's last interaction with the company.                                         |
| `Churn`                    | Whether the customer has churned (1) or not (0).                                                 |
| `Gender`           | Indicator for female gender.                                                                       |
| `Subscription Type` | Indicator for basic subscription type.                                                            |
| `Contract Length`  | Indicator for an annual contract length.                                                           |

## Repository Contents

- **`Customer Churn Prediction.ipynb`**: Jupyter Notebook containing the code for data processing, model building, and evaluation.
- **`Dataset Desc.pdf`**: Detailed description of the dataset, including feature explanations.
- **`train.csv`**: Training dataset used for model training.
- **`test.csv`**: Test dataset used for model evaluation.
- **`Dashboard.png`**: Visualization dashboard depicting data exploration and insights.

## Project Workflow

1. **Import Libraries and Load Data:**
   - Ensure all necessary tools and datasets are ready.

2. **Data Exploration and Visualization:**
   - Understand data structure, distribution, and relationships.

3. **Data Preprocessing:**
   - Handle missing values, feature selection, and standardization.

4. **Model Building and Training:**
   - Build, train, and evaluate the logistic regression model to predict customer churn.

5. **Model Interpretation and Insights:**
   - Interpret results and derive actionable insights from the model.

## Results

- **Model:** Logistic Regression
- **Classification Report:**

  | Metric       | Value  |
  |--------------|--------|
  | **Precision for Churn (1)** | 0.93   |
  | **Recall for Churn (1)**    | 0.89   |
  | **F1 Score for Churn (1)**  | 0.91   |
  | **ROC-AUC Score**          | 0.96   |

- **Confusion Matrix:**

  |                  | Predicted No Churn (0) | Predicted Churn (1) |
  |------------------|-----------------------|--------------------|
  | Actual No Churn (0)| 34,610                | 3,533              |
  | Actual Churn (1)  | 5,594                 | 44,430             |

## Conclusion

- The predictive model successfully identifies customers at risk of churning with high accuracy and AUC-ROC score.
- Key features influencing churn include "Contract Length_Monthly", "Support Calls", and "Payment Delay".
- Businesses can leverage these insights to design targeted strategies for customer retention and reduce churn rates.

## How to Run the Code

1. Clone the repository:
   ```sh
   git clone https://github.com/riskaamylatulaskiyah/Customer-Churn-Analysis-and-Prediction.git
   cd customer-churn-analysis
