## Data Analysis - Logistics Dataset - Classification

Author: Amanpreet Kaur
Date: December 09, 2022

### Project Overview
This project analyzes a logistics dataset using data preparation, exploratory analysis, and model development techniques. The dataset contains variables related to delivery, packages, customer orders, distance, domestic/international indicators, hazardous products, and carrier services.

### Dataset
The dataset includes the following variables:
- Dom: Domestic/International indicator
- Haz: Hazardous product indicator
- Car: Carrier service indicator
- Del: Delivery time
- Vin: Vintage time
- Pkg: Number of packages
- Cst: Customer order history
- Mil: Distance for delivery

### Project Structure
The project is divided into two parts:

### Part A - Data Preparation and Exploration
- Preliminary Data Preparation:
  - Reading the dataset and modifying variable names.
  - Statistical description of variables.
  - Converting categorical variables to factor variables.
  - Data visualization using histograms, box plots, and density plots to understand variable distributions and identify outliers.
- Exploratory Analysis:
  - Computing a new variable OT_AK (On-Time Delivery) based on delivery time.
  - Calculating numerical correlations and graphical correlation matrix.
  - Performing Chi-Squared test to identify significant predictors for On-Time Delivery.
- Model Development:
  - Developing a logistic regression model (full model and backward model) to predict On-Time Delivery.
  - Analyzing model performance based on AIC, deviance, residual symmetry, z-values, and parameter coefficients.

### Part B - Model Comparison
- Logistic Regression – Backward:
  - Implementing logistic regression with backward elimination for feature selection.
  - Evaluating model performance using confusion matrix and accuracy calculation.
- Naive-Bayes Classification:
  - Implementing Naive-Bayes classification to predict On-Time Delivery.
  - Evaluating model performance using a confusion matrix.
- Linear Discriminant Analysis:
  - Implementing Linear Discriminant Analysis (LDA) for classification.
  - Evaluating model performance using a confusion matrix.
- Decision Tree:
  - Building a decision tree classifier for predicting On-Time Delivery.
  - Visualizing the decision tree.
- Comparative Analysis:
  - Comparing the accuracy of all classifiers to identify the best-performing model.

### Results
- Logistic Regression: 85.59% accuracy, processing time 0.95 secs, 432 false positives.
- Naive-Bayes: 85.02% accuracy, processing time 0.02 secs, 443 false positives.
- Linear Discriminant Analysis: 85.64% accuracy, processing time 0.05 secs, 440 false positives.
- Decision Tree: 85.67% accuracy, processing time 0.38 secs, 403 false positives.

### Conclusion
- The decision tree classifier performs best in terms of accuracy and false positives. 
- Naive-Bayes is the fastest in processing speed but has lower accuracy.
Choose based on priorities: accuracy, processing speed, or minimizing false positives.

### Files Included
- Data Analysis - Logistics Dataset.txt: The original dataset.
- Data Analysis - Classification.Rmd: R script containing the code for data analysis.
- Data-Analysis---Classification.pdf: Output file containing visualizations and model summaries.
