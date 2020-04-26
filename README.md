                                                              Linear-regression

Linear Regression is a supervised machine learning algorithm where the predicted output is continuous and has a constant slope. It’s used to predict values within a continuous range, (e.g. housing prices) rather than trying to classify them into categories (e.g. breast cancer malignant or benign).

In Linear regression if we have only one feature and we have to predict the output(Only Simple regression).
We use hypothesis function to predict the value
                    h(x) = theta(0) + theta(1)(x)
To minimize the error between predicted value and the actual value we use cost function also called as squared error function
                    J(theta(0), theta(1)) = ((1/2*m) * (h(x) - y)^2)
To minimize the cost function gradient descent came into practice where we have to simultaneously update the theta value.
                    repeat until convergence
                    {
                    theta = theta - alpha*(partial derivative(J(theta)))
                    }
           here alpha is the learning rate which needs to be very small.
If alpha is too large it may overshoot the minimum and it can fail to converge or diverge.
Some Important Points related to Gradient Descent
1) If alpha is too small, then gradient descent may take  very long time to converge.
2) If theta(0) and theta(1) are not initialized at local minima then one iteration will not change their value.
3) If the first few iterations of gradient descent cause cost function to increase rather than decerease then the moost likely cause is that we have to set the learning rate to too large.
