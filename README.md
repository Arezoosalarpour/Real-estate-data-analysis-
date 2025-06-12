Real Estate Data Analysis Project


## Introduction

This project focuses on analyzing housing data from California to explore the key factors influencing real estate prices. Through a comprehensive data science workflow—ranging from initial exploration to preprocessing, visualization, and advanced statistical analysis—we aim to uncover trends and patterns in the housing market.

This project is intended for educational and research purposes and demonstrates core data analysis and preprocessing techniques in Python.

## Dataset Information

This project uses the **California Housing** dataset, which is available through the `scikit-learn`.
- Source: [Scikit-learn California Housing Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)  
- Original Source: UCI Machine Learning Repository  
- License: Public domain (educational/research use)

## Stage 1: Data Exploration

### 1.1 General Data Structure Review
• Load the dataset and display general information  
• Check data dimensions (number of rows and columns)  
• Identify variable types (numerical, categorical, text)  
• Show sample records (first and last rows)  

### 1.2 Descriptive Statistical Analysis
• Calculate central statistics (mean, median, mode)  
• Calculate dispersion statistics (standard deviation, range, interquartile range)  
• Check skewness and kurtosis of variable distributions  
• Identify minimum and maximum values for each variable  

### 1.3 Target Variable Analysis
• Examine the distribution of property prices  
• Identify price ranges  
• Analyze normality of the target variable distribution  
• Check for outliers or unusual prices  

---

## Stage 2: Data Preprocessing

### 2.1 Missing Values Management
• Identify and count missing values per column  
• Analyze missing data patterns  
• Implement different imputation methods:  
  - Remove incomplete records  
  - Fill with mean/median/mode  
  - KNN imputation  
  - Regression imputation  
• Compare the performance of different methods  

### 2.2 Outlier Detection and Management
• Detect outliers using IQR method  
• Detect outliers using Z-Score method  
• Detect outliers using Isolation Forest  
• Decide whether to keep or remove outliers  
• Examine the impact of outliers on model performance  

### 2.3 Data Transformation and Normalization
• Apply mathematical transformations (log, square root, power)  
• Standardize data (StandardScaler)  
• Normalize data (MinMaxScaler)  
• Use robust scaling (RobustScaler)  
• Compare different normalization methods  

### 2.4 Feature Engineering
• Create ratio features (e.g., rooms per person)  
• Combine existing features to create new ones  
• Bin continuous variables  
• Create dummy variables for categorical data  
• Extract features from date variables (if any)  

### 2.5 Feature Selection
• Remove low variance features  
• Select features based on correlation  
• Use filter methods (Chi-square, ANOVA)  
• Use wrapper methods (RFE)  
• Use embedded methods (Lasso, Ridge)  

---

## Stage 3: Data Visualization

### 3.1 Univariate Visualizations
• Histogram for numerical variables  
• Box Plot to identify outliers  
• Density Plot to examine distributions  
• Bar Chart for categorical variables  
• Pie Chart for proportions  

### 3.2 Bivariate Visualizations
• Scatter Plot between features and target variable  
• Correlation Heatmap  
• Grouped Box Plot  
• Line Chart for trends  
• Violin Plot for group distributions  

### 3.3 Multivariate Visualizations
• Pair Plot matrix  
• Parallel Coordinates Plot  
• 3D Scatter Plot  
• Advanced Heatmap with clustering  
• Principal Component Analysis (PCA) plot  

### 3.4 Geographic and Spatial Visualizations
• Geographic scatter plot of prices  
• Geographic heatmap  
• Spatial cluster analysis  
• Density plot of points  
• Visualization of regional trends  

---

## Stage 4: Advanced Analysis

### 4.1 Advanced Correlation Analysis
• Calculate various correlations (Pearson, Spearman, Kendall)  
• Detect multicollinearity (VIF)  
• Partial correlation analysis  
• Identify nonlinear relationships  

### 4.2 Distribution Analysis and Statistical Tests
• Normality tests (Shapiro-Wilk, Kolmogorov-Smirnov)  
• Homogeneity of variance tests  
• Group comparison tests (t-test, ANOVA)  
• Residual distribution analysis  

### 4.3 Feature Importance Analysis
• Calculate feature importance using Random Forest  
• Sensitivity analysis of variables  
• Feature ranking  
• Interaction effect analysis  

---

## Stage 5: Preparation for Modeling

### 5.1 Data Splitting
• Split data into training, validation, and test sets  
• Apply stratified splitting  
• Ensure no data leakage  
• Create cross-validation folds  

### 5.2 Preprocessing Pipeline
• Build a complete preprocessing pipeline  
• Save and load the pipeline  
• Validate the pipeline  
• Document the steps  

### 5.3 Final Data Quality Checks
• Final check for missing values  
• Final outlier control  
• Validate value ranges  
• Check class balance (if applicable)  
