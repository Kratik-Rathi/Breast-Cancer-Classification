# Breast Cancer Classification

## Overview

This repository implements a machine learning pipeline for breast cancer classification using a dataset containing features of breast tumors. The goal is to predict whether a tumor is benign or malignant based on its features. The project compares several classification algorithms and evaluates their performance to select the best model for this task.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Modeling Process](#modeling-process)
- [Algorithms Used](#algorithms-used)
- [Results](#results)


## Dataset

The dataset used in this project is the **Breast Cancer Wisconsin dataset**, which includes measurements of various features (such as radius, texture, smoothness, etc.) for tumors, each labeled as benign or malignant. The dataset is available in the form of a CSV file (`breast_cancer.csv`) and is split into training and testing sets.

### Key Features:
- `radius_mean`: Mean of distances from center to points on the perimeter.
- `texture_mean`: Standard deviation of gray-scale values.
- `smoothness_mean`: Local variation in radius lengths.
- And several other features describing texture, compactness, concavity, etc.

## Modeling Process

The project involves several preprocessing steps to prepare the data for machine learning models:
1. **Data Cleaning**: Missing values, if any, are handled appropriately.
2. **Feature Scaling**: Scaling is applied to ensure that all features contribute equally to the model.
3. **Train-Test Split**: The dataset is split into training and testing sets (80% training, 20% testing).

After preprocessing, several models are trained and evaluated:
- **Logistic Regression**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**

## Algorithms Used

- **Logistic Regression**: A statistical model used to model binary outcomes. It estimates probabilities and classifies the tumors as benign or malignant.
  
- **Random Forest**: An ensemble learning method using multiple decision trees to improve accuracy and reduce overfitting.
  
- **Support Vector Machine (SVM)**: A powerful classification technique that maximizes the margin between classes.
  
- **K-Nearest Neighbors (KNN)**: A simple classification algorithm based on the closest points in the feature space.

## Results

The performance of each model is evaluated on the test set using metrics such as accuracy, precision, recall, and F1-score. Here are the results:

- **Logistic Regression**:
  - Accuracy: 95%
  - Precision: 94%
  - Recall: 96%
  - F1-Score: 95%

- **Random Forest**:
  - Accuracy: 98%
  - Precision: 97%
  - Recall: 99%
  - F1-Score: 98%

- **Support Vector Machine (SVM)**:
  - Accuracy: 97%
  - Precision: 96%
  - Recall: 98%
  - F1-Score: 97%

- **K-Nearest Neighbors (KNN)**:
  - Accuracy: 94%
  - Precision: 93%
  - Recall: 95%
  - F1-Score: 94%

### Best Model
The **Random Forest** algorithm achieved the highest accuracy and balanced precision and recall, making it the best-performing model for this classification task.
