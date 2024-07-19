# Real-Estate-Valuation-Project

## Overview
This project involves developing predictive models for real estate valuation using historical market data from Sindian Dist., New Taipei City, Taiwan. The aim is to estimate house prices based on various features such as transaction date, house age, distance to the nearest MRT station, number of convenience stores, latitude, and longitude.

## Objectives
1. **Predictive Modeling:** Develop a linear regression model to predict house prices and evaluate its performance using multiple metrics.
2. **Dimensionality Reduction:** Apply Principal Component Analysis (PCA) to reduce data dimensionality and build a regression model using the principal components.
3. **Performance Comparison:** Compare the performance of the original model with the PCA-based model to understand the impact of dimensionality reduction.

## Key Steps
1. **Data Preparation:**
   - Loaded and inspected the dataset, ensuring there were no missing values.
   - Split the dataset into training and testing sets.

2. **Model Training and Evaluation:**
   - Trained a linear regression model on the original dataset.
   - Evaluated the model using Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared Score (R²).

3. **Principal Component Analysis:**
   - Applied PCA to the dataset and selected the first three principal components.
   - Trained a new linear regression model using the PCA-transformed data.
   - Evaluated the PCA-based model using the same performance metrics.

4. **Visualization and Interpretation:**
   - Created scatter plots to visualize actual vs. predicted prices for both models.
   - Generated a scree plot to show the explained variance by each principal component.

## Results
### Original Model:
- **Mean Absolute Error (MAE):** 5.418
- **Mean Squared Error (MSE):** 54.599
- **Root Mean Squared Error (RMSE):** 7.389
- **R-squared Score (R²):** 0.675

### PCA Model:
- **Mean Absolute Error (MAE):** 6.308
- **Mean Squared Error (MSE):** 73.372
- **Root Mean Squared Error (RMSE):** 8.566
- **R-squared Score (R²):** 0.563

The original model performed better, indicating that the original features hold significant information for predicting house prices. The PCA model, while simpler, had slightly lower accuracy, demonstrating the trade-off between dimensionality reduction and information loss.

## Skills Demonstrated
- **Data Preprocessing:** Efficiently handled and prepared real-world data for modelling.
- **Predictive Modeling:** Built and evaluated regression models using scikit-learn.
- **Dimensionality Reduction:** Applied PCA to understand and manage high-dimensional data.
- **Performance Evaluation:** Utilized multiple metrics to assess model performance.
- **Visualization:** Created clear visualizations to interpret model results and explain findings.

## Attribution
This project is courtesy of Deakin University, where the dataset was obtained.
