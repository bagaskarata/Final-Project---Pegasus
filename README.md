
# Final Project : Term Deposit Conversion Rate (Prediction & Analysis)
## Background and Objective 
* Term deposits are a major source of income for a bank. One of the most effective way to reach out customer is using teleponic marketing. However, a huge investment is required to do this method.
* To address the issue, it is required the data science team to make a model that can predict whether a customer will take the term deposit or not. By then, marketers will call the predicted of convert customers only.
* * Use 5 alghoritms (Logistic Regression, Decision Tree, KNN, Random Forest, XGBoost) and evaluate models using AUC and Precision value. By the end, will choose alghoritm with the best AUC and Precision value.

## Data Overview
* Dataset is provided by [Rakamin Team & Kaggle](https://www.kaggle.com/datasets/prakharrathi25/banking-dataset-marketing-targets)
* Features available : 7 numerical features, 9 categorical features, 1 target (categorical)
 ![image](https://user-images.githubusercontent.com/100980318/168189321-c170d4a0-3595-4ad8-ab01-b880e201046a.png)
* There is no missing value in the dataset.
* Removing 4.163 duplicates data and replacing "Unknown" data with mode.
* Handling outliers using Z-score method and handling imbalance with threshold moving method.

## EDA (Exploratory Data Analysis)
### Feature "campaign"
![image](https://user-images.githubusercontent.com/100980318/168302563-1a164437-3a3c-48a5-a044-0cacb55ab13e.png)
![image](https://user-images.githubusercontent.com/100980318/168302645-7264d53b-e8c5-498b-ae1f-6db8f9c6dff2.png)
From the graph of distribution and boxplot, the more doing campaign seems the customers do not take the term deposit (no). Campaign will be effective (customers take "yes") between 1-5x campaigns.
### Feature " duration"
![image](https://user-images.githubusercontent.com/100980318/168302715-0852cbe2-2f39-42ed-9807-562849baf3da.png)
![image](https://user-images.githubusercontent.com/100980318/168302761-593bbccd-1a98-465a-a6ca-9b91cd3366f2.png)
From the graph of distribution and boxplot, the longer marketers make a call with customer seems customers decide not to take the term deposit (no). Phone call will be effective when marketers maximize call within first 500 seconds. 
### Feature "month"
![image](https://user-images.githubusercontent.com/100980318/168302981-6a4356bb-8f94-4922-a0cd-f8df94465448.png)
The graph shows the best months to boost the phone call is in March, September, October, and December Month. Meanwhile, need more research to see how marketers could increase the conversion in other months.




 
