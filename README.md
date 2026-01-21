# Support Vector Machine (SVM) Analysis

This directory contains an implementation of **Support Vector Machine (SVM)**, a robust supervised learning algorithm used for linear classification.

## Dataset Overview

The model uses the `Social_Network_Ads.csv` dataset, which includes:

- **Features**:
  - `Age`: Age of the user.
  - `EstimatedSalary`: Estimated salary of the user.
- **Target**:
  - `Purchased`: Binary classification (0 = No, 1 = Yes).

## Implementation Steps

The implementation follows these key steps:

1.  **Data Preprocessing**:
    - Split the dataset into Training set (75%) and Test set (25%).
    - Applied **Feature Scaling** to normalize Age and Estimated Salary, which is essential for SVM performance.
2.  **Model Training**:
    - Used `sklearn.svm.SVC` with a **linear kernel**.
    - Set `random_state = 0` for reproducibility.
3.  **Prediction and Evaluation**:
    - Predicted test set results.
    - Evaluated the model using a **Confusion Matrix** and **Accuracy Score**.
4.  **Visualization**:
    - Plotted the decision boundaries for the training and test sets to visualize how the linear kernel separates the two classes.

## Results

The linear SVM model achieved the following performance on the test set:

- **Accuracy**: 90%
- **Confusion Matrix**:
  - True Negatives: 66
  - False Positives: 2
  - False Negatives: 8
  - True Positives: 24
- The model successfully identifies a linear boundary to separate buyers from non-buyers based on demographic data.
