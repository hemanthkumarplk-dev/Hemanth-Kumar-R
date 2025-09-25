Housing Price Prediction using Linear Regression
📌 Project Overview

This project builds a Linear Regression model to predict house prices based on features such as area, bedrooms, bathrooms, parking, and categorical attributes (like furnishing status, air conditioning, etc.).

We followed a step-by-step machine learning pipeline:

🚀 Steps Followed
1. Import and Preprocess the Dataset

Loaded the Housing.csv dataset using pandas.

Converted categorical columns (e.g., mainroad, guestroom, furnishingstatus) into numerical dummy variables using one-hot encoding.

Ensured the dataset was fully numeric and ready for model training.

2. Split Data into Train-Test Sets

Divided the dataset into features (X) and target (y = price).

Used train_test_split() to split into:

80% training data (for learning)

20% testing data (for evaluation).

3. Fit a Linear Regression Model

Created a Linear Regression model using sklearn.linear_model.LinearRegression.

Trained the model on the training set (X_train, y_train).

4. Evaluate the Model

Predicted house prices on the test set.

Calculated evaluation metrics:

MAE (Mean Absolute Error) → Average absolute error in predictions.

MSE (Mean Squared Error) → Squared error, penalizes large mistakes.

R² Score → Measures how well the model explains variation in price.

5. Plot Regression & Interpret Coefficients

Plotted actual vs predicted prices (example with area feature).

Extracted model coefficients:

Intercept (b0): Base house price when all features = 0.

Coefficients (b1, b2, ...): Effect of each feature on house price.

Example: If coefficient for area = 500, each additional sq ft increases price by ₹500 (keeping other factors constant).

📊 Key Insights

The model shows which features strongly influence house prices.

Numeric features like area and categorical ones like airconditioning_yes significantly impact price.

Performance (R² score) tells how well the model explains price variation.
