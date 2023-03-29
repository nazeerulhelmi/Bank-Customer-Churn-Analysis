# Bank Customer Churn Analysis (Power BI)
To identify the churn rate, identify the factors contributing to churn rate

Steps taken:
  - Get familiar with the raw data available (.csv file)
  - Performed data preparation and cleaning
    - Connect the raw data into Power BI
    - Launch Power Query to transform the data
    - Rename columns name
    - Ensure correct data types and make changes where necessary
    - Replaced or converted values into a meaningful text
    - Created 3 new columns to assign certain data columns into a categories/groups e.g. age 25 into an age group 21-30
      - Age groups, Credit score, Account balance
  - Created measures using DAX
    - Customers lost = CALCULATE(COUNT('Customer Data'[Churn Status]), 'Customer Data'[Churn Status] = "CHurned")
    - Churn rate = 'Customer Data'[Customers Lost] / 'Customer Data'[Customers]
  - Data visualization
    - Customers by gender
    - Customers by Activity Status
    - Customers by Credit Card Status
    - Customers by Country
    - Customers by Products
    - Customers and Churn Rate by Age Groups
    - Customers and Churn Rate by Credit Scores
    - Customers and Churn Rate by Account Balance

Some of the insights:
  - The churn rate is 20.4% equivalent to 2037 customers
  - 7055 customers owned a credit card and has 20.2% churn rate
    - In the age category, age group of 51-60 contributed 54.9% of the churn rate
    - In the credit scores category, unsurprisingly, higher credit scores contributed to lesser churn rate
  
