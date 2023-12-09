# Predictive Maintenance Classification Documentation

## Overview

This documentation outlines a machine learning project focused on predictive maintenance classification. The project utilizes a synthetic dataset that mimics real-world scenarios in the industry, containing 10,000 data points with 14 features. These features include information about air temperature, process temperature, rotational speed, torque, tool wear, and machine failure indicators.

## Dataset Details

- **Unique Identifier (UID):** Ranges from 1 to 10,000.
- **Product ID:** Variants L (50%), M (30%), and H (20%) with specific serial numbers.
- **Features:**
  - Air Temperature [K]
  - Process Temperature [K]
  - Rotational Speed [rpm]
  - Torque [Nm]
  - Tool Wear [min]
- **Targets:**
  - Failure or Not
  - Failure Type: Tool wear failure, heat dissipation failure, power failure, overstrain failure, random failures.

## Acknowledgements

The dataset is sourced from the UCI Predictive Maintenance Dataset.

## Data Exploration

### Dataset Characteristics

- **Shape:** (10000, 14)
- **Columns:**
  - UDI, Product ID, Type, Air temperature [K], Process temperature [K], Rotational speed [rpm], Torque [Nm], Tool wear [min], Machine failure, TWF, HDF, PWF, OSF, RNF.

### Statistical Summary of the Dataset

- Descriptive statistics for numerical features.

### Data Types and Null Values

- Information about data types and null values.

## Data Visualization

- Visualizations include histograms of numerical features, a bar chart showing the count of each failure type, and a heatmap of the correlation matrix.

## Data Preprocessing

- Handling categorical features using one-hot encoding.
- Train-test split.
- Feature scaling using StandardScaler.

## Machine Learning Models

### Logistic Regression

#### Model Details

- **Algorithm:** Logistic Regression
- **Training Set:** 80% of the dataset
- **Testing Set:** 20% of the dataset
- **Evaluation Metrics:**
  - Confusion Matrix
  - Classification Report
- **Results:**
  - Accuracy: 97%
  - Precision (class 1): 0.63
  - Recall (class 1): 0.28

### Decision Tree Classifier

#### Model Details

- **Algorithm:** Decision Tree Classifier
- **Training Set:** 80% of the dataset
- **Testing Set:** 20% of the dataset
- **Evaluation Metrics:**
  - Confusion Matrix
  - Classification Report
- **Results:**
  - Accuracy: 98%
  - Precision (class 1): 0.69
  - Recall (class 1): 0.67

### Random Forest Classifier

#### Model Details

- **Algorithm:** Random Forest Classifier
- **Training Set:** 80% of the dataset
- **Testing Set:** 20% of the dataset
- **Evaluation Metrics:**
  - Confusion Matrix
  - Classification Report
- **Results:**
  - Accuracy: 97%
  - Precision (class 1): 0.79
  - Recall (class 1): 0.18

### TensorFlow Model

#### Model Details

- **Algorithm:** Neural Network using TensorFlow
- **Architecture:**
  - Input Layer with 64 neurons and ReLU activation
  - Output Layer with 1 neuron and Sigmoid activation
- **Training Set:** 80% of the dataset
- **Testing Set:** 20% of the dataset
- **Training Parameters:**
  - Epochs: 10
  - Batch Size: 32
- **Evaluation Metrics:**
  - Confusion Matrix
  - Classification Report
- **Results:**
  - Accuracy: 97%
  - Precision (class 1): 1.00
  - Recall (class 1): 0.02

### Support Vector Machine (SVM) Classifier

#### Model Details

- **Algorithm:** Support Vector Machine (SVM) Classifier with a linear kernel
- **Training Set:** 80% of the dataset
- **Testing Set:** 20% of the dataset
- **Evaluation Metrics:**
  - Confusion Matrix
  - Classification Report
- **Results:**
  - Accuracy: 97%
  - Precision (class 1): 0.64
  - Recall (class 1): 0.26

### Gradient Boosting Classifier

#### Model Details

- **Algorithm:** Gradient Boosting Classifier
- **Training Set:** 80% of the dataset
- **Testing Set:** 20% of the dataset
- **Hyperparameters:**
  - Number of Estimators: 100
- **Evaluation Metrics:**
  - Confusion Matrix
  - Classification Report
- **Results:**
  - Accuracy: 98%
  - Precision (class 1): 0.83
  - Recall (class 1): 0.49

## Conclusion

- Summarizing the results and comparing the performance of different models.
