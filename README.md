# Project_Valuation_Anaysis
For the Analysis and model prediction I have used this Dataset
https://drive.google.com/file/d/1Ybgvs_UMaC6400mNGgGVqIuGSMXa-Tw_/view

## Project Name. Project Valuation Analysis 

# 2.1. Dataset Overview
•	Source: unicorns till sep 2022.csv
•	Size: Contains data on various unicorn companies.

Key Features:
•	company: Name of the company\n
•	valuation_($b): Valuation in billions
•	country: Country of the company
•	date_joined: Date when the company became a unicorn

# 2.2. Data Cleaning and Preprocessing
•	Renamed columns for consistency.
•	Converted valuation_($b) to float after removing the dollar sign.
•	Extracted year and month from the date_joined column.

# 2.3. Exploratory Data Analysis (EDA)
•	Visualized the distribution of company valuations.
•	Identified top companies by valuation and plotted a bar chart.
•	Analyzed the distribution of unicorns by country using a pie chart.
•	Tabular Analysis: A detailed table was created to summarize the count of companies by country, year, month, and industry.

# 2.4. Model Development
•	Features and Target Variable:
•	Features: All columns except valuation_($b) and company
•	Target: valuation_($b)	
•	Model Selection: Linear Regression and Random Forest Regressor were used.
•	Data Preprocessing: Implemented a pipeline for handling missing values, scaling, and encoding categorical features.

# 2.5. Results
•	Evaluated both models using MSE and R².
•	Linear Regression:
•	MSE for Linear Regression: 28.17
•	R2 for Linear Regression: -2.21
•	Random Forest:
•	MSE for Random Forest Regressor: 15.53
•	R² for Random Forest Regressor: -0.77
•	Conducted hyperparameter tuning for the Random Forest model using GridSearchCV. 
•	Reported the best parameters and scores from the tuning process.
•	Best Parameters: {'model__max_depth': 10, 'model__min_samples_split': 5, 'model__n_estimators': 100}
•	 Best Score: 0.018757365706072893
•	Optimized Random Forest:
•	MSE: 14.66
•	R2:  -0.67

