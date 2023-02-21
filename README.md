# Credit-Card-Fraud-Detection

### Problem Statement - 
Predict fraudulent credit card transactions with the help of Machine learning models.

### Dataset Description - 

The data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The data set has also been modified with principal component analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value of 1 in cases of fraud and 0 in others.

### Project Pipeline - 
The project pipeline can be briefly summarised in the following four steps:

#### Data Understanding: 
We need to load the dataset and understand the features present in it. 

#### Exploratory Data Analysis (EDA): 
We need to check whether there is any skewness in the data and try to mitigate it, as it might cause problems during the model building phase.

#### Train/Test split: 
It is required to split the dataset into train/test set to check the performance of the models with unseen data. We need to use stratified k-fold cross-validation method. 

#### Model building / hyperparameter tuning: 
We have to try building different models and fine-tune their hyperparameters until we get the desired level of performance on the raw (imbalanced) data set. Finally, we have to build up a better model after balancing the dataset (SMOTE & ADASYN). 

#### Model evaluation: 
Evaluate the models using an appropriate evaluation metric. Note that since the data is imbalanced, it is is more important to identify the fraudulent transactions accurately than the non-fraudulent ones. We need to choose an appropriate evaluation metric that reflects this business goal.
