# Heart Disease Classification
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
<br>

<p align="center">
<img width="208" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/17ce8503-85c2-4ca8-b3a0-6f8fbdb237e8"></p>
<p align="center"> Figure 2: Heatmap of the Dataset</p>
<p align="justify">Python is a powerful tool that allows users to generate images and tables to illustrate data further; heatmap is a tool that shows the values with the corresponding color depending on the different values that allows the user to analyze the patterns and correlations of the data (Ramuglia, 2023). Hence, heatmap was used to analyze the correlation of the obtained data, the data used colors to represent a certain value. For instance, the data indicates the intensity of data showing its correlation, as the correlation gets closer to the value of 1, the two data types are positively correlated, and negatively correlated for negative values. Thus, the correlation is illustrated by the color temperature of every cell. We can see there is a positive correlation between chest pain (cp) & target (our predictor). This makes sense since, the greater amount of chest pain results in a greater chance of having heart disease.</p>
<br>

<p align="center">
<img width="313" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/6042370e-abb5-459e-9cd0-acecf74c965f"></p>
<p align="center"> Figure 3: Barplot of Slope with Respect to Target</p>
<p align="justify">The ST segment is the region between the end and beginning of repolarization of the heart in ECG. Thus, the ST segment can be displaced above(upsloping) or below (downsloping) the baseline in a different manner, while having a flat ST segment indicates an average slope (Kashou, 2023). The table plotted different types of slopes that indicate the peak of exercise ST segment gathered with reference to the target that indicates the diagnosis of the patients. Slope 0 with 9, slope 1 with 49, and slope 2 with 107. The "slope" hue, refers to the peak exercise ST segment, with values: 0: upsloping , 1: flat , 2: downsloping).</p>
<br>

<p align="center">
<img width="338" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/0d450ba8-b2cb-418f-b32f-20b920351346"></p>
<p align="center"> Figure 4: Distribution Plot of Thalac</p>
<p align="justify">The displot indicates the density of the maximum heart rate (thalac). It is noticeable that the plot made a bell like shape as the maximum density falls between 150-175. The displot was also customized to red color. Maximum heart rate indicates the highest heart rate that can beat per minute to help an individual monitor the activities that they are doing (How to Calculate Max Heart Rate and Train with it, 2022)</p>
<br>

**Barplot of Cp Based on Target**<br>
<p align="center">
<img width="341" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/47d2aa2f-9ddc-48c6-8da0-bc9553bc28d9"></p>
<p align="center"> Figure 5: Barplot of CP with Respect to Target</p>
<p align="justify">The table plotted different types of chest pain that the respondents experienced that indicates the diagnosis of the patients. Cp 3 with 39, Cp 2 with 41, Cp 1 with 69, and Cp 0 with 16. Chest pain is a feeling the users experience and encompasses a broad differential diagnosis. In this program, the data set includes various classifications, including typical angina, also known as stable angina, characterized as discomfort provoked by extension at rest (Gillen,2022). Furthermore, atypical angina is chest pain that occurs when the heart lacks the supply of oxygenated blood (Atypical Chest Pain, n.d.). Tee Melecgrito (2023)n said that anginal chest pain ranges from gastrointestinal problems. Lastly, asymptomatic chest pain is defined as rupture causes a blood clot to form in the artery, leading to acute blockage (Gayle, 2020). Cp (chest pain), is an ordinal feature with 4 values. This makes sense since, The greater amount of chest pain results in a greater chance of having heart disease. </p>
<br>

<p align="center">
<img width="338" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/df08e54d-8bd1-47c5-beea-4eec69488220"></p>
<p align="center"> Figure 6: Distribution Plot of Age</p>
<p align="justify">The table plotted different types of chest pain that the respondents experienced that indicates the diagnosis of the patients. Cp 3 with 39, Cp 2 with 41, Cp 1 with 69, and Cp 0 with 16.  Cp (chest pain), is an ordinal feature with 4 values. This makes sense since, The greater amount of chest pain results in a greater chance of having heart disease. The results reflected the study of Hearth Health and Aging (n.d.) that determines a person whose age is 60 and older is more prone to heart disease compared to young individuals as aging can cause changes in heart and blood vessels, increasing the risk of health.</p>
<br>

**OutLiers**
**Age**<br>
<p align="center">
<img width="356" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/5ca4b0cb-c30f-4c88-89e5-2f2f4b800cdd"></p>
<p align="center"> Figure 7: Histogram of Age with Respect to Target</p>
<p align="justify">The histogram classified the ages based on the target having target 0 as people without disease and target 1 as people with the disease. As we can see between 35 - 70,in age 50-60 has the highest number of people without disease then it goes lower as the people get older. On the other hand, people with disease have a scattered histogram; it is unstable as the blocks in histogram increase and decrease simultaneously as the age progresses.</p>
<br>

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
<br>

**Ageband**<br>
<p align="center">
<img width="150" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/ef5bda21-36cb-4cf8-af66-4791ffc8e814"></p>
<p align="center"> Figure 9: Ageband</p>
<p align="justify">The table shows and created an ageband that are further used on the later program as a condition to process and classify the signal</p>
<br>
 
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
<br>

**Sex**
<p align="center">
<img width="326" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/14f19472-13b6-4f53-b7e1-f3f6ac6eb5bf"></p>
<p align="center"> Figure 11: Countplot of Sex</p>
<p align="justify">The barplot indicates that the number of male has 207 respondents making it larger than 96 data of the females. This explains why the male barplot in the previous age graphs are generally higher than the female.</p>
<br>

**Trestbps**<br>
<p align="center">
<img width="324" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/1fc07dc3-4cb4-4d69-abbf-dff15ee2b0dc"></p>
<p align="center"> Figure 12: Distribution Plot of Trestbps</p>
<p align="justify">Blood pressure is the force excreted by the heart when it pumps to the artery walls. Thus, it is composed of systolic (highest pressure when the heart pumps) and diastolic ( pressure when the heart relaxes) (Blood pressure (high)-hypertension, n.d.). In this activity, the distplot indicates the resting blood pressure of the respondent measured with respect to density. It shows a bell-like shape showing a highest 120-140. </p>
<br>

**Chol**<br>
<p align="center">
<img width="332" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/b37c7e33-819b-4603-85b6-874405d6217c"></p>
<p align="center"> Figure 13: Distribution Plot of Chol </p>
<p align="justify">Cholesterol is one of the parameters that define the state or health of the heart. Cholesterol is a waxy substance for building healthy cells (High Cholesterol-Symptoms and Causes-Mayo Clinic, 2023). Thus, the high-density lipoprotein (HDL), low-density lipoprotein (LDL), and triglycerides can be seen in a person's serum cholesterol, and it was used to indicate the risk of having a heart disease (Huizen, 2021). In this activity, distplot shows the cholesterol level in mg/dl with density as it's y-axis parameter. The data shows a highest point at 200-300. The observed data shows a more compressed distplot than the other.</p>
<br>

**Fbs**<br>
<p align="center">
<img width="328" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/f7795705-9122-4eef-ad2b-cdc49133f95a"></p>
<p align="center"> Figure 14: Countplot of FBS</p>
<p align="justify">The number of glucose or sugar in the blood is defined as the fasting blood sugar; results in 100-125 mg/dl indicate prediabetes, and above 126 mm/dl means diabetes (Professional, n.d.). The countplot shows the counted graph of the fasting blood sugar where the data is classified as more 120(1) and otherwise (0).</p>
<br>

**Restecg**<br>
<p align="center">
<img width="317" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/1ca83609-5005-4f11-bb53-18c40a3d92ad"></p>
<p align="center"> Figure 15: Countplot of Restecg</p>
<p align="justify">A resting electrocardiogram is the electrical activity of the heart while at rest and defines the enlargement of the heart (Resting Electrocardiography, 2016). In this program, the table counted the resting electrocardiographic results showing a lowest count in 2. The x values indicate ecg results as:</p>

* Value 0: showing probable or definite left ventricular hypertrophy by Estes’ criteria<br>
* Value 1: normal<br>
* Value 2: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)<br>
<br>

**Thalach**<br>
<p align="center">
<img width="332" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/60e95b80-e214-4a67-b45b-ef06b368e7ea"></p>
<p align="center"> Figure 16:  Distribution Plot of Thalach with Respect to Target</p>
<p align="justify">The maximum heart rate is measured by subtracting your age from 220 and multiplying it by 0.64 and 0.76, indicating 64% and 74% of the average maximum heart rate (Target Heart Rate and Estimated Maximum Heart Rate| Physical Activity | CD, n.d.). The distplot indicates the maximum heart rate achieved with respect to the density as its y-axis parameter.</p>

* The left plot shows that the data is spread from 75-200, it shows a high data output in the 150<br>
* The right plot shows that the data is spread 100-200 making it to have a more compact bellshaped, it has the highest data outpu0t in the 150<br>
<br>

**Exang**<br>
<p align="center">
<img width="322" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/e738353c-e426-416d-ad7a-94d30de0257d"></p>
<p align="center"> Figure 17: Countplot of Exang</p>
<p align="justify">Exercise-induced angina is a pain that was measured in the dataset in this activity; in an article entitled Angina: Symptoms, Diagnosis, and Treatments (2021), angina was defined as the pain in the chest that can be felt during exercise, stress, and activities that makes the heart work harder. In this activity, the image shows the counted respondents classifying if they experience exercise-induced angina (1) or not(0). The data shows 0 has the highest number of counts in the table.</p>
<br>

**Oldpeak**<br>
<p align="center">
<img width="315" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/c668b106-b783-415f-bc8e-0b272baf3964"></p>
<p align="center"> Figure 18: Distribution Plot of Oldpeak</p>
<p align="justify">Old peak is defined as the ST depression (occurs when the J point is displaced below baseline) induced by exercise relative to rest (Deshmukh, 2022). This program showed that the image shows the counted respondents classifying if they experience exercise-induced angina (1) or not(0). The data shows 0 has the highest number of counts in the table.</p>
<br>

<p align="center">
<img width="338" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/5cc058e1-69d1-4cd9-bb47-a4dcef1eed13"></p>
<p align="center"> Figure 19: Distribution Plot of Oldpeak Based on Target</p>
<p align="justify">The data classified the oldpeak using a distplot with respect to the diagnosis.</p>

* The left image indicates a highest data output in the 0 and decreasing line as the oldpeak increases.<br>
* The right image shows the highest data output in the 0 and stop decreasing in the 1.75 before continuing its decrease. The image has a narrower line compare to the other one as it involves a lesser number values of oldpeak.<br>
<br>

**CA**<br>
<p align="center">
<img width="342" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/a8c3c36f-c56b-4110-86b6-47bf251e9a1f"></p>
<p align="center"> Figure 20: Barplot of CA with Respect to Target</p>
<p align="justify">The barplot indicates the number of major vessels colored by fluoroscopy, it shows a highest value of ca and highest value of error bar at 4</p>
<br>

**Thal**<br>
<p align="center">
<img width="314" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/9b1a360a-3a47-4ffe-b2c8-321d6e6305c7"></p>
<p align="center"> Figure 21: Barplot of Thal with Respect to Target</p>
<p align="justify">Thalassemia is a disease that was analyzed in the dataset, it is defined as an inherited blood disorder when the body doesn't make enough hemoglobin (Learn more about  thalassemia | CDC, 2023). In this activity, the barplot shows a highest number of data in 2 but a highest error bar in 0</p>
<br>

**Modeling**<br>
<p align="center">
<img width="150" alt="image" src="https://github.com/BioE-3101-Group1/Heart-Disease-Classification/assets/150891754/c46cd1e3-7236-4c23-9325-486e6b570b3c"></p>
<p align="center"> Figure 22: Maximum Score of the Used Model</p>
<p align="justify">The table shows the highest value attained in each modeling and to analyze the highest model method. The data shows that random forest has the highest score values attained used to perform both regression and classification tasks with the use of multiple decision trees and a technique called Bootstrap and aggregation.</p>
<br>

**Stacking Best Cross Validation from 4**<br>
<p align="justify">Achieving reliable and accurate forecasts is crucial for proactive healthcare interventions and well-informed decision-making in the field of heart disease mortality predictive modeling. Stacking, an advanced ensemble methodology, has been used to overcome this difficulty by combining the advantages of four different cross-validation techniques. By combining various viewpoints and prediction skills from several cross-validation methods, the stacked model aims to strengthen the predictive model's overall generality and dependability. After extensive training and assessment, the combination of these approaches produced an outstanding 88.16% final accuracy score. This success not only demonstrates how well stacking unifies disparate model outputs, but also emphasizes how it might improve the accuracy of forecasts for important health outcomes, such as heart disease mortality.</p>

## Application
<p align="justify">The integration of the developed program holds significant practical applications in real-world medical settings and is crucial for the progression of the healthcare industry. In a study conducted by Javaid et al. (2022), physicians, scientists, or researchers may use machine learning as a potent tool; this technology helps organizations and pharmaceutical companies create treatments for serious illnesses more quickly and efficiently. This predictive tool can assist healthcare professionals in risk classification and personalized treatment planning for patients with suspected cardiovascular issues.  By analyzing diverse factors that were set as the parameters, the program can provide insights into the likelihood of different heart diseases, enabling clinicians to make more informed decisions about diagnostic tests, interventions, and long-term management strategies. </p>

<p align="justify">The program's integration into routine clinical practice has the potential to enhance accuracy in disease classification, optimize resource allocation, and ultimately improve patient outcomes by tailoring interventions to individualized risk profiles. Priya et al. (2021) denoted that for someone undergoing diagnosis, early abnormality prediction will be vital. Hence the contribution to preventive care efforts by identifying high-risk individuals who may benefit from targeted lifestyle modifications and early interventions to mitigate the progression of cardiovascular conditions is of interest. </p>

<p align="justify">(TR et al., 2022) highlighted that even with a smaller data set, machine learning models remain the most effective option for classifying and predicting cardiac disease. These technological advancements empower healthcare professionals with data-driven insights, fostering a more personalized and proactive approach to patient care. Moreover, such technologies facilitate a shift towards preventive healthcare, as they identify individuals at higher risk, allowing for timely implementation of preventive measures. Ultimately, these advancements streamline decision-making processes, improve overall healthcare quality, and position the industry to meet the challenges of an evolving medical landscape, where precision, efficiency, and patient-centric care are of utmost importance. </p>

## Conclusion
<p align="justify">In conclusion, the objectives set out for this broad analysis of the heart disease dataset have been accomplished, generating important insights and practical applications. The statistical analysis provided an in-depth analysis of the dataset, cast on the distribution pattern as well as aspects of numerous variables, setting up the foundation for a more comprehensive understanding of heart disease. The use of data modification techniques was important in ensuring the correctness and precision of the program. The dataset's integrity was maintained by identifying and correcting missing or inaccurate codes, which improved the accuracy of subsequent analyses and predictions.The ability to predict can help healthcare workers identify high-risk individuals and conduct early interventions to enhance the treatment of patients. The analysis of practical applications in real-world healthcare settings underlines the program's potential impact, from risk assessment to guiding treatment methods, this program has the potential to improve clinical decision-making processes, ultimately contributing to more effective and specific treatment for patients.</p>
<p align="justify">The distribution and interrelationships among numerous variables were shown using meticulous data refining and strong visualization tools. The graphs and figures provided insights into the world of heart health, presenting a vivid picture of relationships between characteristics such as pain in the chest, age, and diagnostic outcomes. The dataset showed important characteristics such as the frequency of heart disease across different ages and genders, the impact of chest pain on diagnosis, and the complex patterns in variables such as heart rate at rest, cholesterol levels, and blood pressure. These findings supported existing medical knowledge, emphasizing the importance of these parameters in predicting heart condition. Identifying abnormalities, especially in age distribution, showed significant trends, highlighting differences in disease frequency across age groups and genders. This comprehensive analysis examines blood pressure, cholesterol, and fasting blood sugar levels, providing light on their distributions and possible implications in cardiovascular disease. The predictive modeling phase, highlighted by the stacked ensemble approach's resilience, stands out as an indicator of accuracy, attaining a final accuracy value of 88.16%. This combination of numerous modeling tools underlined the necessity of collaboration in enhancing the precision of heart disease mortality forecasts.</p>

## Disclaimer 
<p align="justify">The instructions and code used in the project are based on the provided guidelines. The program and dataset used for this gathered from the work of Lital Davar, retrieved from https://www.kaggle.com/code/litaldavar/heart-disease-classification/notebook?fbclid=IwAR2cdwNNp4vxBi9uz7WbOQonzs0qwT-eMuV4JVDBU4kgN8FGGptylk7p93k </p>
