# CS6220 Final Project
1. California Housing Price Prediction
   
This repository contains the final project for CS6220, where we explore and compare multiple models to predict housing prices in California using a real-world dataset.


2. Dataset
   
We used the California Housing Prices dataset from Kaggle, which includes both demographic and geographic features such as:
- Median_House_Value (Target Values)
- Median Income
- Median_Age
- Total Rooms and Bedrooms
- Latitude and Longitude
- Population
- Households
- Distances to major cities (e.g., LA, San Diego, San Jose, San Francisco)
- Distance to the coast

3. Project Objectives
   
- Perform data cleaning and remove capped housing values (at $500,000) to reduce ceiling effect.
- Conduct exploratory data analysis (EDA) including histograms，scatter plots and correlation heatmap.
- Apply Principal Component Analysis (PCA) for 2D visualization.
- Train and evaluate four models:
Linear Regression
Decision Tree Regressor
Random Forest Regressor
Gradient Boosting Regressor

Evaluate models using:
R² score
Root Mean Squared Error (RMSE)
Residual plots

4. Key Results
   
Random Forest achieved the best performance:
R² ≈ 0.8047
RMSE ≈ 43,276.66

Gradient Boosting also performed well (R² ≈ 0.7544).
Linear Regression and Decision Tree underperformed due to oversimplification.

-Residual Analysis showed:

Linear Regression suffers from heteroscedasticity.
Random Forest and Gradient Boosting provided more evenly distributed residuals.

- Feature Importance:
 
Median Income is the most significant predictor.
Distance to coast and  Latitude also impacts housing prices.

5. Dependencies
   
Python - pandas, numpy, matplotlib, seaborn

scikit-learn


6. How to Run
   
You can open the notebook in Google Colab or Jupyter Notebook. The dataset is expected to be named California_Houses.csv.
Make sure to adjust the path if loading from a different location.

7. Reference
   
F. Soriano, California Housing Prices Data (extra features). Kaggle, 2022. [Online]. Available:
https://www.kaggle.com/datasets/fedesoriano/california-housing-prices-data-extra-features
