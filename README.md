# Credit_Risk_Analysis
## Overview
This study uses sklearn library, pandas & python to develop different machine learning models to predict credit applications status using individual applicants data.
### Background
The dataset used to train & develop the models is from Q1 loans data in 2019, the dataset can be found in the following link:
https://github.com/Lamismn/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources%20(1)/LoanStats_2019Q1.csv

The dataset is cleaned & reshaped using different methods to drop null cells, & rehsape Boolean data to binary inputs. This allows the regression models to understand & predict the dataset.

The dataset is afterwards divided into two sets, a training & testing sets to train & test the different models. Then different sampling methods are used to compare them & test the accuracy of each model.

## Results
Because the dataset is imbalanced, (51352 accepted loans Vs 260 unaccepted), we used different oversampling & undersampling techniques to make up for the imbalance.
We also used ensemble learning techniques to train the models.
the results of the different methods are as follows:
### Resmpling methods
#### Naive Random Oversampling:
The results of the Naive random oversampling is as follows:

<img width="557" alt="ros" src="https://user-images.githubusercontent.com/79733383/123736624-71f84e80-d86f-11eb-9b80-df25ac2d1a9a.PNG">

#### Synthetic Minority Oversampling Technique (SMOTE)

The results of the Smote oversampling are as follows:

<img width="570" alt="smote" src="https://user-images.githubusercontent.com/79733383/123736855-f0ed8700-d86f-11eb-803e-88cb7af7f76d.PNG">

#### Undersampling

The results for using undersampling are as follows:

<img width="566" alt="Undersampling" src="https://user-images.githubusercontent.com/79733383/123736946-18445400-d870-11eb-9fa8-8b49b7966950.PNG">

#### Combination of over & under sampling

The results are as follows:

<img width="590" alt="Smoteenn" src="https://user-images.githubusercontent.com/79733383/123737167-7c671800-d870-11eb-9c77-357f50286fce.PNG">

### Ensemble learning methods
#### Balanced Random Forest classifier
The results of the first ensemble learning model used are as follows:

<img width="556" alt="BRFC" src="https://user-images.githubusercontent.com/79733383/123737584-38284780-d871-11eb-8cf3-e9b1716e67f3.PNG">

#### Easy Ensemble AdaBoost Classifier
The results of the easy ensemble adaboost classifier are as follows:

<img width="590" alt="last" src="https://user-images.githubusercontent.com/79733383/123737666-5d1cba80-d871-11eb-98ab-bf7c3f4ece2d.PNG">

## Summary

Looking at the different methods & models we tested, we can see that for the dataset we have, using ensemble learning techniques gave better results than using resampling techniques.
The most accurate model is the Easy Ensemble AdaBoost Classifier.

We also arranged the factors affecting the loan status by importance using the feature_importance function, which showed that the highest factors are the total received principal & interest, while some factors like the tax liens, policy code & payment plan had no effect on the status. 






