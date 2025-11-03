"Comparative Analysis of Regression Models for California Housing Price Prediction"

##Scenario:A real estate agency wants to estimate house prices in California based on various factors like location, number of rooms, and population density. They employ different machine learning models to predict prices and compare their predictions with actual market values to determine the most accurate approach.
##Step 1: Load and Explore the Dataset.We use the California Housing Dataset to train and test the model to see the models's Performance.A Pandas DataFrame is created to store the dataset.

##Step 2: Preprocessing DataFeatures (X) are selected by removing the target variable (Price).Data is standardized using StandardScaler to ensure all features are on the same scale.

##Step 3: Check for MulticollinearityVariance Inflation Factor (VIF) helps detect multicollinearity among features.If a feature has a high VIF (>5 or >10), it indicates redundancy.

##Step 4: Train-Test SplitThe dataset is split into 80% training data and 20% testing data.
##Step 5:Train and Evaluate Each ModelModels are trained on X_train and y_train.Predictions are made on X_test.
Models are evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), RMSE, and R-Square (R²).

##Step 6: Train Multiple Regression Models
Various regression models are trained, including Linear Regression, Ridge, Lasso, ElasticNet, SVR, Decision Trees, and Gradient Boosting.
