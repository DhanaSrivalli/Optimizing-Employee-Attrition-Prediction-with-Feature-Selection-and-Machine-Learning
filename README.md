# Masters Project <a name="mastersproject"></a> 
## Optimizing Employee Attrition Prediction with Feature Selection and Machine Learning

### TABLE OF CONTENTS:
- [Aim of the Project](#aim-of-the-project)
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Preprocessing](#preprocessing)
- [Feature Selection](#feature-selection)
- [Training Models](#training-models)
- [Results](#results)
  
#### Aim of the Project <a name="aim-of-the-project"></a>
This study seeks to investigate the effect of feature selection approaches on the effectiveness of machine learning models for forecasting employee attrition. The study uses L1 regularization and Recursive Feature Elimination (RFE) to find the most relevant elements affecting turnover and improve model accuracy.

#### Project Overview <a name="project-overview"></a>
Project Overview: The project compares the performance of Gradient Boosting, Decision Tree, and Multilayer Perceptron (MLP) models with and without feature selection. Using the IBM HR Analytics Attrition dataset, it compares alternative feature selection strategies, including the union of L1 and RFE, and examines their effect on model efficiency, predictive accuracy, and feature importance in forecasting employee turnover.

#### Dataset <a name="dataset"></a>
This research data was sourced from Kaggle IBM HR Analytics Employee Attrition (Subhash, 2021)
"https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset"

The data collection contains 1,470 records of employee information, with 35 parameters such as age, work satisfaction, performance rating, monthly pay, years with the company, and attrition (staff turnover). The data collection includes both qualitative and numerical characteristics, such as employee details, experience, and remuneration, which can be utilized to build predictive models. Surprisingly, the last column, called "Attrition", is the answer variable that indicates whether or not the employee left. 
Format: CSV
Size: 1,470 records with 35 features, including demographic, professional, and performance-related data.
Target Variable: Attrition (indicates whether an employee left the organization).

#### Features <a name="features"></a>
>* Implements feature selection techniques:
- L1 Regularization (Lasso)
- Recursive Feature Elimination (RFE)
- Union and Intersection of L1 and RFE
>* Machine learning models used:
- Gradient Boosting (GB)
- Extreme Gradient Boosting (XGB)
- Histogram-Based Gradient Boosting (HGB)
- Decision Tree (DT)
- Multi-Layer Perceptron (MLP)
>* Comprehensive evaluation metrics:
Accuracy, Precision, Recall, F1 Score, False Positive Rate (FPR), False Negative Rate (FNR)
Balances imbalanced datasets using SMOTE.

#### Preprocessing <a name="preprocessing"></a>
Cleans the dataset by removing redundant features and handling missing values.
Encodes categorical variables and balances the dataset using SMOTE.

#### Feature Selection <a name="feature-selection"></a>
Applies L1, RFE, Union, and Intersection to identify key features.

#### Training Models <a name="training-models"></a>
Trains GB, XGB, HGB, DT, and MLP on both full and feature-selected datasets.
>*Evaluation:
Compares models using metrics like accuracy, F1 score, and confusion matrices.
>*Visualization:
Visualizes learning curves, performance metrics, and feature importance.

#### Results <a name="results"></a>
>*Best Models:
HGB and XGB: Achieved the highest accuracy of 91% on the original dataset with 32 features.
Feature Selection Observations:
Union of L1 and RFE (29 features) provided the best balance between performance and dimensionality reduction.
Intersection of L1 and RFE (11 features) negatively impacted model accuracy.
>*Key Metrics:
XGB and HGB maintained low FPR and FNR, ensuring high reliability in predicting employee turnover.
