# Project 4 : Female in the Workplace Analysis: A Machine Learning Approach

**Check out our project outputs by visiting our Project4 Page: https://lxproject4.s3.ap-southeast-2.amazonaws.com/project-4/index.html**

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

# Part-1 Opportunities Equity Analysis: 
# 1.1 Unemployment Analysis

## Preprocessing

## Clustering
- K-Means Clustering: Partition countries into groups based on similarities in their unemployment data.

## Classification: classify countries into different categories based on unemployment rates (high, medium, low unemployment), convert the unemployment rate into a categorical variable and use classification algorithms:
- Random Forest Classifier: Classify data points into the defined unemployment categories based on the features.
Note: The choice of bins for categorising the unemployment rate is subjective and heavily affect the model's performance (If have more time, will try more bins). 

## Model Optimizion： To improve this machine learning model using the following enhancements:
- SMOTE (Synthetic Minority Over-sampling Technique): Balances the dataset if it's imbalanced.
- GridSearchCV: Searches for the best hyperparameters.
- Classification Report and Confusion Matrix: Provides a detailed evaluation of the model's performance.
- Cross-Validation: Provides a more robust estimate of the model's performance.

## Interpretation and Assessment of Performance:
- The model's performance has improved, with accuracy increasing from 67% to 85%.
- The classification report indicates good precision and recall across all classes, which is further supported by strong F1-scores. This suggests the model is fairly accurate and balanced in predicting each class.
- The confusion matrix reveals some misclassifications, but the majority of predictions are correct, as seen in the high numbers along the diagonal.
- The cross-validation scores indicate a decent but somewhat varying performance across different parts of the dataset.

Overall, the model's performance can be considered good, especially in comparison to the initial model. However, there is always room for further tuning and improvement, particularly in addressing the variability indicated by the cross-validation scores. This could involve further hyperparameter tuning, feature engineering, or even collecting more data if possible.

# 1.2 Employment Analysis 

## Preprocessing
- Dropping unused columns & rows 
- Handling Categorical Variables: Categorical variables such as country, education level, and marital status are processed using OneHotEncoder.

## Building and Evaluating a Linear Regression Model
- The poor performance indicates that this algorithm does not suit the dataset well.

## Implementing an optimal model : Random Forest Regressor
- Achieve better scores by implementing the Random Forest Regressor, and also obtain the top 10 feature importances that influence the model's prediction ability.

Feature importance:
1. Model Interpretability: It helps in understanding the model's decision-making process. Knowing which features significantly influence the model's predictions can provide insights into the underlying data and the problem being solved.
2. Model Simplification: By identifying the most important features, one can simplify the model by removing less important features. This can lead to a reduction in model complexity, faster training times, and sometimes improved model performance.
3. Feature Engineering: Understanding which features are important can guide further feature engineering. It can reveal if additional data collection or generation of new features could improve the model.
4. Data Reduction: For datasets with a large number of features, feature importance can be used to reduce the dimensionality of the data. This is particularly useful in cases where data collection or storage is expensive.

# To do: 
- Seek additional datasets that include other features, particularly economic ones, as these can have a significant impact on employment.
- Create a database. 
- Upgrade the webpage to be interactive. 