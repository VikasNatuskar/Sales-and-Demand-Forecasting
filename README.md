                ****AI Capstone Project****
**Retail – Demand and sales Forecasting** 

DESCRIPTION
**Problem Statement**
      •	Demand Forecast is one of the key tasks in Supply Chain and Retail Domain in general. It is key in effective operation and optimization of retail supply      chain. Effectively solving this problem requires knowledge about a wide range of tricks in Data Sciences and good understanding of ensemble techniques. 
      •	You are required to predict sales for each Store-Day level for one month. All the features will be provided and actual sales that happened during that month will also be provided for model evaluation. 

Dataset Snapshot
Training Data Description: Historic sales at Store-Day level for about two years for a retail giant, for more than 1000 stores. Also, other sale influencers like, whether on a particular day the store was fully open or closed for renovation, holiday and special event details, are also provided. 
 
 
Project Task: Week 1

    Exploratory Data Analysis (EDA) and Linear Regression:
1.	Transform the variables by using data manipulation techniques like, One-Hot Encoding 
2.	Perform an EDA (Exploratory Data Analysis) to see the impact of variables over Sales.
3.	Apply Linear Regression to predict the forecast and evaluate different accuracy metrices like RMSE (Root Mean Squared Error) and MAE(Mean Absolute Error) and determine which metric makes more sense. Can there be a better accuracy metric?
•	Train a single model for all stores, using storeId as a feature.
•	Train separate model for each store.
•	Which performs better and Why? [In the first case, parameters are shared and not very free but not in second case]
•	Try Ensemble of b) and c). What are the findings?
•	Use Regularized Regression. It should perform better in an unseen test set. Any insights?
•	Open-ended modeling to get possible predictions.
    Other Regression Techniques:
4.	When store is closed, sales = 0. Can this insight be used for Data Cleaning? Perform this and retrain the model. Any benefits of this step?
5.	Use Non-Linear Regressors like Random Forest or other Tree-based Regressors.
•	Train a single model for all stores, where storeId can be a feature.
•	Train separate models for each store.
Note: Dimensional Reduction techniques like, PCA and Tree’s Hyperparameter Tuning will be required. Cross-validate to find the best parameters. Infer the performance of both the models. 
6.	Compare the performance of Linear Model and Non-Linear Model from the previous observations. Which performs better and why?
7.	Train a Time-series model on the data taking time as the only feature. This will be a store-level training.
•	Identify yearly trends and seasonal months
 
Project Task: Week 2

    Implementing Neural Networks:
1.	Train a LSTM on the same set of features and compare the result with traditional time-series model.
2.	Comment on the behavior of all the models you have built so far
3.	Cluster stores using sales and customer visits as features. Find out how many clusters or groups are possible. Also visualize the results.
4.	Is it possible to have separate prediction models for each cluster? Compare results with the previous models.
Applying ANN:
5.	Use ANN (Artificial Neural Network) to predict Store Sales.
•	Fine-tune number of layers,
•	Number of Neurons in each layers.
•	Experiment in batch-size.
•	Experiment with number of epochs. Carefully observe the loss and accuracy? What are the observations?
•	Play with different  Learning Rate  variants of Gradient Descent like Adam, SGD, RMS-prop.
•	Which activation performs best for this use case and why?
•	Check how it performed in the dataset, calculate RMSE.
6.	Use Dropout for ANN and find the optimum number of clusters (clusters formed considering the features: sales and customer visits). Compare model performance with traditional ML based prediction models. 
7.	Find the best setting of neural net that minimizes the loss and can predict the sales best. Use techniques like Grid search, cross-validation and Random search.
