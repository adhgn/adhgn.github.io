---
layout: default
title: Marketing Campaign Analysis
---

# Marketing Campaign Analysis
[GitHub Link](https://github.com/adhgn/301_Project/tree/main)
## Introduction
The dataset Marketing Campaign contains information about customers of a Portuguese retail company. It includes demographic, financial, and behavioural attributes that describe customer purchasing habits and campaign responses.

**Research Question:**

We want to examine the association between whether a customer accepts the latest marketing campaign offer (response) and predictors related to demographic characteristics (e.g., income, age, marital status, family composition) and behavioural characteristics (e.g., spending on different product categories, purchase channels, website visits, and past campaign responses).

## Method and Result
**Logistic Regression**

Logistic regression is appropriate because our response variable, whether the customer accepted the last campaign offer (1 = yes, 0 = no), is binary. This method models the probability of acceptance as a function of demographic variables and behavioural factors, providing interpretable effects in terms of odds ratios.

**Variable Selection**

To identify an optimal model, we use `stepAIC` with backward elimination for variable selection. The selected model included a smaller set of variables, such as education level, marital status, Teenhome, Recency, several spending variables (`MntWines`, `MntMeatProducts`, `MntGoldProds`), and purchase behaviours (`NumDealsPurchases`, `NumCatalogPurchases`, `NumStorePurchases`, `NumWebVisitsMonth`). In contrast, variables such as `Income`, `Kidhome`, and several product spending categories did not meaningfully improve the model and were excluded.

## Key Takeaways
The selected model is preferred as the final model because it provides a clearer and more concise explanation of campaign acceptance while maintaining excellent fit. With 16 predictors instead of 24 (a 33% reduction), it achieves nearly identical model performance. The residual deviance ($801.54$) and AIC ($835.54$) remain close to those of the full model, and the likelihood ratio test confirms that the full model does not offer a significantly better fit ($p = 0.89$).

By removing non-significant variables, the final model highlights the key demographic, behavioural, and spending factors that truly drive campaign acceptance, offering stronger interpretability without sacrificing predictive ability.

## Dataset
[Kaggle](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis/data)
