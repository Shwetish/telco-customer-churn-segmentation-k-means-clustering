# telco-customer-churn-segmentation-k-means-clustering
K-Means clustering analysis on telecom customer behavior and churn indicators to uncover high-risk subscriber segments and pinpoint retention factors.

# Telco Customer Churn Segmentation

## 1. Business Problem
* **1.1. Business Objective:** Segment telecom customers using service utilization metrics, contract types, and billing information to isolate behavioral profiles susceptible to churn.
* **1.2. Constraints:** Mixed dataset containing both high-cardinality categorical data and numerical charges requiring dummy encoding and normalization.

## 2. Data Dictionary
| Feature | Data Type | Description |
| :--- | :--- | :--- |
| `customerID` | Object | Unique customer identifier. |
| `tenure` | Integer | Number of months the customer has stayed with the company. |
| `MonthlyCharges` | Float | The amount charged to the customer monthly. |
| `TotalCharges` | Float | Total amount charged to the customer. |
| `Contract` | Object | Contract term (Month-to-month, One year, Two year). |
| `Churn` | Object | Whether the customer churned or not (Yes/No). |

## 3. Exploratory Data Analysis (EDA)
* **3.1. Summary:** Summarized numerical attributes and churn frequencies.
* **3.2. Univariate Analysis:** Analyzed tenure lengths, monthly fees, and contract distributions.
* **3.3. Bivariate Analysis:** Investigated relationship trends between month-to-month contracts, higher monthly charges, and churn incidence.

## 4. Data Pre-processing
* **4.1. Data Cleaning & Feature Engineering:** Imputed missing values in total charges, dropped ID columns, applied one-hot encoding to categorical variables, and standardized numerical scales.

## 5. Model Building
* **5.1. Model Execution:** Developed K-Means clustering models on the engineered feature space.
* **5.2. Scree Plot:** Generated Elbow curves to determine the ideal cluster count.
* **5.3. Validation & Insights:** Validated clusters against actual churn labels to identify high-risk segments (e.g., short-tenure, high-bill customers on month-to-month plans).

## 6. Business Benefits & Impact
* Enables retention teams to proactively deploy targeted discounts, contract upgrade incentives, and specialized customer service support to vulnerable segments before they cancel.
