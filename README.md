# Wine Quality Analysis

## Description
This repository contains a complete analysis of a wine quality dataset using various machine learning and statistical models. The dataset is sourced from the UCI Machine Learning Repository and includes both red and white wines. The analysis focuses on data cleaning, exploratory data analysis (EDA), regression models, and classification models to predict the quality of wine based on its features. The repository also demonstrates model evaluation techniques, such as ROC curve comparison and feature importance.

### Key Features:
- Data Cleaning: Handling missing values, removing duplicates, and outlier detection.
- Data Transformation: Normalizing numeric columns using Min-Max Scaling.
- Exploratory Data Analysis: Histograms, bar plots, and correlation matrix.
- Regression Analysis: Linear and multiple linear regression models.
- Classification Analysis: Logistic regression, random forest, and K-nearest neighbors (KNN) for binary classification.
- Model Evaluation: ROC curve comparison for logistic regression and random forest models, along with feature importance analysis.
- Data Saving: Saving cleaned and preprocessed data for future use.

## Dataset
The dataset consists of two parts:
- **Red Wine**: Data related to red wine features.
- **White Wine**: Data related to white wine features.

Both datasets are combined into a single dataset and used for analysis. Each wine sample contains several features like alcohol content, pH, sulphates, density, and quality score.

## Data Preprocessing
- **Missing Values**: Missing values are filled with the median of the respective columns.
- **Duplicates**: Duplicate rows are removed.
- **Outliers**: Outliers are removed using the Interquartile Range (IQR) method.
- **Normalization**: Numeric columns are normalized using Min-Max scaling to bring all features into the range [0, 1].

## Exploratory Data Analysis (EDA)
- **Histograms**: Visualizations of alcohol content, density, and pH for both red and white wines.
- **Correlation Matrix**: A heatmap to visualize the relationships between different features.

## Model Building
1. **Linear Regression**: Predicting wine quality using a simple linear regression model.
2. **Multiple Linear Regression**: Using multiple features (alcohol, pH, and sulphates) to predict wine quality.
3. **Logistic Regression**: Converting wine quality into a binary classification (high vs. low quality) and building a logistic regression model.
4. **Random Forest**: A random forest model is built to predict wine quality, and feature importance is evaluated.
5. **K-Nearest Neighbors (KNN)**: A classification model to predict wine quality.

## Model Evaluation
- **ROC Curve**: The ROC curve is plotted to compare the performance of logistic regression and random forest models.
- **Confusion Matrix**: Used to evaluate the performance of the KNN model.

## Feature Importance
- The importance of each feature is evaluated using the random forest model.

You can install these packages by running the following command:

```r
install.packages(c("tidyverse", "pROC", "caret", "randomForest", "class", "ggcorrplot", "ucimlrepo"))
