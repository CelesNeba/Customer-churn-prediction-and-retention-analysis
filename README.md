# Customer-churn-prediction-and-retention-analysis
The goal of this project is to analyze customer behavior, identify key churn drivers, and build a predictive model to help business stakeholders retain customers effectively.

## Problem Statement 

A company is experiencing a decline in revenue due to a high rate of customer churn, the phenomenon where customers stop using the company’s products or services. This poses a significant threat to the company’s growth and profitability. The company seeks to understand why customers are leaving and to identify actionable strategies to retain valuable customers. By analyzing historical customer data and predicting which customers are at risk of churn, the company aims to reduce churn, improve customer retention, and increase overall profitability.


### Tools to be used in this project

1.	Excel / CSV: Store and manage the raw customer churn dataset. Easy to inspect, filter, and export data for analysis.

2. Jupyter Notebook (Python):

- Perform data cleaning, exploratory data analysis (EDA), and preprocessing.

- Build and evaluate the churn prediction model.

- Document code and visualizations step-by-step.

3. Power BI:

- Visualize insights for business stakeholders.

- Create charts, graphs, and dashboards to highlight churn trends and drivers.




## 📊 Dataset: Customer Churn 2000

The dataset used in this project is a synthetic but realistic dataset of customer behavior and churn for a subscription-based company. It contains **2,000 customer records** with demographic, service, and billing information, which can be used to analyze churn patterns and build predictive models.

### 📥 Download
You can download the dataset here:  
[customer_churn_2000.csv](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/customer_churn_2000.csv)

### 🧾 Dataset Description

| Column | Description |
|--------|-------------|
| `CustomerID` | Unique identifier for each customer |
| `Gender` | Customer gender (Male, Female) |
| `SeniorCitizen` | 0 = No, 1 = Yes |
| `TenureMonths` | Number of months the customer has stayed with the company |
| `Contract` | Type of contract (Month-to-month, One year, Two year) |
| `InternetService` | Type of internet service the customer uses |
| `PaymentMethod` | Method used to pay the bill |
| `MonthlyCharges` | Monthly payment amount |
| `TotalCharges` | Total amount paid over tenure |
| `Churn` | Target variable: whether the customer left the service (Yes/No) |

### 🧠 Usage

This dataset is suitable for:

- Exploratory data analysis (EDA)  
- Feature engineering and model training  
- Churn prediction modeling  
- Business dashboard and retention analysis

**Note:** The dataset is clean and formatted as CSV, ready to be used in Excel, Jupyter Notebook, or Power BI.

### Data cleaning

- Handle missing values

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Handle%20missing%20values.PNG)


- Remove duplicates

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/drop%20duplicates.PNG)


- Encode target variable

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Encode%20target%20variables.PNG)


###  Exploratory Data Analysis (EDA)

- Churn Rate

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/churn_rate%20(EDA).PNG)


- Plot churn distribution

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Churn%20distribution.PNG)


- Check churn by Key features. Example: by contract type, tenure, or gender:

- Code:


![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Churn%20by%20key%20features%20code.PNG)












  #### Churn by Contract Type

  ![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/churn%20by%20contract%20typ%20bar%20chart.PNG)








  #### Tenure vs Churn



  ![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Tenue%20vs%20churn%20chart.PNG)





  #### Churn By InternetService

  ![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/churn%20by%20intenet%20service%20bar%20chart.PNG)





#### Churn by monthly charges 

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/churn%20by%20monthly%20charges%20bar%20chart.PNG)


    








  ### Feature preparation for modeling

  


- Split features & target

  ![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Split%20Features%20%26%20Target%20image.PNG)






### Build a simple churn prediction model

- Logistic regression

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Logistic%20regression%20image.PNG)



- Model evaluation

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Model%20Evaluation%20image.PNG)


![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Model%20Evaluation%20image2.PNG)



- Feature importance (Top drivers)

![](https://github.com/CelesNeba/Customer-churn-prediction-and-retention-analysis/blob/main/Feature%20Importance%20(Top%20Drivers)%20image.PNG)



#### Business insights summary from the model

The churn model’s performance indicates that the current customer data does not yet provide strong enough signals to reliably predict churn. The model correctly identifies some customers at risk, but it also misses many churners, meaning the organization may still lose customers without warning. This suggests that churn is influenced by additional factors that are not yet captured in the dataset. To improve retention outcomes, the business should focus on collecting richer customer behavior data and strengthening churn-related features before relying on predictive automation.


### Export results for dashboard

- Save predictions file


 ### Power BI Dashboard


 ![](https://github.com/CelesNeba/Fraud-detection-in-financial-transactions/blob/main/Churn_Analysis_Dashboard.PNG)


