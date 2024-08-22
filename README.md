# **Gamma Ray Detection Project**

**Overview**\
This project aims to develop a machine learning model to predict whether a detected event corresponds to a gamma ray (g) or a hadron (h) based on various measured features. The dataset used contains several features related to the characteristics of these events. The project involves data exploration, model development, evaluation, and additional techniques like anomaly detection and dimensionality reduction.

**Table of Contents**\
Project Overview\
Dataset Description\
Exploratory Data Analysis (EDA)\
Model Development\
Anomaly Detection\
Dimensionality Reduction\
Conclusion\
Future Work\
Usage\
Dependencies\


**Dataset Description**\
The dataset used in this project contains the following features:

fLength: Length of the object\
fWidth: Width of the object\
fSize: Size of the object\
fConc: Concentration\
fConc1: Concentration of the brightest spot\
fAsym: Asymmetry\
fM3Long: 3rd root of the long axis\
fM3Trans: 3rd root of the transverse axis\
fAlpha: Alpha angle\
fDist: Distance
Class: Target label (g for gamma ray, h for hadron)

**Exploratory Data Analysis (EDA)**\
EDA was performed to understand the distribution and relationships of the features within the dataset. Key activities include:

Feature Distribution: Histograms and density plots were used to visualize the distribution of each feature.

**Model Development**\
The primary goal was to classify events as either gamma rays or hadrons. The following steps were taken:

Random Forest Classifier: A Random Forest model was developed to predict the class of the events. This model was chosen for its robustness and ability to handle the complexities of the dataset.\
Model Evaluation: The model's performance was evaluated using accuracy, precision, recall, and confusion matrix metrics.\
Feature Importance: Important features contributing to the model's decision-making process were identified.\

**Anomaly Detection**\
An Isolation Forest model was used to detect anomalies in the dataset. A total of 951 potential anomalies were identified, which could represent unusual or rare observations.

**Dimensionality Reduction**\
Principal Component Analysis (PCA) was employed to reduce the dimensionality of the data:

PCA Analysis: The first two principal components explained the majority of the variance, allowing for visualization of the data in a lower-dimensional space.

**Conclusion**\
The project successfully developed a reliable model to classify gamma rays and hadrons. The insights gained from feature importance and anomaly detection added depth to the understanding of the dataset. The project has practical implications in fields like astrophysics, where accurate classification of events is crucial.

**Future Work**\
Potential areas for further exploration include:

Model Enhancement: Exploring more advanced techniques like ensemble methods or deep learning.\
Anomaly Analysis: Further investigation into the detected anomalies could provide valuable insights.\
Hyperparameter Tuning: Fine-tuning the model for improved accuracy.

**Dependencies**\
The following packages are required to run the project:

pandas\
numpy\
scikit-learn\
matplotlib\
seaborn
