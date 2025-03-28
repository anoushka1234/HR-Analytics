# HR-Analytics
This machine learnign classificaiton notebook aims to predict whether a candidate is looking for a job change (target = 1) based on various attributes from the HR dataset.

Steps I took were the following:

1.Imported necessary libraries: 
-  numpy, pandas: Data manipulation and analysis.
-  matplotlib, seaborn, plotly: Data visualization.
-  scipy: Statistical analysis (normality check, skewness).
-  sklearn: Data preprocessing, model training, and evaluation.
-  imblearn: Handling imbalanced data using SMOTE.
-  pivottablejs: Creating interactive pivot tables.

2.Loading Data:
- Reading the dataset (aug_train.csv) into a DataFrame.
- Inspecting missing values.

3.Exploratory Data Analysis (EDA):
- Creating bar plots to check frequency distribution of categorical features with respect to the target variable.
- Generating pivot tables to examine relationships between features like education level, experience, gender, company type, and training hours.
- Visualizing data distribution using sns.distplot() for training_hours.
- Treated missed typos and cleaned the outliers of the dataset for better analysis

4.Handling Missing Values:
- Replacing missing gender values with 'Male' (based on predominant category).
- Filling missing enrolled_university entries with 'no_enrollment'.
- Filling education_level with mode or forward/backward filling.
- Various other handling strategies applied for missing data.

5.Encoding Categorical variables:
- Using LabelEncoder() for transforming categorical features to numeric representation as well Ordinal Encoding for some of the ordered columns

6.Handling Imbalanced Data:
- Applying SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.

7.Feature Scaling:
- Applying SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.

8.Model Training and Evaluation:
- Training a Random Forest Classifier, Logistic Regression,Gaussian Naive Bayes,K Nearest Neighbors Classifier,Decision Tree Classifier,Support Vector Classifier, Gradient Boosting Classifier, XG Boosting Classifier. 
-  Using train_test_split() to split data into training and testing sets.
- Applying StratifiedKFold() and RandomizedSearchCV() for hyperparameter tuning.
- Evaluating model performance using accuracy_score and classification_report --> found RandomForrest to be best model with minimal overfitting and the most contirbuting features are: city_development_index,training_hours,experience.

9.Generating Visualizations:
- Using Seaborn, Matplotlib, and Plotly to create distribution plots, bar charts, pivot tables, pairplots, treamaps, sunburst, pointplot,histogram, joinplot,catplot, piechart, subplot,bubblechart etc.



