# Heart-Disease-Classification
# Introduction
# Objectives
# Methodology
**Data columns desc**

The program used various codes, syntax, tools, and modules to generate the predictive capability of the system. The system used a dataset as data to be analyzed; it consists of 303 rows and 13 columns. To further understand the analysis, the user must be familiarized with the data column description below: 

**age**= refers to the age of the respondents
**sex**= refers to the basis of the respondent's reproductive function: Male(1) and Female(0)

**cp**= refers to the type of chest pain that the respondents experienced: typical angina(0), atypical angina(1), non-anginal pain(2), and asymptomatic(3)

**trestbps**= refers to the resting blood pressure of the respondent measured in the hospital in mm Hg

**Chol**= refers to the respondent's cholesterol in mg/dl

**fbs**= refers to the fasting blood sugar of the respondents. When the data is more significant than 120, it will indicate 1, meaning that it is true, and 0 if otherwise

**restecg**= refers to the resting electrocardiographic results of the respondents

**thalach** = refers to the maximum heart rate achieved

**exang**= refers to the respondent's exercise-induced angina: Yes (1) and No(0)

**oldpeak**= refers to the ST depression induced by exercise relative to rest

**Slope** = refers to the slope of the peak exercise ST segment gathered from the respondents with values: upsloping(0), flat(1), and downsloping (2)

**ca**= refers to the number of major vessels(0-30) colored by fluoroscopy gathered from the respondents

**thal3**= normal 6= fixed defect 7 = reversible defect

**Target** = refers to the diagnosis of the respondents having a heart disease (1) or not(0)


****Preprocessing data****
Outliers were used in the program to deviate significantly from the rest of the objects. Hence, it is used to find errors in the dataset. The program measured the outlier by checking the outliers by using the 25 and 75 percent of every column. In addition, the program normalized the numeric data by storing the data columns in a syntax standardizing the numeric features of the data using the StandardScaler function and replacing the original values with the standardized version.

**Modeling**

 The program used modeling to test the system's accuracy in predicting; the users used cross-validation, gradient boosting, random forest, AdaBoost, and SVM. Cross-validation was used by taking the classifier and its parameters along with the feature matrix and target variable and returning the score as a percentage, rounded to two decimal places.
	In addition, Gradient Boosting was used for regressing and classifying problems by testing the predictive capability of the machine learning model using two parameters: learning and model. The program tested the system using different values of parameters. Random forest were used to perform regression and classification tasks using multiple decision trees and a technique called Bootstrap and Aggregation. In this program, the user used different types of estimators and criterion in a max depth of 1.
	Adaboost was used to complete the training dataset to train weak learners, and it is a sequential process that corrects the error of the previous model. The program used different values of estimators and learning rates as parameters. Lastly, SVM was used to supervise machine learning. The program tested the system using different values and types of C and kernel as parameters

 
**Stacking best cross validation from 4**

In terms of stacking best cross-validation, the program used k-fold cross-validation and trained the classified and collected data, this was used for predictions and model stacking. Thus, the program piled the data into syntax and ran the syntax through another boosting meta-model and ensemble methods used for predicting the death rate caused by heart diseases

# Results and Discussion
**Countplot of  Target**
