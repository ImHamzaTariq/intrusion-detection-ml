#  AI-Based Intrusion Detection System

## Overview

This project implements a machine learning-based intrusion detection
system to classify network traffic as either **normal** or **attack**.
It uses the **KDD Cup 99 dataset**, a widely recognized benchmark
dataset in cybersecurity research.

The goal of this project is to demonstrate how machine learning
techniques can be applied to detect malicious network activity and
improve system security.

------------------------------------------------------------------------

##  Objectives

-   Build a binary classification model for intrusion detection\
-   Apply data preprocessing techniques to mixed-type features\
-   Evaluate model performance using standard classification metrics\
-   Analyze feature importance to understand network behavior patterns

------------------------------------------------------------------------

##  Dataset

-   **Dataset**: KDD Cup 99 (SA subset via scikit-learn)\
-   **Type**: Network traffic data\
-   **Classes**:
    -   `normal` → legitimate traffic\
    -   `attack` → malicious traffic

------------------------------------------------------------------------

##  Technologies Used

-   Python\
-   Scikit-learn\
-   Pandas\
-   NumPy\
-   Matplotlib

------------------------------------------------------------------------

##  Methodology

### 1. Data Preprocessing

-   Handling missing values using imputation\
-   Encoding categorical variables using **One-Hot Encoding**\
-   Scaling numerical features using **StandardScaler**

### 2. Model

-   **Random Forest Classifier**
    -   Robust and effective for tabular data
    -   Handles non-linear relationships well

### 3. Pipeline

A full machine learning pipeline was built using: - `ColumnTransformer`
for preprocessing - `Pipeline` for combining preprocessing and model
training

------------------------------------------------------------------------

##  Results

  Metric      Value
  ----------- --------
  Accuracy    99.96%
  Precision   1.00
  Recall      0.9867
  F1-score    0.9933

------------------------------------------------------------------------

##  Key Insights

-   Network traffic patterns such as **connection counts** and **byte
    transfer features** are strong indicators of malicious activity\
-   Protocol-related features (e.g., ICMP) significantly influence
    detection\
-   The model demonstrates excellent capability in detecting attacks
    with minimal errors

------------------------------------------------------------------------

##  Limitations

-   The KDD Cup 99 dataset is **outdated** and contains redundant
    patterns\
-   Results may not fully generalize to modern real-world network
    environments

------------------------------------------------------------------------

##  Future Work

-   Apply the model to modern datasets such as **UNSW-NB15**\
-   Extend to **multi-class classification** of attack types\
-   Experiment with advanced models (XGBoost, LightGBM, Deep Learning)

------------------------------------------------------------------------

##  Project Structure

intrusion-detection-ml/ │ ├── intrusion_detection.ipynb ├── README.md

------------------------------------------------------------------------

##  Author

Muhammad Hamza

------------------------------------------------------------------------

