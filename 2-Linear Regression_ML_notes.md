  
***Linear Regression in Machine Learning***

**Definition:**    
Linear regression is a supervised learning algorithm used to predict a continuous target variable based on one or more independent variables.

**1\. Linear Regression Equation**

The relationship is modeled as:

y \= β₀ \+ β₁x₁ \+ β₂x₂ \+ ... \+ βₙxₙ \+ ε

Where:  
\- y: Predicted output (dependent variable)  
\- β₀: Intercept (constant term)  
\- β₁, β₂, ..., βₙ: Coefficients (weights) of the features  
\- x₁, x₂, ..., xₙ: Input features (independent variables)  
\- ε: Error term (residuals)

**2\. Assumptions of Linear Regression**  
. Linearity: The relationship between predictors and response is linear.  
. Independence: Observations are independent.  
. Homoscedasticity: Residuals have constant variance.  
. Normality: Residuals are normally distributed.

**3\. Cost Function**  
Minimize the difference between predicted and actual values using Mean Squared Error (MSE):

MSE \= (1/n) \* Σ(yᵢ \- ŷᵢ)²

Where:  
\- yᵢ: Actual value  
\- ŷᵢ: Predicted value  
\- n: Number of observations

**4\. Derivation of Coefficients**

Find coefficients (β) using the Normal Equation:

β \= (XᵀX)⁻¹Xᵀy

Where:  
\- X: Input features matrix  
\- y: Actual outputs vector

**5\. Evaluation Metrics**

R-squared measures the proportion of variance explained by the independent variables:

R² \= 1 \- (SS\_res / SS\_tot)

Where:  
\- SS\_res \= Σ(yᵢ \- ŷᵢ)² (Residual sum of squares)  
\- SS\_tot \= Σ(yᵢ \- ȳ)² (Total sum of squares)

**6\. Advantages and Disadvantages**

Advantages:  
\- Simple to implement and interpret.  
\- Efficient for linearly separable data.

Disadvantages:  
\- Assumes linearity, which may not always hold.  
\- Sensitive to outliers.

