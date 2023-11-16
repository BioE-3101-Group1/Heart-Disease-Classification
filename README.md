# Heart-Disease-Classification
## Introduction
<p align="justify">Using the capabilities of categorization machine learning algorithms, heart disease prediction has grown in importance in today's healthcare environment. Because cardiovascular diseases are very common, it is critical to create precise and effective predictive models as soon as possible to help doctors diagnose and treat patients early. With so much patient data at their disposal—from demographics to detailed medical histories—classification algorithms have the potential to identify intricate patterns and risk factors that may be difficult to identify with conventional diagnostic techniques. This is a revolutionary strategy where healthcare and machine learning come together to provide doctors with tools that improve the accuracy and timeliness of heart disease prediction.</p>

<p align="justify">The main goal of this study was to predict whether individuals had underlying cardiac problems by using a hospital system dataset for analysis and information extraction. By carefully analyzing the data, the goal was to create a prediction model that would improve the ability to recognize people who are more likely to have these kinds of illnesses. The objective is to use the knowledge gathered from the dataset analysis to support preventative healthcare initiatives.</p>

## Objectives
- Conduct a comprehensive statistical analysis of the heart disease dataset to gain insights into the distribution and characteristics of the variables.<br>
- Implement data refinement techniques to identify and handle missing or erroneous codes, ensuring the quality of the program.<br>
- Visualize the data using appropriate graphs and charts to facilitate a better understanding of the relationships between different features.<br>
- Interpret the results obtained from the models, providing insights into the factors influencing heart disease classification.<br>
- To predict the mortality from heart disease based on the given dataset.<br>
- Explore the practical applications of the developed program in real-world healthcare settings.<br>

## Methodology
### Data Columns Desc <br>
<p align="justify">The program used various codes, syntax, tools, and modules to generate the predictive capability of the system. The system used a dataset as data to be analyzed; it consists of 303 rows and 13 columns. To further understand the analysis, the user must be familiarized with the data column description below:<br>
 
- age= refers to the age of the respondents<br>
- sex= refers to the basis of the respondent's reproductive function: Male(1) and Female(0)<br>
- cp= refers to the type of chest pain that the respondents experienced: typical angina(0), atypical angina(1), non-anginal pain(2), and asymptomatic(3)<br>
- trestbps= refers to the resting blood pressure of the respondent measured in the hospital in mm Hg<br>
- Chol= refers to the respondent's cholesterol in mg/dl<br>
- fbs= refers to the fasting blood sugar of the respondents. When the data is more significant than 120, it will indicate 1, meaning that it is true, and 0 if otherwise<br>
- restecg= refers to the resting electrocardiographic results of the respondents<br>
- thalach= refers to the maximum heart rate achieved<br>
- exang= refers to the respondent's exercise-induced angina: Yes (1) and No(0)<br>
- oldpeak= refers to the ST depression induced by exercise relative to rest<br>
- Slope= refers to the slope of the peak exercise ST segment gathered from the respondents with values: upsloping(0), flat(1), and downsloping (2)<br>
- ca= refers to the number of major vessels(0-30) colored by fluoroscopy gathered from the respondents<br>
- thal3= normal 6= fixed defect 7 = reversible defect<br>
- Target= refers to the diagnosis of the respondents having a heart disease (1) or not(0)<br>

### Preprocessing Data <br>
<p align="justify">Outliers were used in the program to deviate significantly from the rest of the objects. Hence, it is used to find errors in the dataset. The program measured the outlier by checking the outliers by using the 25 and 75 percent of every column. In addition, the program normalized the numeric data by storing the data columns in a syntax standardizing the numeric features of the data using the StandardScaler function and replacing the original values with the standardized version.</p>

### Modeling<br>
<p align="justify">The program used modeling to test the system's accuracy in predicting; the users used cross-validation, gradient boosting, random forest, AdaBoost, and SVM. Cross-validation was used by taking the classifier and its parameters along with the feature matrix and target variable and returning the score as a percentage, rounded to two decimal places.</p>

<p align="justify">In addition, Gradient Boosting was used for regressing and classifying problems by testing the predictive capability of the machine learning model using two parameters: learning and model. The program tested the system using different values of parameters. Random forest were used to perform regression and classification tasks using multiple decision trees and a technique called Bootstrap and Aggregation. In this program, the user used different types of estimators and criterion in a max depth of 1.</p>

<p align="justify">Adaboost was used to complete the training dataset to train weak learners, and it is a sequential process that corrects the error of the previous model. The program used different values of estimators and learning rates as parameters. Lastly, SVM was used to supervise machine learning. The program tested the system using different values and types of C and kernel as parameters.</p>
 
### Stacking Best Cross Validation from 4 <br>
<p align="justify">In terms of stacking best cross-validation, the program used k-fold cross-validation and trained the classified and collected data, this was used for predictions and model stacking. Thus, the program piled the data into syntax and ran the syntax through another boosting meta-model and ensemble methods used for predicting the death rate caused by heart diseases.</p>

## Results and Discussion
<p align="center">
  <img width="342" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/510daa1f-e9e4-4186-87c6-7a678f8288d8"> </p>
<p align="center">Figure 1: Countplot of the Target </p>
<p align="justify">Heart disease is an alarming disease that occurs in different ages and genders; diagnosing this disease involves various tests and diagnosis of the heart, including blood tests, chest x-ray, ECG, heart monitoring, endocardium, exercise tests, cardiac catheterization, heart CT scan, and heart MRI scan (Heart Disease, 2022). This activity shows the total count of the data. Target 1 represents the patient diagnosed with heart disease; while 0 represents the patient not diagnosed with heart disease. The total number of patients with heart disease is 165, and the count of those not having heart disease is 138. A total of 303 entries were recorded.</p>


<p align="center">
<img width="208" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/17ce8503-85c2-4ca8-b3a0-6f8fbdb237e8"></p>
<p align="center"> Figure 2: Heatmap of the Dataset</p>
<p align="justify">Python is a powerful tool that allows users to generate images and tables to illustrate data further; heatmap is a tool that shows the values with the corresponding color depending on the different values that allows the user to analyze the patterns and correlations of the data (Ramuglia, 2023). Hence, heatmap was used to analyze the correlation of the obtained data, the data used colors to represent a certain value. For instance, the data indicates the intensity of data showing its correlation, as the correlation gets closer to the value of 1, the two data types are positively correlated, and negatively correlated for negative values. Thus, the correlation is illustrated by the color temperature of every cell. We can see there is a positive correlation between chest pain (cp) & target (our predictor). This makes sense since, the greater amount of chest pain results in a greater chance of having heart disease.</p>


<p align="center">
<img width="313" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/6042370e-abb5-459e-9cd0-acecf74c965f"></p>
<p align="center"> Figure 3: Barplot of Slope with Respect to Target</p>
<p align="justify">The ST segment is the region between the end and beginning of repolarization of the heart in ECG. Thus, the ST segment can be displaced above(upsloping) or below (downsloping) the baseline in a different manner, while having a flat ST segment indicates an average slope (Kashou, 2023). The table plotted different types of slopes that indicate the peak of exercise ST segment gathered with reference to the target that indicates the diagnosis of the patients. Slope 0 with 9, slope 1 with 49, and slope 2 with 107. The "slope" hue, refers to the peak exercise ST segment, with values: 0: upsloping , 1: flat , 2: downsloping).</p>


<p align="center">
<img width="338" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/0d450ba8-b2cb-418f-b32f-20b920351346"></p>
<p align="center"> Figure 4: Distribution Plot of Thalac</p>
<p align="justify">The displot indicates the density of the maximum heart rate (thalac). It is noticeable that the plot made a bell like shape as the maximum density falls between 150-175. The displot was also customized to red color. Maximum heart rate indicates the highest heart rate that can beat per minute to help an individual monitor the activities that they are doing (How to Calculate Max Heart Rate and Train with it, 2022)</p>


**Barplot of Cp Based on Target**<br>
<p align="center">
<img width="341" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/47d2aa2f-9ddc-48c6-8da0-bc9553bc28d9"></p>
<p align="center"> Figure 5: Barplot of CP with Respect to Target</p>
<p align="justify">The table plotted different types of chest pain that the respondents experienced that indicates the diagnosis of the patients. Cp 3 with 39, Cp 2 with 41, Cp 1 with 69, and Cp 0 with 16. Chest pain is a feeling the users experience and encompasses a broad differential diagnosis. In this program, the data set includes various classifications, including typical angina, also known as stable angina, characterized as discomfort provoked by extension at rest (Gillen,2022). Furthermore, atypical angina is chest pain that occurs when the heart lacks the supply of oxygenated blood (Atypical Chest Pain, n.d.). Tee Melecgrito (2023)n said that anginal chest pain ranges from gastrointestinal problems. Lastly, asymptomatic chest pain is defined as rupture causes a blood clot to form in the artery, leading to acute blockage (Gayle, 2020). Cp (chest pain), is an ordinal feature with 4 values. This makes sense since, The greater amount of chest pain results in a greater chance of having heart disease. </p>


<p align="center">
<img width="338" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/df08e54d-8bd1-47c5-beea-4eec69488220"></p>
<p align="center"> Figure 6: Distribution Plot of Age</p>
<p align="justify">The table plotted different types of chest pain that the respondents experienced that indicates the diagnosis of the patients. Cp 3 with 39, Cp 2 with 41, Cp 1 with 69, and Cp 0 with 16.  Cp (chest pain), is an ordinal feature with 4 values. This makes sense since, The greater amount of chest pain results in a greater chance of having heart disease. The results reflected the study of Hearth Health and Aging (n.d.) that determines a person whose age is 60 and older is more prone to heart disease compared to young individuals as aging can cause changes in heart and blood vessels, increasing the risk of health.</p>


**OutLiers**
**Age**<br>
<p align="center">
<img width="356" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/5ca4b0cb-c30f-4c88-89e5-2f2f4b800cdd"></p>
<p align="center"> Figure 7: Histogram of Age with Respect to Target</p>
<p align="justify">The histogram classified the ages based on the target having target 0 as people without disease and target 1 as people with the disease. As we can see between 35 - 70,in age 50-60 has the highest number of people without disease then it goes lower as the people get older. On the other hand, people with disease have a scattered histogram; it is unstable as the blocks in histogram increase and decrease simultaneously as the age progresses.</p>


<p align="center">
<img width="345" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/fdb7b768-7ffd-4016-b428-edfa8eac445e"></p>
<p align="center"> Figure 8: Histogram of Age Based on Target and Sex</p>

* Target 0 sex 0 
<p align="justify">The histogram shows that the female whose age is within the range of 55-65 has a smaller number of people that doesn't have disease unlike when they are young.</p>

* Target 0 sex 1
<p align="justify">The histogram indicates that the male whose age is between 35 - 70 has a higher number of people that doesn't have a disease compared to female.</p>

* Target 1 sex 0
<p align="justify">The histogram illustrates that the female has a more scattered data compared to male as it's age range from 35-70 but it has a lower number of people that has a disease.</p>

* Target 1 sex 1
<p align="justify">The histogram represents that the male has a more compressed data compared to female as it's age range 35-70 but it has a higher number of people that has a disease.</p>



**Ageband**<br>
<p align="center">
<img width="349" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/2f0ae658-f7c0-4b2f-a41a-f0eaccd04fd0"></p>
<p align="center"> Figure 10: Ageband with Reference to Target and Sex</p>

* Target 0 Sex 0
<p align="justify">The histogram shows that in the female age group of 2,3,and 4 has a lower number of people that doesn't have disease compared to male.</p>

* Target 0 Sex 1
<p align="justify">The histogram indicates that the data of the male age group of 1,2,3,4, and 5 it has a larger number of people that doesn't have a disease compared to female.</p>

* Target 1 Sex 0
<p align="justify">The histogram shows female data are included in all age group indicating that female has a lower number of people who has a disease compared to male.</p>

* Target 1 Sex 1
<p align="justify">The histogram indicates that male data are included in all age group  showing that male has a larger number of people who has a disease compared to female.</p>
<p align="justify">This corresponds to the previous graph showing the specific age of the respondents.</p>

**Sex**
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/58d5c684-d8b3-4494-8802-69a08eeed78f)<br>

* Target 0 Sex 0<br>
The histogram shows that in the female age group of 2,3,and 4 has a lower number of people that doesn't have disease compare to male<br>
* Target 0 Sex 1<br>
The histogram indicates that the data of the male age group of 1,2,3,4, and 5 it has a larger number of people that doesn't have a disease compare to female<br>
* Target 1 Sex 0<br>
The histogram shows female data are included in all age group indicating that female has a lower number of peope who has a disease compare to male<br>
* Target 1 Sex 1<br>
The histogram indicates that male data are included in all age group showing that male has a larger number of people who has a disease compare to female<br>
This corresponds to the previous graph showing the specific age of the respondents.<br>


**Barplot of Sex**<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/217ef030-faa2-4ec8-aef3-cd95bdef7f90)<br>
The barplot indicates that the number of male has 207 respondents making it larger than 96 data of the female. This explains why the male barplot in the previous age graphs are generally higher than the female.<br>


**Distplot of Trestbps**<br>
* Oldpeak = ST depression induced by exercise relative to rest<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/c8ec52b2-db77-48a9-92a0-a582442f8e89)<br>
The distplot indicates the resting blood pressure of the respondent measured with respect to density. It shows a bell like shape showing a highest 120-140.<br>


**Distplot of Chol**<br>
* Chol = serum cholestoral in mg/dl<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/288a35e8-831e-43ed-9fb8-39c579bfed16)<br>
The distplot shows the cholesterol level in mg/dl with density as it's y-axis parameter. The data shows a highest point at the 200-300. The observed data shows a more compressed distplot than the other<br>


**Countplot of Fbs**<br>
* Fbs = ( fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/30f6d2b0-01ef-4752-85d8-217f2ebf47b3)<br>
The countplot shows the counted graph of the fasting blood sugar where the data is classified as more 120(1) and otherwise (0).<br>


**Countplot of Restecg**<br>
* Restecg = resting electrocardiographic results<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/06303242-3ee3-4f3c-a14e-26e22e946614)<br>
The table counted the resting electrocardiographic results showing a lowest count in 2. The x values indicate ecg results as: — Value 0: showing probable or definite left ventricular hypertrophy by Estes’ criteria — Value 1: normal — Value 2: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)<br>


**Distplot of Thalach**<br>
* Thalach = maximum heart rate achieved<br>
  ![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/6e29826e-4c88-409f-a8b5-cec4b7fd123d)<br>
The distplot indicates the maximum heart rate achieved with respect to the density as its y-axis parameter. <br>
* The left plot shows that the data is spread from 75-200, it shows a high data output in the 150<br>
* The right plot shows that the data is spread 100-200 making it to have a more compact bellshaped, it has the highest data outpu0t in the 150<br>


**Countplot of Exang**<br>
* Exang = exercise induced angina (1 = yes; 0 = no)<br>
* ![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/62a6bfc5-7d80-428a-92e5-1918ae8599dc)<br>
The image shows the counted respondents classifying if they experience exercise-induced angina (1) or not(0). The data shows 0 has the highest number of counts in the table<br>


**Distplot of Oldpeak**<br>
* Oldpeak = ST depression induced by exercise relative to rest<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/141978d6-d035-4971-a60b-c2eeccfd5af3)<br>
The image shows the counted respondents classifying if they experience exercise-induced angina (1) or not(0). The data shows 0 has the highest number of counts in the table.<br>


**Distplot based on Target**<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/16ba022a-c311-446e-bad5-4aaced321104)<br>
The data classified the oldpeak using a distplot with respect to the diagnosis.<br>
* The left image indicates a highest data output in the 0 and decreasing line as the oldpeak increases<br>
* The right image shows the highest data output in the 0 and stop decreasing in the 1.75 befor continuing its decrease. The image has a narrower line compare to the other one as it involves a lesser number values of oldpeak<br>


**Barplot od ca**<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/dbd22342-7f81-4cf7-80b1-d95bb63b9665)<br>
The barplot indicates the number of major vessels colored by fluoroscopy, it shows a highest value of ca and highest value of error bar at 4<br>


**Barplot of Thal**<br>
<img width="347" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/1eff0172-d098-4052-be93-b45c8c3c07a8"><br>
The barplot shows a highest number of data in 2 but a highest error bar in 0<br>

**Modeling**<br>
![image](https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/b8e56e31-ade3-455d-8119-79b734262463)<br>
The table shows the highest value attained in each modeling and to analyze the highest model method. The data shows that random forest has the highest score values attained used to perform both regression and classification tasks with the use of multiple decision trees and a technique called Bootstrap and aggregation<br>


**Stacking best cross validation from 4**<br>
* Final score for predicting death by heart disease is 88.16<br>

## Conclusion

## Disclaimer 
The instructions and code used in the project are based on the provided guidelines. The program and dataset used for this gathered from the work of Lital Davar, retrieved from https://www.kaggle.com/code/litaldavar/heart-disease-classification/notebook?fbclid=IwAR1sxjxbEjUTc6cLk70JR8ZPLWbKme7REkpr7vZOVadnS3FlyESwwkToxug<br>
