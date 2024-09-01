# SYRIA TELECOMMUNICATIONS LIMITED
*An analysis of the high churn rate experienced by Syria Tel*

![telecomm](https://github.com/juliettmwaura/Phase-3-Project/blob/main/images/tel%203.jpg)

## Overview

The telecommunication industry plays a huge role in our daily lives thus stiff competition as the growth and technology expands. While acquiring new customers is important, telecommunication companies recognize that retaining existing ones is even more crucial. Customer churn, is defined as the rate at which subscribers switch to competitors, is a major concern in this industry.

## Business and Data Understanding

### Business Understading

Given the fierce competition in the telecom sector, understanding the reasons behind customer departures, whether related to pricing, service quality, customer experience, or competitor tactics, is crucial.
This analysis will enable SyriaTel to identify and rectify underlying problems, ultimately mitigating further churn and fostering long-term profitability and customer loyalty.


**Business Problem and Challenge**

Syria Telecommunications faces a risk of high rates of customer churn that will affect not only profitability but also company reputation and business standing. The projects seeks to develop a model that will predict the rate of customer churn and provide recommendations that will improve.

**Objectives**

Our objective are

1. Identify the factors that contribute to customer churn
2. To build a model that predicts customer churn
3. To draw conclusions and recommendation for customer retention


### Data Understanding

The data was sourced from Kaggle and was stored in a CSV file format.
The data contained 3,333 rows and 21 records.

Key Features include:

> - Minutes and Calls – Consumer’s purchase of minutes and calls made to the domestic and international regions
> - Charges – Charges billed to consumers for making their domestic calls during the day, evening and night, and international calls.
> - Subscriptions – A binary value indicating if the consumer has an international plan or a voice mail
> - Customer Service Calls – Number of times a user has called the customer service
> - Churn - This binary feature indicates if the user left the company.
> - Account Length – period of time the user maintained their account.

### Data Cleaning

The data received had no missing values and no duplicate values. Records were well kept.

Some cleaning aspects done:

> - Conversion of numerical features to categorical.
> - Conversion of boolean features to strings.
> - Droping features.

## Data Analysis

**_Churn_**

![churn_rate](https://github.com/juliettmwaura/Phase-3-Project/blob/main/images/churn_dist.png)

> Nearly 15% of customers churned in the period.


## Modelling

_Preprocessing steps_ followed in this model include:

1. LabelEncoding - conversion of values to a certain predefined label
2. OneHotEncoding - encodes any categorical features.
3. StandardScaling - scales all the numerical features.

_Models_ explored in this project include:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier

Each model's advantages and disadvantages are highlighted to give caution to the reader.

## Evaluation

Evaluation metrics for this model focused primarily on recall.

Each model was given the same set of data and the models competitively scored the test data after training their models before any hyper parameter tuning.

The best models for this project were Random Forest Classifier and the XGBoost. These classifiers were then tested further after hyper parameter tuning and finding the best train-test ratios that maximised the accuracy.

After hyperparameter tuning and picking the right train-test split value, the RandomForest gave us the metrics we required as per the objectives we set out to achieve.


## Conclusion and Recommendations

The high recall score from the RandomForest Classifier means that the model can identify many customers who churn as true positive values, with very few customers being misclassified as non-churners.

Recommendations to ensure Syria Telecommunications retaining of the 80% predicted churners could include but are not limited to:

- Bespoke packages, Incentives and Rewards 
- Trained Customer Service Agents and Customer Feedback Recording
- Re-evaluation of price points.

---
Authored by [Juliet Mwaura]