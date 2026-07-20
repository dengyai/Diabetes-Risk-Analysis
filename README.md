# Diabetes-Risk-Analysis
The project is aimed at analyzing the risk of diabetes occurrence among patients by making use of different variables as provided by the dataset and those engineered for that purpose. 
Table of Contents
1.	Executive Summary	2
2.	Introduction	2
3.	Problem Statement	3
4. Project Objectives	3
4.1 Specific Objectives	3
5. Dataset Description	4
6. Methodology	5
7. Exploratory Data Analysis Summary	6
8. Machine Learning Model Development	6
Selected Model	6
9. Feature Importance Analysis	7
10. Future Diabetes Risk Projection	7
11. Recommendations	8
12. Limitations	8
13. Conclusion	8

 
DIABETES ANALYSIS DOCUMENTATION
Compiled by Dhulac Deng Yai and Abdulye Djibrine Nassir
(Nile Basin Analytics)

1.	Executive Summary 
This project aimed to develop a predictive machine learning model capable of identifying individuals at risk of diabetes using demographic, behavioral, and health-related variables from the BRFSS 2015 healthcare dataset. A comprehensive analytics workflow was implemented, including data cleaning, feature engineering, exploratory data analysis, dashboard development in Power BI, and predictive modeling using Logistic Regression, Decision Tree, and Random Forest algorithms.
Among the evaluated models, the Random Forest classifier achieved the best overall performance with an accuracy of 74.93%, a recall of 79.67%, an F1-score of 76.07%, and a ROC-AUC of 82.83%. These results demonstrate that the model can effectively distinguish individuals with diabetes from those without diabetes.
Feature importance analysis revealed that General Health, High Blood Pressure, Body Mass Index (BMI), Age Category, and High Cholesterol were the strongest predictors of diabetes. These findings reinforce existing clinical evidence that diabetes is closely associated with cardiovascular health, obesity, aging, and overall physical well-being.
The project demonstrates how Business Intelligence and Machine Learning can complement one another. Power BI dashboards provide descriptive insights into the current state of diabetes prevalence, while machine learning extends these insights by identifying individuals at elevated risk and highlighting the factors most strongly associated with diabetes. These outputs can support evidence-based decision-making, early screening initiatives, and targeted public health interventions.

2.	Introduction 
Diabetes mellitus is one of the most significant chronic diseases affecting populations worldwide. Its increasing prevalence places considerable pressure on healthcare systems due to long-term complications such as cardiovascular disease, kidney failure, vision impairment, and reduced quality of life. Early identification of individuals at high risk is essential for timely intervention and prevention.
Advances in data science and machine learning provide opportunities to analyze large healthcare datasets and identify complex patterns that may not be apparent through traditional statistical methods. Predictive models can support clinicians and policymakers by estimating diabetes risk and identifying the most influential contributing factors.
This project combines Business Intelligence and Machine Learning techniques to investigate diabetes risk using the Behavioral Risk Factor Surveillance System (BRFSS) 2015 dataset. The work includes descriptive analytics through Power BI dashboards and predictive analytics through supervised machine learning models.
3.	Problem Statement 
Healthcare organizations often collect large volumes of patient information but may not fully utilize these data to support proactive disease prevention. Traditional reporting methods primarily describe historical trends without identifying individuals who are most likely to develop or already have diabetes.
The challenge addressed in this project is to develop a predictive model that accurately classifies diabetes status while identifying the health, demographic, and lifestyle factors that contribute most significantly to diabetes risk. Such a model can support early screening, better allocation of healthcare resources, and evidence-based public health interventions.

4. Project Objectives 
To develop a comprehensive diabetes risk analysis and predictive analytics system by integrating Business Intelligence (Power BI) and Machine Learning techniques to identify the major factors associated with diabetes, predict diabetes risk, and support evidence-based healthcare decision-making.
4.1 Specific Objectives
The project aims to:
a)	Collect and analyze the BRFSS 2015 Diabetes Health Indicators dataset to understand the prevalence and distribution of diabetes. 
b)	Perform data cleaning, preprocessing, and feature engineering to improve data quality and prepare the dataset for analysis and machine learning. 
c)	Develop an interactive Power BI dashboard that provides descriptive and diagnostic insights into diabetes prevalence, demographic characteristics, lifestyle factors, and health indicators. 
d)	Explore the relationships between diabetes and major risk factors such as: 
a.	High Blood Pressure 
b.	High Cholesterol 
c.	Body Mass Index (BMI) 
d.	Age 
e.	Physical Activity 
f.	Smoking 
g.	General Health 
h.	Income Level 
i.	Education Level 
e)	Build and evaluate multiple machine learning classification models, including: 
a.	Logistic Regression 
b.	Decision Tree 
c.	Random Forest 
f)	Compare model performance using evaluation metrics such as: 
a.	Accuracy 
b.	Precision 
c.	Recall 
d.	F1-Score 
e.	ROC-AUC 
g)	Identify the most influential predictors of diabetes using Random Forest Feature Importance analysis. 
h)	Develop a predictive model capable of estimating an individual's likelihood of having diabetes based on demographic, behavioral, and clinical characteristics. 
i)	Provide data-driven recommendations to support healthcare professionals, policymakers, and public health organizations in designing effective diabetes prevention and intervention strategies. 
j)	Demonstrate how Business Intelligence and Machine Learning can be integrated into a single decision-support solution for healthcare analytics. 

5. Dataset Description 
Attribute	Value
Dataset	BRFSS 2015 Diabetes Health Indicators
Total Records	70,692
Features	22
Target Variable	Diabetes Status
Predictor Variables	21
Missing Values	None
Class Balance	50% Diabetic | 50% Non-Diabetic


6. Methodology 

Business Understanding
│
Data Understanding
│
Data Cleaning
│
Feature Engineering
│
Exploratory Data Analysis
│
Power BI Dashboard
│
Machine Learning
│
Model Evaluation
│
Feature Importance
│
Recommendations


7. Exploratory Data Analysis Summary 
The Exploratory Data Analysis provided a comprehensive understanding of the diabetes dataset and identified the variables most strongly associated with diabetes. These findings guided the subsequent stages of the project, including feature engineering, dashboard development, and predictive modeling.
The EDA confirmed that General Health, High Blood Pressure, Body Mass Index (BMI), Age Category, and High Cholesterol are the most influential factors associated with diabetes. These insights were later validated through the Random Forest model, which identified the same variables as the leading predictors of diabetes risk.
Overall, the exploratory analysis established a strong analytical foundation for the Business Intelligence dashboards and the machine learning models, enabling reliable predictive analytics and supporting data-driven healthcare decision-making.

8. Machine Learning Model Development 
Model	Accuracy	Precision	Recall	F1 Score	ROC-AUC
Logistic Regression	74.59%	73.72%	76.40%	75.04%	82.32%
Decision Tree	73.99%	71.77%	79.09%	75.25%	81.54%
Random Forest	74.93%	72.77%	79.67%	76.07%	82.83%
Selected Model
Random Forest was selected because it achieved the strongest overall balance of predictive performance, particularly in recall and ROC-AUC.

9. Feature Importance Analysis 
Rank	Risk Factor	Importance
1	General Health	22.31%
2	High Blood Pressure	18.99%
3	BMI	14.06%
4	Age Category	10.06%
5	High Cholesterol	8.98%
6	Difficulty Walking	4.73%
7	Income Level	3.86%
8	Physical Health	3.49%
9	Heart Disease	2.75%
10	Mental Health	1.82%

10. Future Diabetes Risk Projection 
It is important to interpret this carefully.
Your model predicts the current probability that an individual belongs to the diabetic class based on the available features. It does not forecast future disease incidence over time because the BRFSS dataset is cross-sectional rather than longitudinal.
However, the model supports evidence-based projections:
a)	Individuals with poor general health, hypertension, elevated BMI, older age, and high cholesterol consistently receive higher predicted diabetes risk. 
b)	Communities with a greater concentration of these risk factors are likely to have a higher future burden of diabetes if no preventive action is taken. 
c)	Public health interventions focused on these high-risk groups have the greatest potential to reduce future diabetes prevalence. 




11. Recommendations 
Clinical
a)	Increase routine diabetes screening for individuals with hypertension, obesity, and poor general health. 
b)	Integrate cholesterol monitoring into diabetes prevention programs. 
Community
a)	Promote regular physical activity and healthy eating. 
b)	Expand health education targeting older adults and underserved populations. 
Policy
a)	Improve access to preventive healthcare and chronic disease management. 
b)	Support programs addressing socioeconomic barriers that influence health outcomes. 
Analytics
a)	Deploy the Random Forest model as a clinical decision-support tool, with appropriate validation and governance. 
b)	Retrain and recalibrate the model periodically using newer and more representative datasets.
12. Limitations 
a)	The dataset represents a single point in time and cannot directly model disease progression. 
b)	Predictor variables are based largely on self-reported survey responses. 
c)	External validation on independent datasets would strengthen confidence in the model's generalizability. 
d)	The model is intended to support, not replace, clinical judgment.
13. Conclusion 
This project demonstrates a complete end-to-end healthcare analytics workflow, combining Business Intelligence with Machine Learning to produce descriptive, diagnostic, and predictive insights. The Random Forest model provided the strongest overall predictive performance, while feature importance analysis highlighted general health, hypertension, BMI, age, and cholesterol as the primary contributors to diabetes risk. These findings support targeted screening, preventive interventions, and data-driven healthcare planning.
