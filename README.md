Codetech internship
Name: J STANES JENSON
Company: CODTECH IT SOLUTIONS.
1D: CT08DS7325
Domain: Data Science
Duration: Auguest to September 2024
Mentor: SRAVANI GOUNI
Overview of the Project

TASK-1
@ Project: Exploratory Data Analysis (EDA) 
This project focuses on Exploratory Data Analysis (EDA) using a dataset loaded from Google Colab. The dataset contains various employee-related data such as salary, experience, team, and incentives. EDA is performed to understand the structure, distribution, and relationships within the dataset. The steps outlined in the project cover data cleaning, transformation, statistical analysis, and visualizations.

Key Objectives:
Loading and Previewing Data:
The dataset is loaded using pandas, and an initial inspection is done by displaying the first few rows of the dataframe.

Data Cleaning:
Removing Irrelevant Columns: The Senior Management column is removed since it’s irrelevant for the analysis.
Handling Duplicate Rows: Duplicate entries are removed to ensure data quality and consistency.
Renaming Columns: The Bonus column is renamed to Incentive to provide more clarity.
Handling Missing Data: Missing values in the dataset are removed using dropna(). Alternatively, the NaN values in the 'Salary' column are filled with the mean salary to retain more data.

Statistical Analysis:
Central Tendency (Experience): The mean, median, and mode of the Experience column are calculated to understand the distribution.
Variability Measures: Variance, standard deviation, interquartile range (IQR), and quantiles are calculated for the Experience column to measure the spread of the data.
Z-score Calculation: The z-scores are computed for Experience to detect outliers based on standard deviations from the mean.
Data Visualization:

Boxplots: Boxplots are used to detect outliers in the Experience column.
Correlation Heatmap: A heatmap is plotted to visualize correlations between Salary, Experience, and Age. This helps in identifying relationships between key variables.
Outlier Detection and Removal:
IQR Method: Outliers in the Experience column are detected using the IQR method and then removed. The IQR is recalculated after removing outliers.
Z-score Method: Outliers are also detected using the z-score method. Z-scores greater than 3 or less than -3 are considered outliers and are removed from the data.
Appending New Data:
Two new rows are appended to the dataset, representing hypothetical employees with specific values for Salary, Experience, and other features.
Final Cleanup:
The last two rows (newly added) are dropped from the dataframe to revert the dataset to its previous state.

TASK-2
Simple Linear Regression Project
This project involves implementing a simple linear regression model using Python. The goal is to understand the process of predicting a continuous target variable based on one or more input features. Here’s a summary of the steps involved:

Objective:
The main objective is to:

Build a simple linear regression model.
Train the model using a dataset with continuous target variables.
Evaluate the model's performance using metrics such as Mean Squared Error (MSE) and R-squared (R²).
Visualize the regression line and the relationship between actual and predicted values.
Linear Regression Concept:
Linear regression is a statistical method for modeling the relationship between a dependent variable (target) and one or more independent variables (features). In this project, we use a single feature to predict the target variable, making it simple linear regression.

 : Coefficient of the feature (slope of the line).
𝜖
ϵ: Error term (random noise).
Steps of the Project:
1. Data Generation or Loading:
A dataset is either created synthetically or loaded from an external source.
In our case, we generated random input data (X) and computed the target variable (y) using a linear equation with added noise.
2. Data Splitting:
The dataset is split into two subsets:
Training Set (80%): Used to train the model.
Testing Set (20%): Used to evaluate the model’s performance on unseen data.
This ensures that the model is tested on data it hasn't seen before, preventing overfitting.
3. Training the Model:
A linear regression model is trained using the training set.
The model attempts to learn the relationship between the feature (X_train) and the target variable (y_train) by estimating the best-fit line that minimizes the prediction error.
4. Making Predictions:
After training, the model makes predictions on the test set.
The test set data (X_test) is passed through the model to predict the corresponding target values (y_pred).
5. Model Evaluation:
Two key performance metrics are used to evaluate the model:
Mean Squared Error (MSE): Measures the average of the squared differences between actual and predicted values. Lower MSE indicates better performance.
R-squared (R²): Measures how well the model explains the variability of the data. R² ranges from 0 to 1, where 1 indicates a perfect fit.
6. Visualization:
Regression Line: The model's predictions (regression line) are plotted over the training data to visualize how well the line fits the data.
Actual vs Predicted Values: A scatter plot is used to compare the actual vs. predicted values. The closer the points are to the ideal diagonal line, the better the model's predictions.
