# Dummy Variable Creation

To include categorical variables in the regression model, dummy variables were created for the variables **region** and **store_type**.

A one-hot encoding approach was used, where each category is represented by a binary variable (0 or 1).

To avoid multicollinearity and the dummy variable trap, one category from each variable was excluded and used as the reference category.

# Region Variable

Dummy variables were created for all regions except the reference category.

* Reference Category: **North** (example)
* Created Dummy Variables:

  * region_East
  * region_South
  * region_West

Interpretation:
The coefficient of each region dummy variable represents the expected difference in monthly sales compared to the reference region (North), while holding all other variables constant.

# Store Type Variable

Dummy variables were created for all store types except the reference category.

* Reference Category: **Standard** (example)
* Created Dummy Variables:

  * store_type_Express
  * store_type_Premium

Interpretation:
The coefficient of each store type dummy variable measures the expected change in monthly sales relative to the reference store type (Standard), controlling for other predictors.

The first category was dropped during encoding (`drop_first = True`) to eliminate redundancy and ensure a stable regression model.




# Model Equations

## Simple Regression Model 1: Monthly Sales and Marketing Spend

# Regression Equation

Monthly Sales = 560777.35 + (2.13 × Marketing Spend)

# Business Interpretation

This equation indicates that increasing marketing expenditure is associated with higher monthly sales. Specifically, for every additional unit spent on marketing, monthly sales are expected to increase by approximately 2.13 units, assuming other conditions remain unchanged.

The intercept represents the estimated monthly sales when marketing spend is zero.

---

## Simple Regression Model 2: Monthly Sales and Footfall

# Regression Equation

Monthly Sales = 446410.58 + (35.68 × Footfall)

# Business Interpretation

This model suggests that customer traffic has a strong positive impact on sales. For every additional customer visiting the store, monthly sales are expected to increase by approximately 35.68 units.

The intercept represents estimated monthly sales when customer footfall is zero.

---

## Multiple Regression Model

# Regression Equation

Monthly Sales = β₀ + β₁(Marketing Spend) + β₂(Footfall) + β₃(Inventory Availability Percentage) + β₄(Region Dummy Variables) + β₅(Store Type Dummy Variables)

# Business Interpretation of Coefficients

* **Marketing Spend Coefficient:** Indicates the expected change in monthly sales resulting from additional marketing investment.
* **Footfall Coefficient:** Measures the expected increase in sales associated with additional customer visits.
* **Inventory Availability Coefficient:** Shows how maintaining adequate inventory levels influences sales performance.
* **Region Coefficients:** Indicate how sales differ across regions relative to the reference region.
* **Store Type Coefficients:** Measure differences in sales performance across store formats relative to the reference store type.

Positive coefficients indicate factors that increase sales, whereas negative coefficients indicate factors associated with lower sales.

---

## Dummy Variable Explanation

Categorical variables such as **region** and **store_type** were converted into dummy variables to allow their inclusion in the regression model.

To avoid redundancy and multicollinearity, one category from each variable was excluded from the analysis and used as the reference category.

## Reference Categories

* Region Reference Category: **North**
* Store Type Reference Category: **Standard**

All other categories were interpreted relative to these baseline categories.

---

## Final Model Selected

The **Multiple Regression Model** was selected as the final model.

## Reason for Selection

The multiple regression model was selected because it considers several business drivers simultaneously and provides a more comprehensive explanation of monthly sales performance.

Compared with simple regression models, the multiple regression model offers greater explanatory power and produces more useful insights for business decision-making.

The model enables management to evaluate the combined effects of marketing activities, customer traffic, inventory availability, regional differences, and store characteristics when making strategic decisions.

