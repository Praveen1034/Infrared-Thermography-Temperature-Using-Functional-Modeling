# **Infrared Thermography Temperature Prediction Using Functional Modeling**

This repository contains a project aimed at predicting infrared thermography temperature measurements using functional modeling and deep learning techniques. The model leverages a multi-output architecture to predict average oral temperatures for males (aveOralM) and females (aveOralF).

**Overview**

Infrared thermography is a non-invasive technique widely used in various applications, including healthcare, to measure body temperature. This project utilizes the Infrared Thermography Temperature Dataset from the UCI Machine Learning Repository to develop a predictive model. The model employs functional modeling with a deep neural network to achieve accurate predictions for both male and female oral temperatures.

**Dataset**
+ Source: UCI Machine Learning Repository - Infrared Thermography Temperature Dataset
+ Features: The dataset includes features derived from infrared thermography.

+ Targets:
> aveOralF: Average oral temperature for females.
> aveOralM: Average oral temperature for males.

**Project Highlights**
+ Functional Model Architecture
+ The functional modeling approach allows for flexibility in constructing multi-output deep learning models. The architecture includes:

+ Input Layer: Accepts preprocessed feature data.
+ Hidden Layers: Three densely connected layers with ReLU activation functions to capture complex patterns in the data.
+ Output Layers: Two separate linear output layers for predicting aveOralF and aveOralM.

**Training**
+ The model was trained using the following configurations:

+ Loss Function: Mean Squared Error (MSE) for both outputs.
+ Optimizer: Adam optimizer for efficient training.
+ Metrics: Mean Absolute Error (MAE) was used as an additional performance metric.
+ Early Stopping: Implemented to prevent overfitting by monitoring validation loss.

**Preprocessing**
+ Data was scaled using Min-Max Scaler to normalize feature values.
+ The dataset was split into training and validation sets for model evaluation.

**Results**
+ The model achieved promising results in predicting the target variables, as assessed by metrics such as MSE, MAE, and R² score.
