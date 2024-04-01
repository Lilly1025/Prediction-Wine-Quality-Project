# **Red Wine Quality Prediction**
## Description

**Red Wine Quality Prediction** is Machine Learning project for 01418362 
(Introduction to Machine Learning). This project use red wine dataset from [Vinho Verde] 
https://archive.ics.uci.edu/dataset/186/wine+quality 

The goal is to model wine quality based on **all** and **Selected features** 
of physicochemical with Support Vector Machine 
Target is quality that:
* quality <= 5 is bad wine
* quality > 5 is good wine

**ATTENTION PLEASE**
* เลือก V2.0.0 เป็น version ที่จะนำเสนอ เนื่องจากข้อมูลมีความสมดุลกัน ขนาดเท่าๆกัน ทำให้ได้เห็นประสิทธิภาพที่แท้จริงของโมเดล มีการปรับค่า parameter
  เพื่อจูนโมเดลตามหลักของ Gradient descent
  
## Data Information
Input Variables:
* **fixed acidity:** most acids involved with wine or fixed or nonvolatile
* **volatile acidity:** the amount of acetic acid in wine
* **citric acid:** found in small quantities, citric acid can add 'freshness' and flavor to wines
* **residual sugar:** the amount of sugar remaining after fermentation stops
* **chlorides:** the amount of salt in the wine
* **free sulfur dioxide:** the free form of SO2 exists in equilibrium between molecular SO2 (as a dissolved gas) and bisulfite ion
* **total sulfur dioxide:** amount of free and bound forms of S02
* **density:** the density of water is close to that of water depending on the percent alcohol and sugar content
* **pH:** describes how acidic or basic a wine is on a scale from 0 (very acidic) to 14 (very basic)
* **sulphates:** a wine additive which can contribute to sulfur dioxide gas (S02) levels
* **alcohol:** the percent alcohol content of the wine

Output Variable:
* **quality**: output variable (based on sensory data, score between 0 and 10)

## Getting Started

### Dependencies
* python
* VS code
```
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn import preprocessing 
plt.style.use("ggplot")  #using style ggplot
from sklearn.metrics import accuracy_score, confusion_matrix
```
### Installing
```
git clone https://github.com/Lilly1025/Red-Wine-Quality-Prediction_ML_Project.git
```
Red-Wine-Quality-Prediction_ML_Project
* All_features
  * All_red_wine_SVM_**original**.ipynb - (SVM)
  * All_red_wine_SVM_**V1.0.0**.ipynb - (SVM with unbalance data, eliminate outliers)
  * All_red_wine_SVM_**V2.0.0**.ipynb - (SVM with balance data, eliminate outliers)
    
* Selected_features
  * feature_selected_red_wine_SVM_**original**.ipynb - (SVM)
  *  feature_selected_red_wine_SVM_**V1.0.0**.ipynb - (SVM with unbalance data, eliminate outliers)
  *  feature_selected_red_wine_SVM_**V2.0.0**.ipynb - (SVM with balance data, eliminate outliers)
  *  feature_selected_red_wine_SVM_**V3.0.0**.ipynb - (SVM with balance data, eliminate outliers, features scaling)

* winequality-red.csv

### Program Outline

* Import Libralies
* Load Red Wine Dataset
* Preprocessing Data for binary classification
* Detect & Deal With Outliers
* Select features and target Variables
* Split data set to training & test set
* Training SVM Model
* Predict using the trained SVM model
* Future Predictions
* Calculate the hinge loss for the test data
* Confusion Matrix
* Future Predictions
* Calculate the hinge loss for the future prediction
* Decision Boundary of SVM (for Selected_features)
  
```
Run all
```

## Authors

Pornpailin Kamonsantisuk
6310401068 หมู่ 1
