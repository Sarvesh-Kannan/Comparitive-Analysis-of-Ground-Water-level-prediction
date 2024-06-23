# Groundwater Levels Prediction for Chennai (2011-2021)

## Overview
This project focuses on predicting groundwater levels in Chennai city using data from the years 2011 to 2021. The project uses two different regression models: Polynomial Regression and Linear Regression, to conduct a comparative analysis. The dataset contains historical groundwater levels along with date information in the `Month-Year` format. The project preprocesses the data, handles missing values, and evaluates the performance of the regression models, demonstrating that Polynomial Regression performs better.

## Dataset
The dataset used for this project is `EVS_Dataset.csv`. The key column is `Groundwater Levels`, and the date information is in the `Month-Year` column. The data covers groundwater levels in Chennai from the year 2011 to 2021.

## Requirements
- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Project Structure
The main script for this project performs the following steps:
1. **Data Loading and Preprocessing**
2. **Model Training**
3. **Model Evaluation**
4. **Performance Comparison**
5. **Visualization**

### Data Loading and Preprocessing
1. Load the dataset using Pandas.
2. Convert the `Month-Year` column to datetime format.
3. Extract day, month, and year from the `Month-Year` column.
4. Handle missing values in the `Groundwater Levels` column by replacing them with the mean value.

### Model Training
Two models are trained on the preprocessed data:
1. **Polynomial Regression**: 
   - Uses a polynomial degree of 2.
   - Combines Polynomial Features, Standard Scaler, and Linear Regression in a pipeline.
2. **Linear Regression**: 
   - Standard Linear Regression model without polynomial features.

### Model Evaluation
1. Evaluate both models using Mean Squared Error (MSE) and R-squared metrics.
2. Compare the performance of the models based on these metrics.

### Performance Comparison
The project demonstrates that Polynomial Regression performs better than Linear Regression in predicting groundwater levels in Chennai.

### Visualization
The results are visualized using bar charts to compare the MSE and R-squared values of the two models.

## Usage
1. Ensure all required libraries are installed.
2. Place the `EVS_Dataset.csv` file in the same directory as the script.
3. Run the script to perform data preprocessing, model training, evaluation, and visualization.
