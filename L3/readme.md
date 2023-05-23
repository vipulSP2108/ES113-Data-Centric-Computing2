# Problem

Load the Diabetes dataset using (x, y) =
sklearn.datasets. load_diabetes (return _X_y= True). 
We will fit the following regression models to predict the y values (blood sugar) based on the
features. We will use the sklearn implementation of the regression models.

> 1. LinearRegression
> 2. RandomForestRegressor (random_state=1)
> 3. GradientBoostingRegressor (random_state=1)

> 1. What is the resulting residual error value for each of the three regressors.
> 2. Take the first 20 examples. Find out their predictions using LinearRegression, 
> RandomForestRegressor, and Gradient BoostingRegressor.
> 3. Plot the three y-values for each of these 20 examples. Use the following code 
> for plotting.

plt.figure()
plt.plot(pred1, "gd", label="Gradient BoostingRegressor")
plt.plot(pred2, "b", label="RandomForestRegressor") plt.plot(pred3, "ys", label="Linear Regression")
plt.tick_params(axis="x", which "both", bottom-False, top-False,

labelbottom=False) 
plt.ylabel("predicted")
plt.xlabel("training samples")

Please submit both the code as well all the output.
