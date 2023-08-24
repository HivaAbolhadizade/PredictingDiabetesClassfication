# Predicting Diabetes Risk Using Health Indicators - Machine Learning Approach
This repository presents a machine learning model designed to predict whether individuals are at risk of diabetes based on specific health indicators. The aim of this project is to develop a predictive system that can assist healthcare professionals in diagnosing diabetes. The analysis is performed on the 2015BRFSS dataset, involving various preprocessing steps such as removal of duplicate data, dataset binarization, data balancing, and dimensionality reduction. The primary goal is to create a robust model capable of determining an individual's likelihood of developing diabetes. The models have been trained on the Diabetes Health Indicators Dataset available on Kaggle.
## Dataset:
The dataset can be accessed at https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset. It comprises data related to various health indicators such as blood glucose levels, blood pressure, body mass index, etc., for individuals, along with their diabetes status.
## Data Preprocessing:
Upon thorough examination of the data, it was discovered that there were some duplicated observations within the dataset. To enhance the model's learning process, these duplicate entries were removed. Furthermore, diabetes and prediabetes groups were merged, transforming the model into a binary classification problem.
## Impact of Features:
The impact of different features on the risk of diabetes was investigated using the Hit-map method, and among them, 17 features that had the most significant impact on the susceptibility to diabetes were identified.
## Data Balancing:
It was found that the available data in the two distinct classes, diabetic and prediabetic, is imbalanced, and there is a significant disparity in the number of observations. Initially, various methods were employed, including Random down-sampling, NearMiss algorithm, Cluster Centroid, SMOTE, and SMOTE with Edited Nearest Neighbors, in an attempt to balance the data.
After applying various techniques to balance the data and utilizing the selectKbest algorithm from the sklearn library to identify less impactful features and remove them, the dataset was prepared in a more optimized manner.
## Model Training:
Following data preprocessing, which includes normalization and removal of unnecessary data, various models, including Logistic Regression, Decision Tree, K Nearest Neighbors (KNN), Random Forest, Support Vector Machines (SVM), and XGBoost, were trained.
## Selecting the Best Model:
By comparing the accuracies of the models, it was determined that the data-balancing approach had the most significant impact on the models. Weighted and random down-sampling techniques resulted in better accuracy for the models.
In the end, two models with higher accuracy were chosen: K Nearest Neighbors (KNN) with random down-sampling for balanced data, achieving an F1-score of weighted avg = 0.779 and macro avg = 0.602, and the XGBoost model.
![image](https://github.com/HivaAbolhadizade/PredictingDiabetesClassfication/assets/96919633/6849caa2-5324-46b1-a22d-3e9a86e6d337)

## Conclusion:
Considering the F1-score metric, the XGBoost model was identified as the best choice for predicting diabetes risk. It took into account data balancing through the weighting parameter in the two classes, achieving an F1-score of weighted avg = 0.784 and macro avg = 0.665. This project underscores the potential of accurate diabetes risk prediction through careful data analysis and appropriate model selection.
![image](https://github.com/HivaAbolhadizade/PredictingDiabetesClassfication/assets/96919633/d06834ff-253a-4c33-b233-2495aff41924)

## Prepared by:
Zahra Hosseini
Najme Navabizade
and me:)

