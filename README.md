# Credit_Risk_Analysis
## Overview
This study uses sklearn library, pandas & python to develop different machine learning models to predict credit applications status using individual applicants data.
### Background
The dataset used to train & develop the models is from Q1 loans data in 2019, the dataset can be found in the following link:
https://github.com/Lamismn/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources%20(1)/LoanStats_2019Q1.csv

The dataset is cleaned & reshaped using different methods to drop null cells, & rehsape Boolean data to binary inputs. This allows the regression models to understand & predict the dataset.

The dataset is afterwards divided into two sets, a training & testing sets to train & test the different models. Then different sampling methods are used to compare them & test the accuracy of each model.

## Results
Because the dataset is imbalanced, (51352 accepted loans Vs 260 unaccepted), we used different oversampling & undersampling techniques to make up for the imbalance, the results of the different methods are as follows


