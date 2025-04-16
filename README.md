Used car sales data is evaluated using various regression techniques. Once the model is created, it can be used to predict the sales price of a vehicle, as well as assessed to determine which features of a car have the biggest impact on price.

Three different regression algorithms were used (Linear Regression, Ridge Regression, and LASSO Regression) to produce models, which were then compared against each other.

For the linear regression, first, polynomial features of increasing degree were iterated and cross-validated to determine the optimal degree without overfitting. After that, SequentialFeatureSelector was used to limit the resulting features to 6.

For both Ridge and LASSO regressions, GridSearchCV was used for hyperparameter selection of alpha.

After the optimal model for each algorithm was determined, the models were tested with a test data set, and their mean squared errors were compared to determine the best model.

Additionally, the coefficients of each model were analyzed to gain insight into the primary driving factors in what determines the price of a used car.

After completing the analysis, the Ridge Regression model is determined to be the most optimal.

The features that have the biggest impact on the sales price are:
-Odometer reading
-Age
-Diesel fueled
-12 cylinder engine
-Convertable
-Electric
-Offroad
-Truck
