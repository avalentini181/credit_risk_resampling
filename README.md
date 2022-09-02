# credit_risk_resampling

# Overview of the Analysis

I was tasked with using various techniques to train and evaluate models with imbalanced classes. I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. Using my knowledge of the imbalanced-learn library, I used a logistic regression model to compare two versions of the dataset. Logistic regression analysis is valuable for predicting the likelihood of an event. It helps determine the probabilities between any two classes. The dataset had information about the clients loan size, intrest rate, income, debt to income and etc. however, the most important section in the dataset was loan status. The loan status had two categories it showed on a client either a healthy loan (0) or high-risk loan (1). I wanted my models to be able to predict whether a client would be a healthy loan or a high risk loan. When performing a value count on the loan status I was able to see that the healthy loans outnumber the highrisk loans. To ensure that the model I create is best one therefore, I created two models one using the original data provided while the other I used a resampling method technique. This was to reduces the variance between the two categories and see if we can get a more accurate result. 

# Results
Precision quantifies the number of positive class predictions that actually belong to the positive class. The F1-score is one of the most important evaluation metrics in machine learning. It elegantly sums up the predictive performance of a model by combining two otherwise competing metrics — precision and recall.

Machine Learning Model 1:
- Healthy loans:
    * Precision: 1.00
    * f1 score: 1.00
- High-risk loans:
    * Precision: 0.85
    * f1 score: 0.88
  
Machine Learning Model 2:
 - Healthy loans:
    * Precision: 1.00
    * f1 score: 1.00
 - High-risk loans:
    * Precision: 0.84
    * f1 score: 0.91

# Summary

From the two models created I believe that the resampling model performs the best out of the two. This can be seen by looking at the classification report showing that the second model has a better f1 score compared to the the first model with the original data. This shows that the second model is able to detect more high-risk loans than the first model. In this case performance does depend on the problem we are trying to solve which is to see if the client would be a healthy loan or a high-risk loan. I personally would recommend the second model until you have more data for high-risk loans that you can add to the original dataset.
