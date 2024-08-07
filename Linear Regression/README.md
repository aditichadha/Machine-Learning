
# Gradient Descent and Closed Form Solutions for Linear Regression
In this notebook, I will be implementing the closed form, gradient descent, and stochastic gradient descent techniques. I will also evaluate their performance through various combinations of learning rates and regularization parameters on training, convergence, and ultimate performance.

## Steps Taken:
1. Constructor Initialization: Initializes the class with input features 𝑋, target variable 𝑦 learning rate, epsilon for convergence, maximum iterations, regularization parameter (λ), and flags for gradient descent (gd) and stochastic gradient descent (sgd).

2. Data Splitting: The split_data method splits the dataset into training and test sets.

3. Normalization: The normalize_train and normalize_test methods standardize the features and add a column of ones for the intercept term.

4. Rank Checking: The rank, check_fullRank, and check_lowRank methods check if the matrix X has full rank or is low rank.

5. Closed Form Solution: The close_form_solution method calculates the optimal weights using the normal equation.

6. Gradient Descent: The gradient_descent method iteratively updates the weights to minimize the cost function.

7. Stochastic Gradient Descent: The stochastic_gd method updates weights using a single training example at a time.

8. Model Fitting: The fit method orchestrates the data preparation, rank checking, and calls the appropriate solution method (closed-form or gradient descent).

9. Plotting RMSE: The plot_rmse method plots the RMSE over iterations for gradient descent methods.
