# Flood Prediction in Kerala

## Problem Statement

Floods are a recurring natural disaster that can have devastating effects on communities. The ability to predict the occurrence of floods is crucial for implementing timely preventive measures and minimizing the impact on human lives and infrastructure. This project focuses on predicting the likelihood of floods in Kerala based on historical rainfall data.

## Dataset

The dataset used for this project contains historical rainfall data for Kerala, spanning several years. Each record includes monthly rainfall values and an indicator for whether a flood occurred during that period.

### Data Columns

- `YEAR`: The year of the record
- Monthly rainfall values (in mm) for each month from January (`JAN`) to December (`DEC`)
- `ANNUAL RAINFALL`: Total annual rainfall
- `FLOODS`: Binary indicator (0 or 1) representing whether a flood occurred (1) or not (0)

## Data Preprocessing

- The `SUBDIVISION` column, which contains constant values, was dropped.
- Missing values were filled with zeros.
- The target variable, `FLOODS`, was binarized using LabelBinarizer.

## Exploratory Data Analysis

- Visualized the average monthly rainfall in Kerala using a bar plot.
- Explored the distribution of rainfall across different months.

## Model Training

- Utilized logistic regression for binary classification.
- The dataset was split into training and testing sets.
- The Min-Max scaler was applied to normalize the feature values.
- Trained the logistic regression model on the training set.

## Model Evaluation

- Evaluated the model on the testing set.
- Calculated accuracy, precision, recall, and F1 score metrics.
- Visualized the confusion matrix using a heatmap.

## Results

- **Training Set Accuracy:** 90.43%
- **Testing Set Accuracy:** 87.50%
- **Precision:** 1.00
- **Recall:** 0.79
- **F1 Score:** 0.88
