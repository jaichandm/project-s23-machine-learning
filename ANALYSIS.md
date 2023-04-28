# Analysis on my project:

### linear Regression
The linear notebook is performing linear regression on a laptop price dataset using scikit-learn. The dataset is split into training and testing sets using the train_test_split function. The ColumnTransformer class is used to transform the categorical variables using one-hot encoding. The transformed data is then fed into a linear regression model using the LinearRegression class.

The Pipeline class is used to chain the data transformation and the regression model together. The model is trained on the training set using the fit method and then used to make predictions on the test set using the predict method. The notebook then calculates the R2 score and mean squared error (MSE) using the r2_score and mean_squared_error functions, respectively.

Finally, the notebook generates a scatter plot of the predicted versus actual values using matplotlib. The plot includes a line of best fit to visually compare the predicted and actual values. The R2 score of 0.807 indicates a relatively good fit of the linear regression model to the data, while the MSE of 0.0737 shows the average squared difference between the predicted and actual values.

[Linear Regression Notebook](linear_regression.ipynb)

### Classification notebook

The notebook uses pandas, sklearn.model_selection, and sklearn.preprocessing to train two different models on a laptop dataset, with mean squared error and R-squared metrics used to evaluate the decision tree regressor and accuracy, precision, and F1-score for the SVM model.

Updated with refined analysis of the models using random forest regressor and MLP regressor

The Decision Tree and Linear SVC models have an R2 score of 1.0 and an MSE of 0.0, which suggests that they have a perfect fit to the data. This might indicate that the models are overfitting the data.

The MLP Regressor model has an R2 score of -2.199 and an MSE of 1.171, which indicates that the model performs poorly on the dataset. A negative R2 score means that the model is worse than the baseline model that always predicts the mean of the target variable. The high MSE also suggests that the model is making large errors in its predictions.

The Random Forest model has an R2 score of 0.887 and an MSE of 0.043, which suggests that the model performs well on the dataset.

[Classification Notebook](classification.ipynb)

### Limitations

The major problem I encountered was that there were all the String values in my dataset initially. I had to use a lot of regular expressions to filter and store necessary data.