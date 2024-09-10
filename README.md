
# HW 2 due Sep 15th
Part 1: Refer to §1 of the code Lecture 5 Linear Regression.ipynb
(a) Notice that we used 100 epochs, which was a waste of time because we could have stopped earlier. After about epoch 55 or so, the loss does not significantly decrease. Modify the code so that if the percentage change in loss is less than 1%, you exit the iterations.

(b) The class MyLinReg in the above code uses batch gradient descent to find the minimum of the loss function. Modify the original code to use stochastic gradient descent (SGD) instead. Iterate over many iterations and observe how the RMSE changes. The graph of RMSE for batch gradient descent is typically smooth and decreases as the number of iterations increase. What can you say about the graph of RMSE when using stochastic gradient descent?

Part 2: Refer to §3 of the code Lecture 5 Linear Regression.ipynb
Use sklearn's SGDRegressor class instead of sklearn's LinearRegression. If the input variables are of different scales (e.g., TV and radio), scaling these variables typically improves SGD convergence. Read about sklearn's MinMaxScaler and explore if using it gives better results.
Link: sklearn MinMaxScalerLinks to an external site.

Part 3: Import the data file mtcars.csv
The goal is to identify two or three continuous numerical variables that can be used to predict mpg (miles per gallon) using multiple linear regression. You can use sklearn or a custom class, and experiment with batch gradient descent (GD), stochastic gradient descent (SGD), or mini-batch SGD, along with scaling.

Part 4: Read about the Probabilistic Interpretation of Linear Regression
Read pages 11–13 of reference [1] to understand the probabilistic interpretation of linear regression.
