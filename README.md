# Sales prediction for food items sold at various stores

Numann Malik

## Objectives

- Our main goal is to help the retailer understand the properties of products and outlets that play crucial roles in increasing sales.
- After cleaning the data we completed statistical analyses that might help us understand, explain, or model with our data. This includes a Histogram to view the distributions of various features in our dataset, aBoxplot to view statistical summaries of various features in our dataset, and a Heatmap of the correlation between features.
- We built several data visualizations to help our stakeholders better understand trends in the data.
- By using machine learning, we help the retailer to make predictions about future sales based on the data provided.
- Finally, we built a linear regression model and a simple regression tree model on our data set. These are to help the retailer understand the properties of products and outlets that play crucial roles in predicting sales.

## Data Dictionary

Below is a key for what each column in our data set represents:

![DD](DD.png)

## Visual insights from the data

Below are a subset of exploratory and explanatory data visualizations to help us understand any trends in the data:

![MRP](MRP.png)

![FT](FT.png)

![OS](OS.png)

## Summary of the model and its evaluation metrics

Below we state the R squared and mean squared error scores for our two models:

- Linear Regression Model
 - LR Model Training R2: 0.6712693760364781
 - LR Model Testing R2: -9.996148242813593e+19
 - LR Model Training RMSE: 986.3385424596464
 - LR Model Testing RMSE: 16606970213579.328

- Simple Regression Tree Model:
 - DT Model Training R2: 1.0
 - DT Model Testing R2: 0.21988566762195583
 - DT Model Training RMSE: 4.925864104892086e-15
 - DT Model Testing RMSE: 1467.0779546170936

- Tunded Simple Regression Tree Model:
 - DT Model Training R2: 0.6042066848171654
 - DT Model Testing R2: 0.5960039728227073
 - DT Model Training RMSE: 1082.281287111312
 - DT Model Testing RMSE: 1055.7536944506849

## Final recommendations

- Overall, we recommend the tuned Decision Tree model over Linear Regression due to the improved testing data results (we keep in mind that there is high bias even after tuning the max depth to 5). From the testing R^2 score we see that 59.6% of the 'Item Outlet Sales' variance is explained, with root mean square error of 1055.69.
- MRPs are widely distributed amongst food items. There is one particularly low count around the $70 range.
- Fruits, vegetables, and snack foods dominate in quantity. However, seafood items lie at the bottom of food types, followed by breakfast and starchy foods. Retailers may therefore wish to focus on selling more of the dominant food categories, and fewer on the low end of the ditribution.
- Outlet 27, which is a Tier/Type 3 Supermarket, far outsells the other outlets (most of which are Type 1 supermarkets). Groceries sold far fewer products compared to all types of supermarkets in comparison. The retailer may then want to investigate further to see how Outlet 27 is performing more successfully.
