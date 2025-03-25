# HR-Analytics
This machine learnign classificaiton notebook aims to predict whether a candidate is looking for a job change (target = 1) based on various attributes from the HR dataset.

Steps Performed in the Notebook:

Importing Necessary Libraries:

numpy, pandas: Data manipulation and analysis.

matplotlib, seaborn, plotly: Data visualization.

scipy: Statistical analysis (normality check, skewness).

sklearn: Data preprocessing, model training, and evaluation.

imblearn: Handling imbalanced data using SMOTE.

pivottablejs: Creating interactive pivot tables.

Loading Data:

Reading the dataset (aug_train.csv) into a DataFrame.

Inspecting missing values.

Exploratory Data Analysis (EDA):

Creating bar plots to check frequency distribution of categorical features with respect to the target variable.

Generating pivot tables to examine relationships between features like education level, experience, gender, company type, and training hours.

Visualizing data distribution using sns.distplot() for training_hours.

Handling Missing Values:

Replacing missing gender values with 'Male' (based on predominant category).

Filling missing enrolled_university entries with 'no_enrollment'.

Filling education_level with mode or forward/backward filling.

Various other handling strategies applied for missing data.

Encoding Categorical Variables:

Using LabelEncoder() for transforming categorical features to numeric representation.

Handling Imbalanced Data:

Applying SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.

Feature Scaling:

Using MinMaxScaler() to scale features before feeding them into the model.

Model Training & Evaluation:

Training a RandomForestClassifier.

Using train_test_split() to split data into training and testing sets.

Applying StratifiedKFold() and RandomizedSearchCV() for hyperparameter tuning.

Evaluating model performance using accuracy_score and classification_report.

Generating Visualizations:

Using Seaborn, Matplotlib, and Plotly to create distribution plots, bar charts, pivot tables, etc.





