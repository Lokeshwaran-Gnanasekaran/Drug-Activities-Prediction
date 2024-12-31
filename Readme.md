**Drug Activities Prediction**

**Overview:**

This project aims to predict whether a given compound is active (1) or inactive (0) based on its molecular features. It implements various feature selection and classification methods, addressing the challenges of an imbalanced dataset. The final model achieves an F1 score of 0.68 on the test dataset.

**Goal:**

* Feature selection and dimensionality reduction.  
* Experimentation with different classification models.  
* Addressing imbalanced datasets.  
* Achieving high F1 scores for binary classification.

**Methodology:**

**Data Preprocessing**

* Converted training and test data into sparse matrices.  
* Addressed imbalanced data using oversampling and undersampling techniques.

**Feature Selection**

* Applied chi-squared dimensionality reduction with 300-350 components.

**Model Training**

* Experimented with various classifiers:  
  * Decision Tree (F1 Score: 74%)  
  * Naive Bayes (F1 Score: 60%)  
  * Multi-Layer Perceptron (MLP) Classifier (F1 Score: 84%)  
* Selected the MLP model for final predictions.

**Imbalance Handling**

* Used bucketing to create balanced datasets.  
* Incorporated SMOTE and RandomUnderSampler techniques in a pipeline.

## **Results:**

* Final F1 Score: **0.68**  
* MLP Model Configuration:  
  * Layers: \[64, 32\]  
  * Activation: ReLU  
  * Optimizer: Adam  
  * Regularization (alpha): 0.00001

