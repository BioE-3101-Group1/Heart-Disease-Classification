<img width="227" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/1ce0509c-c3a1-4992-9070-b75069482c2a"># Heart-Disease-Classification
# Introduction
# Objectives
# Methodology
**Data columns desc**<br>
	The program used various codes, syntax, tools, and modules to generate the predictive capability of the system. The system used a dataset as data to be analyzed; it consists of 303 rows and 13 columns. To further understand the analysis, the user must be familiarized with the data column description below:<br>
* age= refers to the age of the respondents
* sex= refers to the basis of the respondent's reproductive function: Male(1) and Female(0)
* cp= refers to the type of chest pain that the respondents experienced: typical angina(0), atypical angina(1), non-anginal pain(2), and asymptomatic(3)
* trestbps= refers to the resting blood pressure of the respondent measured in the hospital in mm Hg
* Chol= refers to the respondent's cholesterol in mg/dl
* fbs= refers to the fasting blood sugar of the respondents. When the data is more significant than 120, it will indicate 1, meaning that it is true, and 0 if otherwise
* restecg= refers to the resting electrocardiographic results of the respondents
* thalach= refers to the maximum heart rate achieved
* exang= refers to the respondent's exercise-induced angina: Yes (1) and No(0)
* oldpeak= refers to the ST depression induced by exercise relative to rest
* Slope= refers to the slope of the peak exercise ST segment gathered from the respondents with values: upsloping(0), flat(1), and downsloping (2)
* ca= refers to the number of major vessels(0-30) colored by fluoroscopy gathered from the respondents
* thal3= normal 6= fixed defect 7 = reversible defect
* Target= refers to the diagnosis of the respondents having a heart disease (1) or not(0)

**Preprocessing data** <br>
	Outliers were used in the program to deviate significantly from the rest of the objects. Hence, it is used to find errors in the dataset. The program measured the outlier by checking the outliers by using the 25 and 75 percent of every column. In addition, the program normalized the numeric data by storing the data columns in a syntax standardizing the numeric features of the data using the StandardScaler function and replacing the original values with the standardized version.<br>

**Modeling**<br>
	The program used modeling to test the system's accuracy in predicting; the users used cross-validation, gradient boosting, random forest, AdaBoost, and SVM. Cross-validation was used by taking the classifier and its parameters along with the feature matrix and target variable and returning the score as a percentage, rounded to two decimal places.<br>
	In addition, Gradient Boosting was used for regressing and classifying problems by testing the predictive capability of the machine learning model using two parameters: learning and model. The program tested the system using different values of parameters. Random forest were used to perform regression and classification tasks using multiple decision trees and a technique called Bootstrap and Aggregation. In this program, the user used different types of estimators and criterion in a max depth of 1.<br>
	Adaboost was used to complete the training dataset to train weak learners, and it is a sequential process that corrects the error of the previous model. The program used different values of estimators and learning rates as parameters. Lastly, SVM was used to supervise machine learning. The program tested the system using different values and types of C and kernel as parameters.<br>

 
**Stacking best cross validation from 4** <br>
	In terms of stacking best cross-validation, the program used k-fold cross-validation and trained the classified and collected data, this was used for predictions and model stacking. Thus, the program piled the data into syntax and ran the syntax through another boosting meta-model and ensemble methods used for predicting the death rate caused by heart diseases.<br>

# Results and Discussion
**Countplot of  Target**<br>
<img width="220" alt="1aa" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/a323d404-46f1-45fb-92e2-25c642d8b61b"><br>
Illustrates the number number of respondents having a heart disease (1) or not(0) using bar graph<br>

**Heatmat**<br>
<img width="176" alt="1bb" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/c54321ac-9c85-4af8-a2fc-1f028ba88f50"><br>
The heatmap was used to analyze the correlation of the attained data, the data used colors to represents. For instance the data indicates the intensity of data showing the its correlation, as the correlation gets closer to the value of 1, the two data types are positively correlated, and negatively correlated for negative values. The correlation is illustrated by the color temperature of every cell. We can see there is a positive correlation between chest pain (cp) & target (our predictor). This makes sense since, The greater amount of chest pain results in a greater chance of having heart disease.<br>

**Barplot of Slope Based Target**<br>
<img width="222" alt="1cc" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/310896fb-0c57-48cb-89f3-c27d041a088f"><br>
The graph plotted different types of slopes that indicates the peak of exercise ST segment gathered with reference to the target that indicates the diagnosis of the on the patients. Slope 0 with 9, slope 1 with 49, and slope 2 with 107. The "slope" hue, refers to the peak exercise ST segment, with values: 0: upsloping , 1: flat , 2: downsloping.<br>
This supports the plot above because low ST Depression yields people at greater risk for heart disease[x value=downsloping - closer to target with value of 1(with disease).] While a high ST depression (upsloping) is considered normal & healthy.<br>

**Distplot of thalach**<br>
<img width="227" alt="1dd" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/61b67131-6b9a-49f8-92bb-6f1852191b45"><br>
The displot indicates the density of the maximum heart rate (thalac). It is noticeable that the plot made a bell like shape as the maximum density falls between 150-175. The displot was also customize to red color.<br>

**Barplot of cp based on target**<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/b0291195-385d-420d-996e-f5f94c99ffc9)<br>
The table plotted different types of chest pain that the respondents experienced that indicates the diagnosis of the on the patients. Cp 3 with 39, Cp 2 with 41, Cp 1 with 69, and Cp 0 with 16.<br>
Cp (chest pain), is a ordinal feature with 4 values. This makes sense since, The greater amount of chest pain results in a greater chance of having heart disease.<br>

