# Air Quality Prediction

This project demonstrates a regression model for air quality prediction using a multiple linear regression algorithm in R. The model is built using the air quality dataset, which contains hourly responses from a gas multisensor device deployed in an Italian city. The dataset also includes gas concentrations references from a certified analyzer.

## Data

The dataset contains 9358 instances of hourly averaged responses from an array of 5 metal oxide chemical sensors embedded in an Air Quality Chemical Multisensor Device. The device was located on the field in a significantly polluted area, at road level, within an Italian city.

You can access the dataset and its information from the following link: [Air Quality Dataset](https://archive.ics.uci.edu/ml/datasets/Air+Quality#)

Data were recorded from March 2004 to February 2005 (one year), representing the longest freely available recordings of on-field deployed air quality chemical sensor devices responses. Ground Truth hourly averaged concentrations for CO, Non Metanic Hydrocarbons, Benzene, Total Nitrogen Oxides (NOx), and Nitrogen Dioxide (NO2) were provided by a co-located reference certified analyzer.

Missing values are tagged with -200 value.

### Attribute Information

1.  Date (DD/MM/YYYY)

2.  Time (HH.MM.SS)

3.  CO.GT. - True hourly averaged concentration CO in mg/m\^3 (reference analyzer)

4.  PT08.S1(CO)-Tin oxide hourly averaged sensor response (nominally CO targeted).

5.  C6H6(GT)-True hourly averaged Benzene concentration in microg/m\^3 (reference analyzer).

6.  PT08.S2(NMHC)-Titania hourly averaged sensor response (nominally NMHC targeted).

7.  NOx(GT)-True hourly averaged NOx concentration in ppb (reference analyzer)

8.  PT08.S3(NOx)-Tungsten oxide hourly averaged sensor response (nominally NOx targeted).

9.  NO2(GT)-True hourly averaged NO2 concentration in microg/m\^3 (reference analyzer).

10. PT08.S4 (tungsten oxide)-hourly averaged sensor response (nominally NO2 targeted).

11. PT08.S5 (indium oxide)-hourly averaged sensor response (nominally O3 targeted).

12. Temperature-Temperature in Â°C.

13. Humidity-Relative Humidity (%).

14. AH-Absolute Humidity.


## Project Structure
The repository is organized into several sections:

1. Data: This section provides an overview of the dataset, including the input variables and the target variable. It describes the attributes and their meanings, helping you understand the data better.

2. Data Preprocessing:
   - Handle missing values: If there are missing values in the dataset, perform necessary imputation or deletion.
   - Handle outliers: Identify and handle outliers, either by removing them or applying appropriate transformations.
   - Perform feature engineering: Create new features or transform existing features if necessary.
   - Encode categorical variables: Convert categorical variables into numerical form if needed.
   - Split the data into independent variables (X) and the target variable (y).

3. Exploratory Data Analysis (EDA):
   - Conduct a detailed exploration of the dataset.
   - Display basic statistics, such as mean, standard deviation, minimum, maximum, and quartiles.
   - Visualize the data using plots, histograms, box plots, scatter plots, etc.
   - Analyze correlations between variables using correlation matrices or heatmaps.

4. Building a Multiple Linear Regression Model:
   4.1. Split the data into Training and Testing sets:
       - Use the `train_test_split()` function to split the data into training and testing sets.
   
   4.2. Model Training:
       - Import the Multiple Linear Regression model from the appropriate library.
       - Create an instance of the Multiple Linear Regression model.
       - Train the model on the training data using the `fit()` method.

   4.3. Model Prediction:
       - Use the trained model to make predictions on the test data using the `predict()` method.

   4.4. Model Evaluation:
       - Evaluate the performance of the model using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
       - Compare the predicted values with the actual values.

5. Key Assumption Check:
   - Check the assumptions of multiple linear regression, such as linearity, normality, independence, and homoscedasticity.
   - If any assumptions are violated, apply appropriate transformations or consider alternative regression models.

6. Re-building the Model:
   - Based on the assumption check, perform necessary adjustments to the model, such as feature selection, feature transformation, or including interaction terms.
   - Re-train and evaluate the updated model.

7. Conclusion:
   - Summarize the findings and results from the analysis.
   - Discuss the limitations of the model and potential areas for improvement.
   - Provide recommendations or insights based on the analysis.

This project structure provides a logical flow for your code, starting from data preprocessing and EDA to building, evaluating, and refining the Multiple Linear Regression model.

The detailed project report can be found in the output folder. It is available in HTML format, providing comprehensive analysis, insights, and conclusions derived from the regression models.

## Usage
To run the code and reproduce the results, you need to have R installed on your machine along with the necessary libraries specified in the code. Make sure to set the working directory correctly and run the scripts in the provided order to ensure proper execution.


## Contributions
Contributions to this project are welcome! If you have any suggestions, improvements, or bug fixes, please feel free to open an issue or submit a pull request. Let's collaborate and make this project even better!


## References
  [1] Kaggle Datasets
  
  [2] UCI Machine Learning Repository

