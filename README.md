📌 Project Title

Predicting Bean Varieties with Feature Engineering and ML

👤 Author

Name: HANAN PV

🧠 Problem Statement

In agricultural and food industries, the accurate classification of dry beans is essential for quality control, pricing, and processing automation. Traditionally, bean classification is performed manually, which is time-consuming, labor-intensive, and prone to human errors. This project aims to develop a machine learning model that can automatically classify dry beans based on their morphological characteristics, improving efficiency and accuracy in classification.
🎯 Objective
The goal of this project is to build a predictive model that can classify different varieties of dry beans based on their shape and geometric features. Using supervised machine learning techniques, the model will analyze key morphological attributes such as area, perimeter, aspect ratio, roundness, and compactness to distinguish between different bean types.


📚 Data Description

Source:UCI Machine Learning Repository

Features:
area:The total number of pixels within the bean region (bean size).

perimeter:The total boundary length of the bean shape.

major axis length:The longest axis length of the fitted ellipse around the bean.

minor axis length:The shortest axis length of the fitted ellipse around the bean.

aspect ratio:The ratio of MajorAxisLength to MinorAxisLength (elongation).

eccentricity:The measure of how much the bean shape deviates from being a circle.

convex area:The total number of pixels within the convex hull of the bean.

equivdiameter:The diameter of a circle with the same area as the bean.

extent:The ratio of the bean's area to the bounding box area (compactness).

solidity:The ratio of bean area to convex hull area (density of the shape).

roundness:A measure of how circular the bean is, calculated as (4 × Area) / (π × Perimeter²).

compactness:A shape factor measuring how compact or spread out the bean is.

shapfactor1: A shape factor based on area and perimeter.

shapfactor2:Another shape factor derived from area and major axis length.

shapfactor3:A shape factor using area, perimeter, and major axis length.

shapfactor4:A final shape factor that includes perimeter and minor axis length.

Target variable: CLASS
The dataset consists of 7 different dry bean varieties, classified as follows:

SEKER

BARBUNYA

BOMBAY

CALI

DERMASON

HOROZ

SIRA

Data Type: Mixed (Numerical + Categorical)

🔍 Project Steps

1️⃣ Data Preprocessing

there is no missig values

Outlier detection and removal using IQR

Skewness checked and visualized before and after cleaning

2️⃣ Exploratory Data Analysis (EDA)

Histogram
Heat map
Boxplot
Pie chart
Barplot
Count plot
Kernel Density Estimation (KDE)

3️⃣ Feature Engineering

One-hot encoding for categorical variables 

Ensured all model inputs are numeric

4️⃣ Feature Selection

Used SelectKBest with chi2 test

Applied feature scaling (StandardScaler)

5️⃣ Model Training and Evaluation

Split data into training and testing sets

Models Trained:

Logistic Regression 
Decision Tree
Naive Bayes
Random Forest 
K-Nearest Neighbors (KNN) 
Gradient Boosting 

Metrics used:Confusion Matrix, Accuracy, Precision, Recall, F1-Score, ROC Curve.

6️⃣ Hyperparameter Tuning

GridSearchCV used to tune Random Forest parameters

7️⃣ Model Saving

Best model (Random Forest) saved using joblib

8️⃣ Prediction on Unseen Data
Predict on synthetic unseen data

conclution


