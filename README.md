Exploring the Decision Tree Classifier
Overview
This project explores the fundamentals of Decision Tree Classifiers using the Car Evaluation Dataset from the UCI Machine Learning Repository. The notebook demonstrates building, evaluating, visualizing, and optimizing a Decision Tree model for multi-class classification, predicting car acceptability based on attributes like buying price, maintenance cost, doors, persons, luggage boot size, and estimated safety.
Key concepts covered:

Decision Tree Structure: Root nodes, splitting, leaf nodes, and Gini Impurity for measuring node purity.
Model Training and Evaluation: Accuracy, precision, and recall metrics.
Visualization: Plotting the tree structure.
Feature Engineering: Creating a derived feature (owner_miser) to capture specific decision paths.
Hyperparameter Tuning: Using GridSearchCV to optimize max_depth for better generalization.

The project achieves a test accuracy of 97% after optimization, highlighting the effectiveness of Decision Trees for interpretable, non-parametric classification.
Objectives

Understand Decision Tree mechanics and impurity measures (Gini Impurity).
Preprocess categorical data using Label Encoding.
Train and evaluate a baseline Decision Tree model.
Perform feature engineering to improve model performance.
Optimize hyperparameters via cross-validation.
Visualize the tree to interpret decision boundaries.

Dataset

Source: UCI Car Evaluation Dataset
Description: 1,728 instances with 6 categorical features:

buying: Buying price (vhigh, high, med, low)
maint: Maintenance cost (vhigh, high, med, low)
doors: Number of doors (2, 3, 4, 5more)
persons: Capacity (2, 4, more)
lug_boot: Luggage boot size (small, med, big)
safety: Estimated safety (low, med, high)


Target (class): Acceptability (unacc, acc, good, vgood) – multi-class labels.
File: car.data (CSV-like format; loaded via pandas).

No missing values; all features are nominal.
Dependencies
This project uses Python 3.x and the following libraries:

pandas (data manipulation)
numpy (numerical operations)
scikit-learn (modeling, preprocessing, evaluation, GridSearchCV)
matplotlib (visualization)
seaborn (optional for plots, not heavily used)
