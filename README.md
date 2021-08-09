
## Problem Statement


It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.
We have to predict fraudulent and non fraudulent transactions.

---

## Data Source

Machine Learning Group - ULB - Kaggle - https://www.kaggle.com/mlg-ulb/creditcardfraud

---

## Data Description

1. The dataset contains transactions made by credit cards in September 2013 by European cardholders.
2. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
3. It contains only numerical input variables which are the result of a PCA transformation. This is due to confidentiality issues.
4. The only features which are not transformed are Time and Amount.

---

## Conclusions



- Irrespective of Imbalanced Dataset, we were able to achieve good scores.

- It is recommended to improve the data collection process so that target feature classes can be equal.

- Random Forests and XGBoost gave us the best result with Random Forest being on the top. They both were able to detect more than 80% of the Fraudulent Transactions and at the same time not classifying a lot of non fraud classes as fraud.

- As we saw that with Logistic Regression, the recall was the highest. However, the precision and the f1_score were both really poor. We had to come up with a model where both recall and precision were good. So as we trained the model with Random Forests, the recall score decreased a little but the precision score shot up significantly.

- Hence there is no perfect model. There will always be such trade offs and we have to select which performance metric to give importance to depending on our usecase.

