# Machine-Learning-ML-Project
John Kanoru Macharia

# Table Of Contents
 - Overview
 - Business Problem
 - Method 
 - Analysis
 - Recommedations
 - Author
 
# Overview
For this project I evaluated a dataset of 20 attributes and 3333 rows containing SyraTel's churn metrics. I outline my process of identifying the top indicators of churn and creating machine learning model to predict whether or not a client will soon churn. I was able to create several machine learning classification models and compare their performance on unseen data to decide on a final predictive model that SyriaTel could deploy on their current client database. My final model utilized sklearn's Decision Tree Classifier.
 
# Business Problem 
SyriaTel is a national telecommunications company interested in reducing how much money is lost because of customers who don't stick around very long, that is, reducing their churn rate. In the telecom industry, it costs [5 times](https://towardsdatascience.com/customer-churn-in-telecom-segment-5e49356f39e50) as much to acquire new business than it does to maintain existing clients. Given this information, it is important that SyriaTel ensures that its customers do not leave the company.

![image](https://user-images.githubusercontent.com/104419109/182048311-7cb61b1a-4864-42c5-bdfa-51635c61de03.png)

# Method
This objective will be achieved by first assessing feature importance on the below attributes and determining which tend to be the strongest predictors of churn. Secondly, I will apply these attributes to the final classification model to classify at clients who pose a risk of churning presently and in the future. The final step will ultimately be the deployment of a final model on existing clients database.

# Analysis
Using sklearn's .feature_importance_, the following features seemed to have the biggest impact on churn:
 - customer service calls - the number of calls a client made to the customer service line
 - total_charge - how much a client was charged for all phone call categories (international, evening, night, and day)
 - international plan_no - the number of international plans a customer had.
Upon further investigation uinto the customer service calls feature, I discovered that atleast 80% of all cusstomers made a phone call to the customer service.
The proportion of clients making 4 or more calls account for 28% of the total churned clients. By addressing just this portion of clients, we could potentially reduce churn by up to 4%.
![Average churn](https://user-images.githubusercontent.com/104419109/182048723-22626f14-da9d-477b-b227-32edb71d11a8.png)

Additionally, price has an outsized impact on customer churn. 74% of clients getting charged $75 and up will churn.
![proportions](https://user-images.githubusercontent.com/104419109/182048804-55b51397-5afc-4527-be04-4dba27b9a757.png)

A further breakdown of charges, ascertained that cstomers spending $40 or more were more likely to churn.
![Churn rate against charges](https://user-images.githubusercontent.com/104419109/182048905-d3e3981a-fd60-4045-aeac-d49d6cde7d2b.png)

# Recommendations
Based on the analysis and results from my final model, it is clear that customer service calls and day call charges have a significant impact on customer satisfaction. SyriaTel could reevaluate its prices for day calls, track the customer service calls and introduce key performance indices(KPIs) to help avoid redundancy.

# Author
- John Kanoru Macharia
- Github :[Kanoru01](https://github.com/Kanoru01)
