<a name="readme-top"></a>

<!-- SPRINT SHIELDS -->
<a href="#overview">![Overview][overview-shield]</a>
<a href="#init_exp">![Init_exp][init_exp-shield]</a>
<a href="#lin_reg">![Lin_reg][lin_reg-shield]</a>

# Laptop price prediction
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

<a name="overview"></a>
## Overview on the project
### Objective:
The objective of this machine learning project is to predict the price of a laptop based on its specifications and features such as CPU, RAM, screen size, storage, brand, etc.

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

### Expected Answer/Output:
The goal is to create a model that can assist consumers in making informed decisions about purchasing laptops by providing them with an estimated price range based on the laptop's specifications.

Design a predictive model that can accurately predict the price of a laptop based on its features and specifications.
The model will take in the relevant laptop features, such as brand, processor, RAM, storage, screen size, graphics card, and operating system, and output a predicted price for the laptop.
The model will be trained on the available laptop price dataset and evaluated for its accuracy in predicting prices for new laptops with similar features.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Data source:
Here are few possible sources for my project:

1. [Dataset](https://www.kaggle.com/datasets/mohidabdulrehman/laptop-price-dataset) by MOHID ABDUL REHMAN
2. [Dataset](https://www.kaggle.com/datasets/kuchhbhi/latest-laptop-price-list?select=Cleaned_Laptop_data.csv) by SANTOSH KUMAR
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS -->
[overview-shield]: https://img.shields.io/badge/Overview-brightgreen
[init_exp-shield]: https://img.shields.io/badge/notebook-initial__exploration-yellowgreen
[lin_reg-shield]: https://img.shields.io/badge/notebook-linear__regression-yellowgreen
