# Simple-linear-regression-Indepth

## Fitting a line to data aka Least squares

![Screenshot (48)](https://user-images.githubusercontent.com/58145503/96085261-2f0f6a00-0ede-11eb-8dc4-236d7d94eff6.png)

Now, how can you determine that which is the best fit line for that data???

so, we can measure how well this line fits the data by seeing how close it is to the data points 

![Screenshot (55)](https://user-images.githubusercontent.com/58145503/96086836-86163e80-0ee0-11eb-86b7-f44e60df3b6e.png)

For example, Here I have taken horizontal line to calculate to residuals. 
* note: If there are points above the line those are negative values so we take square of the differnce to avoid negative values. This is called the total sum of squared residuals and we got 24.62

what it we rotate the line downwards and calculate the residuals?? can it reduce total sum of squares?? The answer is yes!!!

![Screenshot (56)](https://user-images.githubusercontent.com/58145503/96087401-6a5f6800-0ee1-11eb-80f8-30b2d5c5fac2.png)
By rotating the I can able to reduce the error and it is better than before. But how much should I rotate??


## Model Evaluation techniques for Regression
To find which is a better model in regression,there are many regression techniques, here we are some most commonly used evaluation metrics in machine learning
1.R-Squared
2.MSE (Mean Squared Error)
3.RMSE (Root Mean Squared Error )

**1. R – Squared**
It is also called as coefficient determination. If the R-square value is low then our model is bad. If R -square value is high then our model is good. It is a range between 0 to 1

* R2  = 1 - SSresidual / SStotal 
* SStotal = 1/n Σ(yi - ypred_mean)2 
* SSresidual =  1/n Σ(yi - ypred)2         *SS - Sum of Squares*

- SSresidual = 0 then R2 = 1 ; machine learning model is good.
- SStotal> SSresidual ; R2 lies in between 0 to 1.
- SStotal= SSresidual ; R2 =0 is a simply mean model.
- SStotal < SSresidual ; R2 is negative. so our machine learning model is worst.

**2. MSE (Mean Squared Error)**
Mean Squared Error is a technique to compute errors in regression machine learning models. It is very simple to compute and interpretable. we calculate the sum of squares of errors of model predictions.

MSE =  1/n Σ(yi - ypred)2 
> Always errors or loss must be near to zero. so If MSE is high our model is worst, If MSE is low our model is good. check more about MSE here

**3. RMSE ( Root Mean Squared Error)**
It is simply the root of MSE. If RMSE is high our model is worst, If RMSE is low our model is good.

RMSE =  Root( 1/n Σ(yi - ypred)2)

> some other model evaluation techniques for Regression are out there. You can check it them also through google. But these are commonly used model evaluation techniques for regression
