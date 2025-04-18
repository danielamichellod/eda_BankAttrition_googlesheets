# Bank XYZ's Attrition Project Analysis


![Logo](/eda_BankAttrition_googlesheets/Pictures/LogoBankXYZ.jpeg)



The aim of this project is to analyse the Bank XYZ customer's dropout rate by using a dataset from kaggle (https://www.kaggle.com/datasets/marusagar/bank-customer-attrition-insights) and showing the results in an interactive dashboard. 

## Description of the project
Churn analysis aims to identify patterns and factors that contribute to customer attrition.   
The final outcome of this project is a dashboard that displays key metrics, descriptive analyses, and interactive charts to enhance comprehension on customer behavior and why they are droping out.   
For better understanding of the terms used in this project, please note we might refer to dropout rate as attrition or churn.

## Structure of the project

GitHub Folder system
```bash
eda_BankAttrition_googlesheets/
|--DataRaw # Folder with the unprocessed data
|  |--Bank-Customer-Attrition-Insights-Data.csv
|--IMG # Folder with the image used for the dashboard
|  |--LogoBankXYZ.jpeg
|  |--Dashboard.jpeg
|--README.md
```
GoogleDrive Folder system (https://drive.google.com/drive/folders/1TG40DRokWvGCVPLF20B1koIacEc_LSLA?usp=sharing)
```bash
Dashboard_Project_CustomerAttrition_XYZMultistateBank/
|--DataRaw # Folder with the unprocessed data
|  |--Bank-Customer-Attrition-Insights-Data.csv
|  |--Dataset-Overview-for-XYZ-Multistate-Bank
|--eda_CustomerAttrition_XYZMultistateBank # Folder with the processed data and the final dashboard
|  |--CustomerAttrition_XYZMultistateBank
|--Project-Tasks 
```

## Structure of the data
The dataset overview from this project was provided directly from kaggle website. Please note that the data has been slightly modified during the analysis and some row have been added or deleted. Below you will find a short description of each column. 

- **CustomerId**: Unique randomly generated identifier for each customer.
- **Surname**: Last names of the customers. 
- **Country**: Geographical location of the customers (Spain, France, and Germany).
- **Gender**: Gender of the clients (Male or Female).
- **Age**: Age of the customers (from 18 to 92 years old).
- **Tenure**: Number of years a customer has been with the bank. 
- **CreditScore**: This feature refers to the score you get by using your credit card. Customers with higher credit scores are generally considered more financially stable and less likely to face issues with financial institutions. 
- **Balance**: Amount of money a customer holds in their bank account.
- **ProductsNumber**: Number of products (ie. savings accounts, loans, credit cards) that a customer has with the bank. 
- **CreditCardHolder**: It indicates wheter or not a customer holds a credit card with the bank. 
- **IsActiveMember**: It indicates whether a customer actively engages with the bank's services by using the bank's products and services. 
- **EstimatedSalary**: Representation of the customer's estimated annual salary.
- **Exited**: This is the target variable in the dataset, indicating whether a customer has left the bank or remained. 
- **Complain**: This column shows whether or not a customer has filed a complaint with the bank.
- **SatisfactionScore**: This represents how satisfied a customer is with the bank's complaint resolution process.
- **CardType**: This column refers to the type of credit card a customer holds, such as a standard, premium or rewards card. 
- **PointEarned**: This shows the loyalty points a customer has accumulated through the use of their credit card.
- **AgeRange**: This columns is an extension of the "Age" column to sort it by three categories: Young Adult (below 30), Adult (below 40), Middle Age (below 50) and Senior. 
- **CreditCardUsageFrequency**: This columns aims to identify how the customers use their credit card: "Used little or nothing" or "Frequently used".

## Project development
The development of the project is also included in the google drive link (https://drive.google.com/drive/folders/1TG40DRokWvGCVPLF20B1koIacEc_LSLA?usp=sharing) under "Project Tasks".

### First step
- Creation of the folders systems, pre-analysis of the dataset, data normalisation, cleaning of the dataset, verify duplicates, change columns names and delete columns that won't be relevant for the analysis. 

### Second step
- Creation of the GitHub repository, harmonise the text in the dataset, flip binary values (1,0) to (Yes, No), Delete the empty cells from the document, addition of new columns that could be relevant in the analysis and creation of pivot tables related to the client analysis. 

### Third step
- Creation of pivot tables related to the financial parameters analysis, creation of pivot tables and charts related to descriptive analysis numerical and categorical.

### Fourth step
- Creation of KPIs and selection of the relevant columns for the Dashboard, Creation of the Dashboard and of the filters in it.

### Fifth step
- Completing the README file with the explanation of the project and the descriptive analysis.

## Dashboard
![Texto alternativo](/eda_BankAttrition_googlesheets/Pictures/Dashboard.jpeg)

## Conclusions
Below are the main conclusions from the analysis:

- We are experiencing a 20% customer attrition rate.
- The analysis shows that customers with higher credit scores are generally considered more financially stable and less likely to leave the bank, as they are less likely to face issues with financial institutions. There is a low churn rate among customers that have a CreditScore between 400 and 899. On the other hand, we can see that customers with a CreditScore from 300 to 399 are all leaving. If the CreditScore is low it might be because the customers are quite new. There are very few customers in this category (only 19) but a way to make them stay in the bank will be to encourage discounts or promotions when you are a new client. 
- Another interesting point is that we may incline to think that customers with multiple products are usually more invested in the bank, making them less likely to leave. The greater the number of products, the higher the customer's commitment to the bank. In this analysis, the outcome reveals the opposite trend. Customers with 1, 3 or 4 products show a larger rate of churn. The majority of customers have either 1 or 2 products. It might be worth exploring why customers who own two products show a much lower churn rate than the others.
- Customers that have a higher bank balance (starting from 100'000) are showing a larger rate of dropout. This might be due to the competence offering better conditions for higher incomes. 
- Typically, older customers are less likely to churn because they tend to be more established with their financial institutions and may have a greater sense of loyalty. In contrast, younger customers may be more likely to switch banks, especially if they are seeking better services or offers. The result of this analysis suggest the contrary by having a higher churn rate among Middle Age and Senior category. If customers from this categories tend to leave the bank, it could be insightful to offer them products and offers to make them stay. 
- Another point worth mentioning is that customers from Germany have a higher attrition rate than the ones from Spain or France. This could be the result of more attractive offers from competing banks in the market. 

## Contributions
Your contributions are appreciated. Please feel free to reach out with any suggestions, enhancements, or corrections.  

Any kind of contribution — whether it's code, documentation, or feedback — will be appreciated. Thank you for your help and collaboration.

## Author
- Daniela - [GitHub Profile](https://github.com/danielamichellod)

