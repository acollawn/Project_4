# Project_4
Module 23/24 Project

## Report

### Overview of the analysis: Explain the purpose of this analysis.
* In this project we analyze the diabetes.csv which is featured in the Kaggle database. The purpose of this project is to use a machine learning model to analyze and correctly predict whether or not a patient has diabetes or not. In an attempt to find the most accurate model for our data, we used 2 different models, the logistic regression and random forest models. 

* The data points that are taken into consideration are: 
    1) pregnancies
    2) glucose
    3) blood pressure
    4) skin thickness
    5) insulin
    6) BMI
    7) diabetes pedigree function
    9) age
    10) outcome

### Results: Using bulleted lists and images to support your answers, address the following questions:

#### Data Preprocessing

What variable(s) are the target(s) for your model?
* The target of our models was "Outcome". This column stated whether the participant has diabetes or not.

What variable(s) are the features for your model?
* The features of our model were pregnancies, glucose, blood pressure, skin thickness, insulin, BMI, diabetes pedigree function, and age.

What variable(s) should be removed from the input data because they are neither targets nor features?
* We deemed all columns important features for our model.

#### Compiling, Training, and Evaluating the Model
* Logistic Regrssion Model
    * Accuracy Score (pre randomoversampler): 0.732944503358077
    * Accuracy Score (post randomoversampler): 0.7427055702917772
* Random Forest Model
    * Accuracy Score (pre randomoversampler): 0.78125
    * Accuracy Score (post randomoversampler): 1.0

What steps did you take in your attempts to increase model performance?
* After starting off with the logistic regression model, we decided to try out a different model that might be better for the dataset and our goal.
* Despite our first attempt using the random forest model generating an accuracy score of .78, we resampled the data using the RandomOverSampler (imblearn) and our model was then able to predict with an accuracy rate of 1.0. 


### Summary:
* The Random Forest Model was ideal to predict our diabetes dataset. We produced an initial model and made edits to it in order to optimize the accuracy score. 
* Our model achieved an accuracy score of 1.0, recall of 1.0, precision of 1.0, and f1-score of 1.0.
* The three most important features from our dataset, according to the feature_importances_, are 1. glucose 2. BMI, 3. Age. 
* While our model is able to predict with 100% accuracy this is due to the limitation that our sample size is small. Our data is comprised of 768 rows of data (females only) with 8 measurable variables and 1 outcome. We would benefit from inputting a larger dataset with both genders.



### Tableau Pages:
Please follow the link to our Tableau Public page for our Random Forest Model: 
<a href="https://public.tableau.com/app/profile/jared.sletto/viz/RF_Diabetes_Tablea/PredictingDiabetes">Predicting Diabetes</a>
