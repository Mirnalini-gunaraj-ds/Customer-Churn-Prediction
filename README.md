Predictve Analysis of Customer Retention/Churn

Business Problem: This study will assess their dataset and discuss how to construct a model in order to anticipate the bank's future clients who are interested in acquiring a product. The goal is to boost earnings and stop overpaying.

Problem Synopsis Create a categorization model based on consumer personal data, marketing campaign data, and economic background characteristics to forecast prospective customers who could be interested in signing up for a term deposit.

Resolution Algorithms for data mining : SVM, GBDT, Decision Trees, and Logistic Regression

Performance assessment:
  There was a trade-off between enhancing the outcomes and taking precision (TP/(TP+FP)) and recall (TP/(TP+FN)) into consideration. In this study, "false positive" (FP) refers to a "false" client who ultimately declines to buy the product; "true negative" (FN) refers to a potential customer who eventually subscribes to the product and is forecasted as negative (0) in the model (+1). The bank would suffer a significant loss if "true" potential customers were overlooked. Additionally, it would be a waste of time and human resources to call "false" potential clients. As a result, I ultimately chose to use recall to assess the performance of the model and the F1 score (2*(Recall * Precision) / (Recall + Precision)) as a backup.

OneHotEncoding

Imbalanced dataset I applied oversampling method by duplicating some of the original samples of the minority class.

Training models (including tuning hyperparameters) Models

Summary 
  
A feature's importance is checked In summary In conclusion, out of all the models, I decided on gradient boosting since it yielded the highest recall. As a key performance indicator, recall is crucial in actual business concerns. The bank would benefit from higher profits and lower overhead. I wanted to let the bank's marketing department know how important the qualities I discovered throughout the data analysis were after I had chosen the best model. (1) "Euribor3m" indicates that a high interest rate influences consumers' decisions in a favorable way.
