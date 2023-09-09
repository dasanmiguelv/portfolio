---
title: "BigData Whit BigQuery"
description: "Google Analytics records for the Google Merchandise Store loaded into BigQuery"
dateString: Sep 2023
draft: false
tags: ["GCP", "BigQuery ML", "SQL", "XBoost", "logistic_reg", "Google Analytics"]
showToc: false
weight: 204
cover:
    image: "mL-Engineer-on-GCP/BigQuery-ML/bqml.jpg"
--- 
### 🔗 [View code on Github](https://github.com/dasanmiguelv/ML-Engineer-on-GCP/tree/main/Big%20Data%20-%20BigQuery/scripts)

## Description
The Google Analytics Sample Ecommerce dataset that has millions of Google Analytics records for the Google Merchandise Store loaded into BigQuery. In this lab, I used this data to run some typical queries that businesses would want to know about their customers' purchasing habits. Each row within a table corresponds to a session in Analytics 360.

Objectives:

#### In this Lab we look for predict which new visitors will come back and purchase, through the following tasks.

* Use BigQuery to find public datasets
* Query and explore the ecommerce dataset
* Create a training and evaluation dataset to be used for batch prediction
* Create a classification (logistic regression) model in BigQuery ML
* Evaluate the performance of the machine learning model
* Predict and rank the probability that a visitor will make a purchase

## Outcome

After evaluating the model I got a roc_auc of **0.72**, which shows that the model has not great predictive power.
I Added some new features and create a second machine learning model, a key new feature that was added to the training dataset query is the maximum checkout progress each visitor reached in their session.
With this new model I got a roc_auc of **0.91** which is significantly better than the first model.

## Conclusion

BigQuery ML (BigQuery machine learning) is a feature in BigQuery where data analysts can create, train, evaluate, and predict with machine learning models with minimal coding.