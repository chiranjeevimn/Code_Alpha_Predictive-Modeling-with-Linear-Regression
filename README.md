# Code_Alpha_Predictive-Modeling-with-Linear-Regression

This is a Python script for performing linear regression on a dataset related to salary and years of experience. Here's a step-by-step explanation of the code:

1. **Import Libraries:**
   - `pandas` and `numpy` are imported for data manipulation.
   - `train_test_split` from `sklearn.model_selection` is used for splitting the dataset.
   - `LinearRegression` from `sklearn.linear_model` is imported for linear regression modeling.
   - `mean_squared_error` and `r2_score` from `sklearn.metrics` are used to evaluate model performance.
   - `matplotlib.pyplot` and `seaborn` are used for data visualization.

2. **Load Dataset:**
   - The dataset is loaded from a CSV file using the `pd.read_csv` function.

3. **Data Visualization:**
   - Histograms of features and the target variable are plotted using `df.hist`.
   - Box plots of features and the target variable are plotted using `sns.boxplot`.
   - Pair plots are generated using `sns.pairplot` to visualize relationships between the target variable and one feature (`YearsExperience`).
   - Histogram and box plot of the target variable (`Salary`) are visualized.

4. **Outlier Detection:**
   - Outliers are identified using the Interquartile Range (IQR) method.
   - A box plot is created to visually identify outliers in the target variable.

5. **Data Preparation:**
   - Features (`YearsExperience`) and the target variable (`Salary`) are separated.

6. **Train-Test Split:**
   - The dataset is split into training and testing sets using `train_test_split`.

7. **Linear Regression Model:**
   - A linear regression model is initialized and trained on the training data.

8. **Model Evaluation:**
   - Predictions are made on the test set, and the model's performance is evaluated using mean squared error and R-squared.

9. **Visualization of Model Fit:**
   - The script includes visualizations of the training samples and the regression line.

10. **Predictions vs. Actual Values Visualization:**
   - Scatter plots and regression line visualizations are created to compare actual and predicted values on the test set.

11. **Repeated Model Training:**
   - The script repeats the model training process 5000 times with different random splits and records the R-squared scores.

12. **Print Results:**
   - The maximum R-squared score and the corresponding random state are printed.

In summary, this above code demonstrates the complete process of loading data, exploring its distribution, detecting outliers, preparing data for training, building a linear regression model, evaluating its performance, and visualizing the results. The repeated training with different random splits provides an understanding of the variability in model performance.
