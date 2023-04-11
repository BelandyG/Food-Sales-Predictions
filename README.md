# **Food Sales Predictions**
The goal of this analysis is to provide insights into the retailer's sales data and to create a machine learning model that predicts some of the variation in the data.

**Author**: Belandy Gard

# **Cleaning**
Before machine learning preprocessing, the data was cleaned with the following steps:

- Duplicate rows were dropped
- Spelling inconsistencies were fixed
- Categorical ordinal data was numerically encoded
- High-cardinality feature was dropped ('Item_Identifier')

# **Exploratory Visualization**
To understand the data statistical analyses Exploratory Visualization was completed to explain, or model the data. This was done by each of thed following:

- Histogram to view the distributions of various features in your dataset.
- Boxplot to view statistical summaries of various features in your dataset.
- Heatmap of the correlation between features.

This histogram shows the relationshiop of Item_Outlet_Sales and Outlet location. This can give a better understanding of which outlet produces the best sales.

![image](https://user-images.githubusercontent.com/123032319/230794220-6470ade3-05a6-442f-a220-561dd3580a0e.png)

This heatmap can be used to see which features are highly correlated with eachother.

![image](https://user-images.githubusercontent.com/123032319/230794673-5865c88f-fd36-467f-a64a-293007c5091d.png)


# **Explanatory Visualization**
Explanatory visualizations was used to communicate the results of data analyses. This will convey the results of the data analsis in a clear and concise manner. The goal of explanatory data visualization is to communicate findings and inspire action.

The following Barplot can be used to help determine which product type produces the best Outlet sales

![image](https://user-images.githubusercontent.com/123032319/230795142-0291d32d-952e-47af-9803-80a58da35899.png)


This Barplot can be used to help determine which Outlet Location had the least and most amount of Item sales

![image](https://user-images.githubusercontent.com/123032319/230795979-98237b66-cb5f-45e3-8649-55336458620d.png)



# **Machine Learning**

The data was preprocessed before fitting and testing machine learning models with the following steps:

Validation was performed (75% of data retained for training; 25% reserved for testing)
Missing numerical values were imputed with the mean
Numerical features were scaled
Missing nominal vlues were imputed with the most frequent value
Nominal features were one-hot encoded

# **Linear Regression Model**

A linear and random forest regression model was fit on the training data and then tested on the reserved testing data.
- This model performed well on both the training and test set. 
- This model can account for about 57% of the variation in the test data

# **Decision Tree Regression Model**

A Decision Tree regression model was fit on the training data and then tested on the reserved testing data.

The results improved as far as the regression metrics and the model's performance.
- This model contained some bias.
- For the R^2 score 59.5% of the variance is explained.
- For the MAE testing data is off by about $738.31


# **Final Recommendations**
The Decision Tree regression model would be the best recommendation. The data set showed low bias as it performed well in both training and testing.
This model showed the most accurate predictions of training and test scores.
