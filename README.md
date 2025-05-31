# Milestone-Assignment-2-Principal-Component-Analysis
This project demonstrates how Principal Component Analysis (PCA) can identify essential variables in breast cancer data, enabling dimensionality reduction for more efficient modeling. The analysis includes an optional logistic regression component for prediction.

Requirements
Python 3.7+
Jupyter Notebook
Required Python packages: numpy, pandas, matplotlib, seaborn, scikit-learn

Installation
1. Clone the repository
2. Install the required packages
3. Launch the Jupyter Notebook file

Files:
Milestone Assignment 2 Principal Component Analysis.ipynb
README

Instructions
1. Loaded the breast cancer dataset from sklearn.datasets.
2. Created a pandas DataFrame for exploration.
3. Separated features and target variable.
4. Standardized features using StandardScaler by ensuring all features contribute equally to PCA
5. Performed PCA to reduce the dataset to 2 principal components.
6. Calculated explained variance for each component
7. Split data into training/testing sets (80/20)
8. 2D visualization of PCA results.
9. Identified top features contributing to each principal component
10. Optional logistic regression model - by comparing full-feature model vs PCA-reduced model, visualize decision boundary in PCA space and generated performance metrics (such as accuracy and confusion matrix)

Results
PCA Components:
PC1 explains 44.3% of variance
PC2 explains 18.9% of variance
Combined 63.2% of total variance

Key Variables:
PC1: Strongly correlated with mean radius, perimeter, area
PC2: Primarily associated with texture and smoothness

Visual Separation:
Malignant and benign cases show clear separation in 2D PCA space

Optional: Logistic Regression
1. Implement logistic regression for prediction.
2. Display the logistic regression results.

Key Insight: The PCA model achieves 94.74% accuracy using just 2 components, demonstrating effective dimensionality reduction while maintaining predictive power.

Expected Output
1. PCA Visualization (pca_visualization.png): Scatter plot showing separation of malignant/benign cases in PCA space
2. Feature Importance: Shows top 5 features for each principal component and which cancer characteristics are most significant
3. Model Performance Comparison: Accuracy scores for both models, Confusion matrix for PCA model and Classification report with precision/recall metrics
4. Decision Boundary Visualization (decision_boundary.png): Shows how logistic regression separates classes in PCA space
