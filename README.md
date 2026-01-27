# wine_quality_prediction
Wine Quality Prediction — Machine Learning Project

This project is part of my internship work, where I built an end-to-end Machine Learning system to predict wine quality based on chemical properties. The main goal was to understand the complete ML workflow — from data analysis to model evaluation and optimization.
---
Project Objective

The objective of this project is to analyze wine data and build models that can predict whether a wine is good or bad based on its chemical features.
This project helped me learn how real-world Machine Learning systems are designed and improved.
---
Dataset Overview

File used: winequality.csv
Each row represents one wine sample
Each column represents a chemical property (like acidity, sugar, alcohol, etc.)
The target column is quality, which indicates the wine’s quality score
To make the problem more practical, I converted it into a binary classification task:
Quality ≥ 7 → Good Wine (1)
Quality < 7 → Bad Wine (0)
---
Steps Followed in This Project

1. Data Loading & Understanding
I loaded the dataset using Pandas and explored it using functions like head(), tail(), and sample() to understand the structure and type of data.
What I learned: Each row represents one wine, and all columns contain numerical chemical measurements.
---
2. Basic Data Inspection
I checked:
Column names
Data types
Number of rows and columns
Summary statistics using describe()
Why this step matters: It helps identify unusual values, understand data distribution, and prepare the dataset before modeling.
---
3. Missing Values Analysis
I checked for missing values using isnull() and found no missing data in the dataset.
If missing values existed, I would handle them using imputation or removal depending on the situation.
---
4. Exploratory Data Analysis (EDA)
I analyzed the distribution of wine quality scores and created a count plot.
Key observations:
Most wines fall into medium quality categories
The dataset is slightly imbalanced
Very high and very low quality wines are rare
EDA helped me understand:
How quality scores are distributed
Whether the dataset has bias
What to expect before training models
---
6. Converting to a Classification Problem
I created a new column called quality_label to convert quality scores into two categories: good and bad.
Reason: Binary classification is more practical in real-world applications than predicting exact quality scores.
---
6. Feature & Target Separation
Features (X): Chemical properties
Target (y): quality_label
I excluded the original quality column to avoid data leakage.
---
7. Train-Test Split
I split the dataset into:
80% training data
20% testing data
This ensures the model is evaluated on unseen data, which reflects real-world performance.

---
8. Feature Scaling
I applied StandardScaler to normalize feature values.
Scaling is important for models like:
Logistic Regression
KNN
Support Vector Machine (SVM)
---
9. Model Training
I trained and tested the following models:
Logistic Regression
K-Nearest Neighbors (KNN)
Decision Tree
Random Forest
Support Vector Machine (SVM)
Each model was tested to compare performance and understand its strengths.
---
10. Model Evaluation & Comparison
I evaluated all models using accuracy and created a comparison table.
Best performing model: Random Forest performed the best because it handles non-linear relationships well and reduces overfitting.
---
11. Pipeline & Hyperparameter Tuning
I built a Machine Learning pipeline using scaling and model training together.
Then I applied GridSearchCV to tune parameters such as:
Regularization strength (C)
Kernel type (for SVM)
This helped improve model accuracy and reliability.

---
What I Learned from This Project
How to structure a complete Machine Learning project
The importance of EDA before training models
How feature scaling affects performance
How to compare multiple ML models
How pipelines improve workflow efficiency
How hyperparameter tuning improves accuracy
How ML projects relate to real-world decision-making

---
Final Conclusion

This project helped me understand the full Machine Learning lifecycle — from raw data to optimized models. It improved my confidence in building practical ML solutions and strengthened my understanding of real-world modeling techniques.
