# Data-Mining

## Introduction 

Data is one of the valuable assets in any organisation or business as it helps them to make decisions and address critical challenges from the actionable insights that are drawn from it. Data preprocessing is one of the important steps in the data mining process as it involves data cleaning, data transforming and integrating of data to make it ready for analysis along with improving the quality of data and make it more suitable for the specific data mining task (Jain, 2019). I have discussed about the two datasets that is related to each other, one of which is stroke dataset, and the other is heart disease dataset. In these two datasets, there are some common columns such as age and  gender. These common attributes will provide a good foundation for comparing the risk factors of both stroke and heart disease, since they are known to significantly influence the likelihood of developing these conditions. 
This research focuses on the analysis on stroke and heart disease using Kaggle datasets, preparing and summarising the data in Python and henceforth presenting a data-driven approach toward the research questions which were associated with risk factors of stroke and heart diseases and other health trends.

## General Background

### Stroke: 
The stroke dataset focuses on understanding how a person’s health history and lifestyle choices relate to the risk of stroke. It highlights key factors like age, hypertension, and smoking habits, which play a major role in identifying the likelihood of a stroke. By analysing these factors, the dataset helps in predicting the risk of stroke and supports efforts to develop strategies for early diagnosis and prevention, ultimately aiming to reduce the impact of this serious health condition.

### Heart Disease: 
The heart disease dataset deals about various factors that influence the likelihood of heart disease, including demographic data, medical history, and lifestyle factors. It is commonly used to predict the presence of heart disease based on attributes such as age, cholesterol levels, blood pressure, and exercise habits. It helps in understanding the key risk factors associated with cardiovascular health and supports the development of predictive models for early detection.

## Plan Overview

### Acquisition of Relevant Datasets

#### Stroke: 
The stroke dataset “Stroke Prediction Dataset” is well-structured, making it suitable for data preprocessing and exploratory analysis. It is available in CSV format, which ensures compatibility with Python for seamless loading, cleaning, and analysis. By analysing the relationships among the attributes, the dataset enables the exploration of risk factors and patterns that can support preventive healthcare strategies. 

#### Heart Disease: 
The heart disease dataset “Identifying Risk Factors for Heart Disease” is obtained from Cleveland Heart Disease dataset (reddy, 2020) from Kaggle. The dataset is well-structured data with the CSV file extension. By examining the relationships between attributes such as age, cholesterol levels, and blood pressure, the dataset allows for the identification of key risk factors and patterns that can inform preventive healthcare measures for heart disease.

## Dataset Descriptions

### 1. Stroke Dataset

a.	Source: Kaggle (FEDESORIANO, 2021)

b.	Size: 5110 rows and 12 columns

c.	Fields of Interest: 

    i.	  Age: Age of the individual
    ii.	  Gender: Gender of the individual (Male or Female)
    iii.  Hypertension: Whether the individual has hypertension (1= Yes, 0=No)
    iv.	  HeartDisease: Whether the individual has heart disease (1= Yes, 0=No)
    v.    Ever_married: Whether the individual has ever been married (Yes/No)
    vi.   Work_type: Type of work the individual is involved in (Children, Private,Self-employed, Government job, Never worked)
    vii.  Residence_type: Type of Residence (Urban or Rural)
    viii. Avg_glucose_level: The average glucose level of the individual
    ix.	  Body Mass Index (BMI): The BMI of the individual
    x.	  Smoking status: Smoking status of the individual (formerly smoked or never smoked or smokes)
    xi.	  Stroke: Target variable indicating whether the individual has had a stroke (1= Yes, 0 = No)
d.	Relevance:     
This dataset is highly relevant for stroke prediction and prevention. By analysing its attributes, it helps to identify the key risk factors associated with stroke, which can guide healthcare providers in early detection and intervention.

### 2. Heart Disease Dataset

a.	Source: Kaggle (sethmuneeb, 2024)

b.	Size: 303 rows and 14 columns

c.	Fields of Interest: 

    i.	   Age: Age of the patient
    ii.	   Gender: Gender (1 for male, 0 for female)
    iii.   ChestPainp: Chest pain type (numeric values) 
    iv.	   Resting Blood Pressure
    v.     Cholesterol in mg/dl
    vi.	   Fasting Blood Sugar (1=true; 0=false)
    vii.   RestingECG: Resting Electrocardiographic Results
    viii.  MaxHeartRateAchieved
    ix.	   ExerciseInducedAngina (1=yes, 0=no)
    x.	   Oldpeak: ST depression induced by exercise relative to rest
    xi.	   Slope: Slope of the peak exercise ST segment (1: Normal, 2: Ischemia, 3: Higher risk of ischemia)
    xii.   MajorVessels: Number of Major Vessels (0-3) coloured by fluoroscopy
    xiii.  Thalassemia: Thalassemia (1= normal; 2=fixed; 3=reversible defect)
    xiv.   Target: Diagnosis of heart disease (0: No heart disease, 1, 2, 3, 4: increasing severity of heart disease, 5: specific/rare condition)
d.	Relevance:     
The dataset is highly relevant for predictive modelling and healthcare analytics. It provides valuable insights into identifying the risk factors for heart disease, which are crucial for early diagnosis and intervention. The dataset is used for building models to predict heart disease based on patient data, which can help healthcare professionals in decision-making and preventive care.

## Data Preparation

It is not sure whether the achieved dataset is error and consistency free or not. Therefore, there are some steps to be done to ensure the dataset is clean, complete and accurate. So, data preparation is the process of preparing the data for analysing and changing it for actionable insights (GeeksforGeeks, 2024).

For the preparation and further analysis, I am using Python programming language, which is used to conduct complex data mining techniques, create data visualisations, manipulate and analyse data, and many more (Coursera, 2023).

## Data Preprocessing

Data preprocessing is a methos which involves data cleaning, organisaing, and transforming data, making it ready and more effective for analysis and data mining.

### 1. Handling Missing values

When one or more values are absent in a dataset, missing values occur. It is important to handle missing values for accurate analysis. Incorrect and incomplete data results in inaccurate and misleading analysis. 

To handle the missing values, we have some common techniques:

1. Drop rows with missing values:

This is the easiest approach, but it may result in a significant loss of data.

2. Fill Missing value with a constant:

This method replaced missing value with a constant value, such as mean, median or mode of the feature.

3. Impute missing values with machine learning technology:

This is an advanced techniques like k-nearesr neighbours (KNN) imputation, matrix factorisation, or even train in a mcahine learning model to predict the missing values (sidhikha, 2024).

### 2. Removing Duplicate Data

When the same data is stored in a dataset, then the data is duplicate data.
Checking to see if there is any duplicate data. If yes,dropping the duplicate data.

### 3. Data Aggregation
It is a preprocessing task where the values of two or more objects are combined into a single object  (Koi.edu.au, 2024).

### 4. Data Discretisation
It is a data preprocessing step that is often used to transform a continuous-values attribute to a categorical attribute  (Koi.edu.au, 2024).

## Exploratory Data Analysis (EDA)

EDA is a process to explore and examine a dataset to understand its key features. This often involves using charts, graphs, and statistics to summarise and uncover patterns, trend, and relationships (IBM, 2020).

