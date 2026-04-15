# DATA 22100 – Introduction to Machine Learning
## Final Project: Political Instability Analysis

**University of Chicago**  
**Instructors:** David Biron, Amy Nussbaum  
**Term:** Spring 2024  

**Team Members:**   
- Aren Mizuno
- Ryan Winston   

---

## Overview

This repository contains my final project for *DATA 22100: Introduction to Machine Learning*, a course focused on foundational machine learning methods and their real-world applications.

The course introduced key topics in modern machine learning, including supervised and unsupervised learning, regression and classification, loss functions, empirical risk and overfitting, clustering, and ensemble methods such as decision trees, random forests, and gradient boosting. Students developed an understanding of model evaluation and selection, with exposure to neural networks and deep learning concepts.

---

## Final Project

**Description:**  
This project analyzes and predicts a constructed **political instability index** using economic, demographic, and social variables. The goal is to identify key drivers of instability and evaluate the performance of different machine learning models in capturing these relationships.

The instability index is defined as the log-scaled ratio of fatalities to population (using moving averages), allowing for consistent comparison across time.

---

### Methodology

- Performed **data wrangling and preprocessing**:
  - Interpolated missing yearly data using linear interpolation  
  - Aggregated and cleaned multiple datasets  
  - Constructed a unified dataset across time  
  - Engineered a political instability index using fatalities and population data  

- Conducted **exploratory data analysis (EDA)**:
  - Analyzed distributions and skewness of variables  
  - Identified weak and moderate correlations between predictors  
  - Found stronger relationships with life expectancy  

- Built and compared multiple **regression models**:
  - Linear Regression  
  - LASSO and Ridge Regression  
  - Decision Tree Regression  
  - Random Forest Regression  

- Applied **model selection and validation techniques**:
  - 70/30 train-test split  
  - 10-fold cross-validation for hyperparameter tuning  
  - Evaluation using MSE, MAE, and R²  

- Implemented **dimensionality reduction and clustering**:
  - Principal Component Analysis (PCA)  
  - Reduced to 2 components (~90% variance explained)  
  - K-means clustering with optimal k=4 (based on elbow method and silhouette score)  

---

### Key Findings

- The **Random Forest Regressor** performed best, capturing nonlinear relationships and reducing overfitting  

- Most influential predictors included:
  - Life expectancy  
  - Polarization  
  - Economic vulnerability indicators  

- PCA reduced dimensionality effectively while maintaining strong predictive performance  

- Clustering analysis revealed **distinct groups of political instability levels**, with statistically significant differences between clusters  

---

### Project Deliverables

- `ML Final Project.ipynb`  
  → Full analysis including data preprocessing, modeling, and clustering  

- `Final Project.docx`  
  → Written report with methodology, results, and interpretation  

---

## Skills & Concepts Demonstrated

- Supervised learning: regression models  
- Unsupervised learning: clustering (K-means)  
- Dimensionality reduction (PCA)  
- Feature engineering and data interpolation  
- Model evaluation (MSE, MAE, R²)  
- Cross-validation and hyperparameter tuning  
- Decision trees and random forests  
- Understanding overfitting and model risk  
- Interpreting machine learning results in applied contexts  

---

## Final Takeaway

This project demonstrates how combining **data preprocessing, machine learning models, and statistical evaluation** can uncover meaningful patterns in complex societal data.

It highlights the importance of model selection, validation, and interpretability when applying machine learning techniques to real-world problems.
