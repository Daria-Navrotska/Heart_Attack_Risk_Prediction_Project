# Heart Attack Risk Prediction Project

## Project Overview
This repository presents a comprehensive exploratory analysis of a synthetic Heart Attack Risk Prediction dataset sourced from Kaggle. The objective is to uncover meaningful patterns in cardiovascular risk factors and generate insights that support preventive strategies and public health awareness. The analysis investigates key questions such as which features most strongly correlate with heart attack risk, how age and cholesterol levels influence outcomes. It also explores clustering and regression techniques to assess variable relationships and identify subtle trends across global populations. The dataset’s rich mix of clinical, behavioral, and geographic features enables a holistic view of heart health across diverse patient profiles.


## Key Questions
-  Which features are most correlated with heart attack risk?
-  How does heart attack risk vary across age groups?
-  Is there a relationship between cholesterol levels and heart attack risk?
-  Do lifestyle factors (e.g., exercises) significantly impact risk?
-  How do multiple risk factors interact to influence outcomes? 


## Folders
-01 Project Management: Project brief;
-03 Scripts: Jupyter notebooks containing codes;
-04 Analysis: 'Visualizations' subfolder contains the visualizations generated through the analysis;

## Tools
The data was analyzed using Python and the following supporting libraries:
-Pandas: for data analysis, 
-Numpy: for mathematical equations, 
-Seaborn: for data visualizations, 
-Matplotlib: for data visualizations (pyplot, Pylab), 
-SciPy: for mathematical equations, 3D Visualisation,
-Folium: to create interactive geographic maps in Python,
-Json: to handle structured data format,
-Sklearn: for applying machine learning techniques such regression and clustering.

## Link to Tableau storyboard
https://public.tableau.com/views/HeartAttackRiskPredictionProject/IntroCVDandHeartAttackRisk?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Data Sources
“The Heart Attack Risk Prediction Dataset” accessed from (https://www.kaggle.com/datasets/ghnshymsaini/heart-attack-risk-prediction-dataset?resource=download) via Kaggle.
Note:  It is a synthetic dataset created for research and educational purposes. It likely draws inspiration from established clinical datasets such as the Cleveland Heart Disease dataset or other public health repositories. The dataset, consisting of 8763 records from patients around the globe.

For the Time Series analysis was used "Death rate from cardiovascular diseases, 1950 to 2023" dataset from the WHO Mortality Database (2025) with minor processing by Our World in Data (https://archive.ourworldindata.org/20250909-093708/grapher/cardiovascular-disease-death-rate-who-mdb.html?time=earliest..2023#sources-and-processing). It is reported deaths from cardiovascular diseases in both sexes in those aged all ages per 100,000 people.

## Dataset Glossary (Column-wise): 
1. Patient ID: Unique identifier for each patient. 
2. Age: Age of the patient (numerical). 
3. Gender:  Sex of the patient (categorical: Male/Female). 
4. Cholesterol Level: Cholesterol levels of the patient (numerical), mg/dL 
5. Blood Pressure: Blood pressure of the patient (categorical or numerical depending on the 
format, likely represented as systolic/diastolic). 
6. Heart Rate: Heart rate of the patient (numerical). 
7. Diabetes: Whether the patient has diabetes (binary: Yes/No). 
8. Family Heart Problems:  
Family history of heart-related problems (binary: 1 for Yes, 0 for No). 
9. Smoking: Smoking status of the patient (binary: 1 for Smoker, 0 for Non-smoker). 
10. Obesity: Obesity status of the patient (binary: 1 for Obese, 0 for Not obese). 
11. Alcohol Consumption:  
Level of alcohol consumption by the patient (categorical: None/Light/Moderate/Heavy). 
12. Exercise Hours Per Week: Number of exercise hours per week (numerical). 
13. Diet: Dietary habits of the patient (categorical: Healthy/Average/Unhealthy). 
14. Previous Heart Problems:  
Previous heart problems of the patient (binary: 1 for Yes, 0 for No). 
15. Medication Use: Medication usage by the patient (binary: 1 for Yes, 0 for No). 
16. Stress Level: Stress level reported by the patient (numerical, scale 1-10). 
17. Sedentary Hours Per Day: Hours of sedentary activity per day (numerical). 
18. Income: Income level of the patient (numerical). 
19. Body Mass Index: BMI of the patient (numerical). The BMI is expressed in kg/m2, resulting 
from patient mass in kilograms and height in metres. 
20. Triglyceride Levels: Triglyceride levels of the patient (numerical), mg/dL 
21. Physical Activity Days Per Week: Days of physical activity per week (numerical). 
22. Sleep Hours Per Day: Hours of sleep per day (numerical). 
23. Country: Country of the patient (categorical). 
24. Continent: Continent where the patient resides (categorical). 
25. Hemisphere: Hemisphere where the patient resides (categorical). 
26. Heart Attack Risk: Target Variable.  
Presence of heart attack risk (binary: 1 for Yes, 0 for No). 
