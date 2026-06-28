# Model Comparison

# Introduction

To understand the factors influencing monthly sales, both simple regression and multiple regression models were developed and evaluated. The purpose of this comparison is to determine which model provides better explanatory power and stronger business insights.

## Model 1: Simple Regression using Marketing Spend

# Variables Used

* Dependent Variable: Monthly Sales
* Independent Variable: Marketing Spend

# Findings

The model showed a positive relationship between marketing spend and monthly sales. The coefficient indicated that an increase in marketing expenditure is associated with higher sales.

The R-squared value suggested that marketing spend alone explains only a limited portion of the variation in monthly sales.

The p-value was statistically significant, indicating that marketing spend is an important predictor of sales.

# Business Usefulness

This model is useful for understanding the direct impact of marketing activities on sales performance. However, it cannot capture the influence of other important business factors.

# Limitations

The model considers only one independent variable and ignores factors such as customer footfall, inventory levels, store characteristics, and regional differences.

---

## Model 2: Simple Regression using Footfall

# Variables Used

* Dependent Variable: Monthly Sales
* Independent Variable: Footfall

# Findings

A strong positive relationship was observed between footfall and monthly sales. The model produced a higher R-squared value compared to the marketing spend model, indicating greater explanatory power.

The p-value indicated that footfall is a statistically significant variable.

# Business Usefulness

This model helps management understand the importance of customer traffic in driving store sales.

# Limitations

Although useful, the model still ignores other business drivers and therefore provides only a partial explanation of sales performance.

---

## Model 3: Multiple Regression Model

# Variables Used

* Dependent Variable: Monthly Sales

# Independent Variables

* Marketing Spend
* Footfall
* Inventory Availability Percentage
* Region Dummy Variables
* Store Type Dummy Variables

# Findings

The multiple regression model achieved the highest R-squared value among all models, indicating superior explanatory power.

Several variables, particularly footfall, marketing spend, and inventory availability, were found to be statistically significant based on their p-values.

Positive coefficients indicated variables that increase sales, whereas negative coefficients represented factors associated with lower sales.

Some variables displayed weak statistical significance and should be interpreted cautiously.

# Business Usefulness

The multiple regression model is the most valuable for decision-making because it evaluates several business drivers simultaneously. It provides a more realistic understanding of store performance and allows management to prioritize actions effectively.

# Limitations

Despite its stronger performance, the model does not capture all possible influences on sales, such as seasonality, competitor actions, economic conditions, or customer preferences.

## Overall Conclusion

Among all models, the multiple regression model performed best because it explained the largest proportion of variation in monthly sales.

Therefore, the multiple regression model is recommended for business decision-making, while simple regression models should be used primarily for understanding the isolated effect of individual variables.

