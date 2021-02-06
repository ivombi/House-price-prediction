# House Price Prediction using Azure ML
## Project Objective
This project was aimed at implementing the skills and knowledge gained from acquiring the Azure Data Scientist Associate certification on a real dataset. Random forest and ridge regression were the two machine learning models. Some of the core techniques used were Azure workspace, cluster and compute target, python environment, estimators and Experiment, logging metrics, Hyper-parameter tunning, model registration and deployment. 
## House Price Dataset
This a famous dataset from kaggle consisting of 79 explanatory variables capturing every aspect of residential homes in Ames, Iowa, USA. The target variable is the price of homes. 
## Methodology
The main idea was to build two estimators using Random forest and Ridge regression models. Then use these estimators to run experiments and log some metrics and other valuable information every time parameters are changed. Hyper parameter tuning was used to tune the models over a range of values for the different parameters for each estimator. All of this was done using clusters and compute target in Azure. At the end the best model was saved and deployed to consume via an API. 
## Results
Some of the key metrics used to compare both estimators were RMSE and Coefficient of determination(R2). The metric values for Random forest and Ridge were as follows:
> - RMSE: 27,177.3 vs 26,397.8
> - R2: 0.97 vs 0.93

Taking RMSE as the primary metric, Ridge regression was selected as best performing estimator due to its small value as compared to Randome forest. <br>
Model registration and deployment was done to consume as a service through an API
