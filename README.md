# Project 4 : Female in the Workplace Analysis: A Machine Learning Approach
Website: 

- Overview: This project aims to analyse and visualise the status and trends related to women in the workplace globally. 

- Objectives: 
1.	Problem Identification: Analyse the current state of women in the workplace, focusing on aspects such as opportunity equity, pay equity, and leadership roles. 
2.	Prediction and Visualization: Use ML models to predict future trends in these areas and visualize the data for easy interpretation and insight generation.

- Data Source: We have used 4 csv files sourced from International Labour Organisation https://ilostat.ilo.org/data/ 

- Technologies and Tools
1.	Machine Learning Libraries: Scikit-learn for model building and predictions.
2.	Python: Pandas for data manipulation; Matplotlib for basic visualizations.
3.	Tableau: Plots for interactive visualizations.
4.	Front-End Development: HTML/CSS for user interface design.
5.	Cloud Services: Amazon AWS for cloud data storage and static website host.

# Part-1 Opportunities Equity Analysis: 1.1 Unemployment Analysis

## Clustering
- K-Means Clustering: Partition countries into groups based on similarities in their unemployment data.

## Classification: classify countries into different categories based on unemployment rates (high, medium, low unemployment), convert the unemployment rate into a categorical variable and use classification algorithms:
- Random Forest Classifier: Classify data points into the defined unemployment categories based on the features.
Note: The choice of bins for categorizing the unemployment rate is subjective and heavily affect the model's performance.

## Model Optimizion： To improve this machine learning model using the following enhancements:
- SMOTE (Synthetic Minority Over-sampling Technique): Balances the dataset if it's imbalanced.
- GridSearchCV: Searches for the best hyperparameters.
- Classification Report and Confusion Matrix: Provides a detailed evaluation of the model's performance.
- Cross-Validation: Provides a more robust estimate of the model's performance.

## Interpretation and Assessment of Performance:
- The model's performance has improved from the first to the second part of the code, with accuracy increasing from 67% to 84%.
- The classification report indicates good precision and recall across all classes, which is further supported by strong F1-scores. This suggests the model is fairly accurate and balanced in predicting each class.
- The confusion matrix reveals some misclassifications, but the majority of predictions are correct, as seen in the high numbers along the diagonal.
- The cross-validation scores indicate a decent but somewhat varying performance across different parts of the dataset.

Overall, the model's performance can be considered good, especially in comparison to the initial model. However, there is always room for further tuning and improvement, particularly in addressing the variability indicated by the cross-validation scores. This could involve further hyperparameter tuning, feature engineering, or even collecting more data if possible.

# 1.2 Employment Analysis 

# 1.3 Salaries per Gender
Investigation into salary disparities based on gender.

The graph aims to predict education skill levels based on the passage of time using a linear regression model.
- Data Preparation:
The dataset is loaded and rows with missing values in the target variable are removed.

-Features and Target Variable:
The feature ('X') is defined as the 'time' column, representing years.
The target variable ('y') is the 'obs_value,' indicating education skill levels.

-Train-Test Split:
The data is split into training and testing sets for model evaluation. A linear regression model is created and trained on the training data.

-Model Evaluation:
A scatter plot displays the actual data points ('Actual Data') and overlays the linear regression predictions ('Linear Regression Prediction').
The x-axis represents the year, and the y-axis represents the observed education skill level.

-Future Predictions:
Predictions are made for future years (2021 to 2030) using the trained model.
