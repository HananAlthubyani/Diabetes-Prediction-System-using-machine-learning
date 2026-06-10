# Diabetes-Prediction-System-using-machine-learning
Design and develop a  machine learning model to predict whether a person has diabetes or not based on medical diagnostic features.
# Diabetes Prediction Using Machine Learning

## Project Overview

This project aims to predict diabetes using machine learning techniques. The dataset was preprocessed to improve data quality and model performance. Several preprocessing steps were applied, including outlier removal, feature scaling, and class balancing. Finally, machine learning models were trained and evaluated to identify the most effective approach for diabetes classification.

## Dataset

The project uses the Pima Indians Diabetes Dataset, which contains medical and demographic information related to diabetes diagnosis.

## Data Preprocessing

### 1. Outlier Removal

Outliers were detected and removed to reduce noise and improve the quality of the dataset. This step helped improve the model's ability to learn meaningful patterns from the data.

### 2 . Handling Invalid Zero Values

Several features in the dataset contained zero values that are not medically meaningful, including Glucose, BloodPressure, SkinThickness, Insulin, and BMI. These invalid zero values were replaced using the K-Nearest Neighbors (KNN) Imputer, which estimates appropriate values based on the similarity between neighboring samples. This process helped improve data quality and reduce the impact of unrealistic measurements.

### 3. Feature Scaling

Min-Max Normalization was applied to scale all features into the range [0,1]. This ensures that features with larger values do not dominate the learning process.

### 4. Data Balancing

The dataset was highly imbalanced. To address this issue, the Synthetic Minority Oversampling Technique (SMOTE) was applied to generate synthetic samples for the minority class and achieve a balanced class distribution.



## Models Used

### Random Forest

Random Forest was trained using the balanced and normalized dataset.

### XGBoost

XGBoost was also trained and evaluated for comparison with Random Forest.

## Model Evaluation

The models were evaluated using the following metrics:

* Accuracy
* Precision
* Recall
* F1-Score

### Results

| Model         | Accuracy | Precision | Recall | F1-Score |
| ------------- | -------- | --------- | ------ | -------- |
| XGBoost       | 0.76     | 0.60      | 0.65   | 0.63     |
| Random Forest | 0.77     | 0.61      | 0.75   | 0.67     |

## Conclusion

The Random Forest model achieved the best overall performance. It outperformed XGBoost across all evaluation metrics, particularly in recall, which increased from 0.65 to 0.75. Since recall is a critical metric in diabetes prediction, Random Forest was selected as the preferred model for this project.

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Imbalanced-learn (SMOTE)
* XGBoost
* Matplotlib
* Seaborn
* Jupyter Notebook

## Author
Hanan Althubyani 

Hanan Al-Dhabyani
