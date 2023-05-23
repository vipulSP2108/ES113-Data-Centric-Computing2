# Problem 

In this problem, we will see how to use Leave-One-Out-Cross-validation (LOOCV) as a way to
detect outliers in the data in a simple setting.

Create a dataset of 100 points for regression using the following piece of code.
Each point X(i) will be generated as a 5 dimensional Gaussian random vector. 
  X[i]= random.randn(5)

Define w= [0.2, 0.3, 0.4, 0.5, 0.6]. Then define the target Y(i) as

Y(i) = w*X(i) + random.randn()

The * is a dot product.

Now add in a single point as an outlier. Choose a random index between 0 to 100 and modify
the target Y(i) for that point.

outlierindex= int(random.random()*50) 
Y(outlierindex)=wX(i)+ 10 random.randn()

Notice that it is not known to us which point is an outlier. Now do Linear Regression with 
LOOCV and find out which point has the worst error. Return the index of that point as the 
potential outlier. Compare it with the above outlierindex to see whether you have identified 
it correctly.

Now do the same where you have 5 outliers, inserted into the data in the same way as before. Are you able to identify them in the same manner? Report how many you are able to identify. Note that this may or may not work -to work it needs a modification to the above method that we have not studied.
