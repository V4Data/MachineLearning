**Linear Regression Algorithms**

**1\. Gradient Descent:**  
   \- *Purpose*: This optimization algorithm is used to find the best-fitting line by minimizing the cost function, which quantifies how far the predicted values are from the actual values.

   \- *Key Concept*: It updates the coefficients iteratively based on the gradient (slope) of the cost function with respect to the coefficients. The update rule is: β := β \- α ∇L, where α is the learning rate (a small positive value) and ∇L is the gradient of the loss function.

   \- *Advantages*: Efficient for large datasets that do not fit into memory, as it can work with smaller batches or even single data points. Can be generalized to optimize other types of loss functions beyond linear regression.

   \- *Limitations*: The choice of learning rate (α) is crucial; too high can cause divergence, while too low can lead to slow convergence. May converge to local minima rather than the global minimum, particularly in non-convex problems.

**2\. Ridge Regression (L2 Regularization):**  
   \- *Purpose*: This method addresses the issue of overfitting by adding a penalty term to the loss function, which discourages high coefficients.

   \- *Key Formula*: The objective function minimizes the residual sum of squares plus the penalty term: Minimize ∑ (y\_i \- ŷ\_i)² \+ λ ∑ β\_j². Here, λ is a tuning parameter that controls the strength of the penalty.

   \- *Advantages*: Useful in cases of multicollinearity (when independent variables are highly correlated), as it stabilizes the coefficient estimates. Helps to maintain all predictors in the model and reduces variance.

   \- *Limitations*: Assumes a linear relationship between dependent and independent variables. Does not perform variable selection; all features remain in the model, which can be a drawback in very high-dimensional datasets.

**3\. Lasso Regression (L1 Regularization):**  
   \- *Purpose*: This technique also aims to prevent overfitting, but it does so by adding a penalty that can shrink some coefficients to exactly zero, effectively selecting a simpler model.

   \- *Key Formula*: The objective is: Minimize ∑ (y\_i \- ŷ\_i)² \+ λ ∑ |β\_j|. 

   \- *Advantages*: Performs automatic feature selection by excluding less important features, leading to a simpler and more interpretable model. Particularly effective in high-dimensional datasets where the number of predictors exceeds the number of observations.  
   \- *Limitations*: Can be less stable than Ridge when features are highly correlated, as it may arbitrarily select one feature over another rather than accounting for them both. Requires careful tuning of λ to balance between bias and variance.  
