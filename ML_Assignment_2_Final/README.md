
# Machine Learning Assignment 2
## Classification Model Comparison

### 1. Problem Statement

The objective of this assignment is to implement and
compare five machine learning classification models
using the Adult Income dataset.

The objective is to predict whether an individual's
income is greater than $50K annually.

### 2. Dataset Description

- Dataset: Adult Income Dataset
- Source: UCI Machine Learning Repository
- URL: https://archive.ics.uci.edu/dataset/2/adult
- Problem Type: Binary Classification
- Input Features: 14
- Target Variable: income
- Final Number of Instances: 32537

The dataset contains numerical and categorical features.
Missing values and class imbalance were examined.

### 3. GitHub Repository Link

(https://github.com/souritri2026ct/ML-ASSIGNMENT2_Souritri/tree/main/ML_Assignment_2_Final)

### 4. Models Used

The five implemented models are:

1. Logistic Regression
2. Decision Tree Classifier
3. K-Nearest Neighbors
4. Gaussian Naive Bayes
5. Random Forest Classifier

#### Data Preprocessing

- Duplicate records removed.
- Missing numerical values handled using median imputation.
- Missing categorical values handled using mode imputation.
- Categorical features encoded using One-Hot Encoding.
- Numerical features scaled using StandardScaler.
- Train-test split: 80:20.
- Stratified sampling used.
- Random state: 42.

#### Model Configurations

- Logistic Regression: max_iter=2000
- Decision Tree: random_state=42
- KNN: n_neighbors=5
- Gaussian Naive Bayes: default parameters
- Random Forest: n_estimators=100, random_state=42

#### Model Comparison Table

| Model               |   Accuracy |    AUC |   Precision |   Recall |     F1 |    MCC |
|:--------------------|-----------:|-------:|------------:|---------:|-------:|-------:|
| Logistic Regression |     0.8569 | 0.9099 |      0.7437 |   0.6199 | 0.6762 | 0.5893 |
| Decision Tree       |     0.8207 | 0.7539 |      0.6286 |   0.625  | 0.6268 | 0.5088 |
| KNN                 |     0.8379 | 0.8653 |      0.6778 |   0.6237 | 0.6496 | 0.5452 |
| Naive Bayes         |     0.5361 | 0.7492 |      0.3369 |   0.956  | 0.4983 | 0.33   |
| Random Forest       |     0.8605 | 0.9083 |      0.7444 |   0.6409 | 0.6888 | 0.6023 |

#### Graph Representation

See the plots folder for:

- Class distribution
- Missing-value visualization
- Six-metric model comparison
- Confusion matrices

#### Model Performance Observations

Write your interpretation of the actual results for
each of the five models here.

#### Overall Winner

The model with the highest MCC is:

**Random Forest**

MCC: 0.6023

The overall winner is selected based on MCC, while
considering the other evaluation metrics.

### 5. Execution Instructions

Install dependencies:

    pip install -r requirements.txt

Open the notebook:

    jupyter notebook ML_Assignment2_2026ct05159 (1).ipynb

Execute all notebook cells in order.Ipynb file is available under notebooks folder.

The project generates:
- results.csv
- test_data.csv
- Five trained model files
- Performance graphs
