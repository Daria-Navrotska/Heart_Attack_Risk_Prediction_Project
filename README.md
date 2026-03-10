# Heart Attack Risk Prediction Project


## Project Overview
This repository presents a comprehensive exploratory analysis of a synthetic Heart Attack Risk Prediction dataset sourced from Kaggle. The objective is to uncover meaningful patterns in cardiovascular risk factors and generate insights that support preventive strategies and public health awareness. The analysis investigates key questions such as which features most strongly correlate with heart attack risk, how age and cholesterol levels influence outcomes. It also explores clustering and regression techniques to assess variable relationships and identify subtle trends across global populations. The dataset’s rich mix of clinical, behavioral, and geographic features enables a holistic view of heart health across diverse patient profiles.

<img width="617" height="436" alt="image" src="https://github.com/user-attachments/assets/d4400e81-6a11-4229-b000-1ad468e7b35d" />


## Key Questions
-  Which features are most correlated with heart attack risk?
-  How does heart attack risk vary across age groups?
-  Is there a relationship between cholesterol levels and heart attack risk?
-  Do lifestyle factors (e.g., exercises) significantly impact risk?
-  How do multiple risk factors interact to influence outcomes? 


## Folders
- 01 Project Management: project brief;
- 02 Data Profile: data files used and processed;
- 03 Scripts: Jupyter notebooks containing codes;
- 04 Analysis: contains the visualizations generated through the analysis.

<img width="373" height="281" alt="image" src="https://github.com/user-attachments/assets/84f75412-c015-4c2a-8ee5-77479317c991" />


## Tools and Techniques:
1. The data was analyzed using Python and the following supporting libraries:
- Pandas: for data analysis, 
- Numpy: for mathematical equations, 
- Seaborn: for data visualizations, 
- Matplotlib: for data visualizations (pyplot, Pylab), 
- SciPy: for mathematical equations, 3D Visualisation,
- Folium: to create interactive geographic maps in Python,
- Json: to handle structured data format,
- Sklearn: for applying machine learning techniques such regression and clustering.
2. Exploratory Data Analysis (EDA) to uncover trends, correlations, and health risk patterns.
3. Folium & JSON used for interactive geographic mapping and handling structured data formats.
4. Regression & Clustering Models applied to assess relationships and group individuals based on health profiles. 
5. Time-Series Analysis used to explore historical cardiovascular mortality trends from WHO data.


## Insights

1. The data reveals that heart health and lifestyle indicators show minimal predictive value for heart attack risk in the investigated data sample, despite their known clinical relevance.

There are a very weak negative relationship between Heart Rate, Family Hear Problems, Smoking, Obesity, Alcohol Consumption, Stress Level, Sedentary Hours Per Day, Physical Activity Days Per Week, Sleep Hours Per Day and Heart Attack Risk indicating no meaningful linear relationship between mentioned parameters and heart attack risk based on explored data (despite the common medical knowledge linking some of them to cardiovascular issues).

<img width="923" height="844" alt="image" src="https://github.com/user-attachments/assets/70572cf6-f73f-41cd-9e5f-7af5273f7c42" />


2. Among all countries, the USA, France, and Vietnam show leading average cholesterol levels and Heart Attack Risks, accordingly.

- Cholesterol is a key heart risk factor, making its global distribution a revealing health indicator.
- USA, France, and Vietnam rank among the global leaders in average cholesterol levels.
- However, Cholesterol Level alone do not reliably predict Heart Attack Risk, according to correlation data. 

<img width="1890" height="660" alt="image" src="https://github.com/user-attachments/assets/7398c035-8653-47db-91c3-5648da59a131" />


3. Heart Attack Risk increases notably with age, making it a primary influencing factor (even so no linear regression, no clustering model can’t accurately predict this relation in the investigated dataset).

Age is a probably primary driver of Heart Attack Risk, with older individuals showing significantly higher risk levels. It was choosen as a hypothesis of this analysis.

<img width="848" height="663" alt="image" src="https://github.com/user-attachments/assets/9666c689-e47d-4019-b019-80822d004049" />

Results demonstrate that the Age has a weak and uneven influence on Heart Rate, with only a slight downward trend observed. It is suggested that Age is not a strong predictor of Heart Rate in the analysed dataset - at least not linearly. Moreover, regression line doesn’t perfectly cover all of data points.

<img width="985" height="740" alt="image" src="https://github.com/user-attachments/assets/211fbd2d-5ec4-49f7-9576-d02c368c9645" />

Performed clustering analysis doesn’t reflect a strong or clean separation. The data points across clusters 0, 1, and 2 were densely packed and show considerable overlap missing clear boundary or distinct grouping that separates one cluster from another.
This suggests that individuals of similar Age have a broad range of Heart Rates, and vice versa.

<img width="722" height="502" alt="image" src="https://github.com/user-attachments/assets/d54197bf-17d7-4db6-a0c2-146ed90fe1ce" />

3D clustering by Age, Heart Rate, and Body Mass Index (BMI) showed no clear separation, though color-coded groups suggest general trends: 0 - younger individuals with higher heart rate and lower BMI, 1 - middle-aged with moderate values, and 2 - older individuals with higher BMI and lower heart rate. The complex effects of these parameters are difficult to discuss due to the significant overlap.

<img width="603" height="577" alt="image" src="https://github.com/user-attachments/assets/e0c5f937-fb0e-4296-a41c-922e6f3e7d42" />


## Recommendations and Next Steps
- Perform analysis on real medical data with less binary variables
- Analyse impact of other factors on the Heart Attack Risk and their complex effect
- Just like real estate agents use clusters to tailor marketing, healthcare providers can usethis approach to design targeted wellness programs, prioritize diagnostics, or personalize treatment plans
- Analysis could be useful proxy for educational and further exploratory analysis.
<img width="638" height="623" alt="image" src="https://github.com/user-attachments/assets/15ce65a4-4d75-4b0a-a817-8d4b713349fd" />


## Link to Tableau storyboard
https://public.tableau.com/views/HeartAttackRiskPredictionProject/IntroCVDandHeartAttackRisk?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
The storyboard doesn’t contain every step was taken through analysis — only those relevant to the final results.


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
