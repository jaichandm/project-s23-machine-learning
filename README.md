<a name="readme-top"></a>

<!-- SPRINT SHIELDS -->
<a href="#overview">![Overview][overview-shield]</a>
<a href="#init_exp">![Init_exp][init_exp-shield]</a>
<a href="#lin_reg">![Lin_reg][lin_reg-shield]</a>
<a href="#classification">![classification][classification-shield]</a>

# Laptop price prediction
<<<<<<< HEAD
=======
##  Notebooks
<a name="init_exp"></a>
### initial_exploration notebook
The initial_exploration notebook has been created and I have pulled in the laptop prices dataset using pandas library. I have explored the dataset by checking the first 5 rows, checking for missing and duplicate values, and dropping unnecessary columns. I have also identified the features that may be important in predicting laptop prices such as brand, processor, RAM, storage, screen size, graphics card, and operating system.

After cleaning the dataset, I have created training and testing sets using the train_test_split function from sklearn library. The training set contains 80% of the data while the testing set contains the remaining 20%. 

In summary, the initial exploration notebook has provided us with an overview of the laptop prices dataset, identified important features, cleaned the dataset, and split the data into training and testing sets for future modeling.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="lin_reg"></a>
### linear_regression notebook
In this notebook, I learned how to perform linear regression on a dataset to predict the prices of laptops. I started by reading the dataset, cleaning it, and selecting features for the independent variables X and the target variable Y. I then used one-hot encoding to convert categorical features to numerical ones and split the dataset into training and testing sets. However, the initial linear regression model did not perform well, with a negative R-squared score and a high mean absolute error, indicating that it was not good enought at predicting laptop prices.

The updated R-squared score of 0.729 and mean absolute error of ₹ 14812.68 indicate that the linear regression model with the selected features and the rounded-off weight feature is able to explain around 73% of the variance in the target variable (price) and the predicted prices are on average ₹ 14812.68 away from the true prices.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="classification"></a>
### classification notebook

The notebook uses pandas, sklearn.model_selection, and sklearn.preprocessing to train two different models on a laptop dataset, with mean squared error and R-squared metrics used to evaluate the decision tree regressor and accuracy, precision, and F1-score for the SVM model.

Updated with refined analysis of the models using random forest regressor and MLP regressor

<p align="right">(<a href="#readme-top">back to top</a>)</p>
>>>>>>> 7620d4fa201a2634eac60469a366004a3c170281

<a name="overview"></a>
## Overview on the project
### Objective:
The objective of this machine learning project is to predict the price of a laptop based on its specifications and features such as CPU, RAM, screen size, Resolution, storage, brand, etc.

### Introduction:
This project aims to build a machine learning model to predict the price of a laptop based on its specifications and features. Features that might be important in predicting laptop prices include brand, processor, RAM, storage, screen size, graphics card, and operating system. Some combinations of features that may be useful in predicting laptop prices include Processor and RAM, Graphics Card and Processor, and Storage and Brand. The goal is to create a model that can assist consumers in making informed decisions about purchasing laptops by providing them with an estimated price range based on the laptop's specifications.

__Note:__ Switched to Laptop price prediction instead of project on Boston House Prices
<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Features of importance:
Features that might be important in predicting laptop prices include:

* Brand: some brands may have a higher perceived value and therefore command a higher price
* Processor: faster processors generally cost more than slower ones
* RAM: more RAM may indicate a higher-end laptop and therefore a higher price
* Storage: larger storage capacities may command a higher price
* Screen Size: larger screens may command a higher price
* Graphics Card: a dedicated graphics card may indicate a higher-end laptop and therefore a higher price
* Operating System: certain operating systems, such as macOS, may command a higher price than others
<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Potential useful feature combinations:
Some combinations of features that may be useful in predicting laptop prices include:

Processor and RAM: faster processors and more RAM may indicate a higher-end laptop and therefore a higher price
Graphics Card and Processor: a dedicated graphics card and a faster processor may indicate a gaming laptop or high-performance laptop and therefore a higher price
Storage and Brand: certain brands may command a higher price for larger storage capacities.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Expected Goals:
The goal is to create a model that can assist consumers in making informed decisions about purchasing laptops by providing them with an estimated price range based on the laptop's specifications.

Design a predictive model that can accurately predict the price of a laptop based on its features and specifications.
The model will take in the relevant laptop features, such as brand, processor, RAM, storage, screen size, graphics card, and operating system, and output a predicted price for the laptop.
The model will be trained on the available laptop price dataset and evaluated for its accuracy in predicting prices for new laptops with similar features.

### Conclusion:
In this project, we explored several datasets and used data cleaning and feature engineering techniques to prepare the data for modeling. I then applied various regression and classification algorithms, such as linear regression, decision trees, SVC, random forests, and neural networks, to train our predictive model. We evaluated the accuracy of our model using metrics such as mean squared error, R-squared score, and precision, and compared the results to baseline models and other models to assess their performance.

Overall, I can be concluded that the random forest regression model is a more accurate predictor of the overall cost of a laptop than the linear regression model. The random forest model outperformed the linear regression model in terms of R2 score and MSE, indicating a stronger capacity for prediction. 

I also found below features having strong correlation with price of the laptop(list in decreasing order):
Ram, SSD, ppi(pixel count), CPU brand

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Links

- [RAW DATA](RAW_DATA.md)
- [DATA](DATA.md)
- [ANALYSIS](ANALYSIS.md)
- [CONCLUSION](CONCLUSION.md)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

##  Notebooks
<a name="init_exp"></a>
### initial_exploration notebook
The code is performing data cleaning and feature engineering on the "Laptop Prices" dataset. Here is a summary of what the code is doing:

* The "Ram" and "Weight" columns are cleaned by removing the units and converting them to numeric types.
* The "Touchscreen" and "Ips" columns are created based on the presence of certain keywords in the "ScreenResolution" column.
* The "X_res" and "Y_res" columns are extracted from the "ScreenResolution" column and cleaned by removing commas and converting them to numeric types.
* The "ppi" column is created by calculating the pixel density of the screen based on the "X_res", "Y_res", and "Inches" columns.
* The "Cpu brand" column is created based on the processor brand in the "Cpu" column.
* The "Memory" column is cleaned by removing the units and converting them to numeric types.
* The "Layer1HDD", "Layer1SSD", "Layer1Hybrid", and "Layer1Flash_Storage" columns are created based on the presence of certain keywords in the "Memory" column.
* The "Layer2HDD", "Layer2SSD", and "Layer2Hybrid" columns are created based on the presence of certain keywords in the second layer of the "Memory" column.

Overall, the code is preparing the dataset for further analysis and modeling by cleaning and transforming the data into a more useful format.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="lin_reg"></a>
### linear_regression notebook
The linear notebook is performing linear regression on a laptop price dataset using scikit-learn. The dataset is split into training and testing sets using the train_test_split function. The ColumnTransformer class is used to transform the categorical variables using one-hot encoding. The transformed data is then fed into a linear regression model using the LinearRegression class.

The Pipeline class is used to chain the data transformation and the regression model together. The model is trained on the training set using the fit method and then used to make predictions on the test set using the predict method. The notebook then calculates the R2 score and mean squared error (MSE) using the r2_score and mean_squared_error functions, respectively.

Finally, the notebook generates a scatter plot of the predicted versus actual values using matplotlib. The plot includes a line of best fit to visually compare the predicted and actual values. The R2 score of 0.807 indicates a relatively good fit of the linear regression model to the data, while the MSE of 0.0737 shows the average squared difference between the predicted and actual values.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="classification"></a>
### classification notebook

The notebook uses pandas, sklearn.model_selection, and sklearn.preprocessing to train two different models on a laptop dataset, with mean squared error and R-squared metrics used to evaluate the decision tree regressor and accuracy, precision, and F1-score for the SVM model.

Updated with refined analysis of the models using random forest regressor and MLP regressor

The Decision Tree and Linear SVC models have an R2 score of 1.0 and an MSE of 0.0, which suggests that they have a perfect fit to the data. This might indicate that the models are overfitting the data.

The MLP Regressor model has an R2 score of -2.199 and an MSE of 1.171, which indicates that the model performs poorly on the dataset. A negative R2 score means that the model is worse than the baseline model that always predicts the mean of the target variable. The high MSE also suggests that the model is making large errors in its predictions.

The Random Forest model has an R2 score of 0.887 and an MSE of 0.043, which suggests that the model performs well on the dataset.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS -->
[overview-shield]: https://img.shields.io/badge/Overview-brightgreen
[init_exp-shield]: https://img.shields.io/badge/notebook-initial__exploration-yellowgreen
[lin_reg-shield]: https://img.shields.io/badge/notebook-linear__regression-yellowgreen
[classification-shield]: https://img.shields.io/badge/notebook-classification-yellowgreen
