# Simple-linear-regression-Indepth-

# Model Evaluation techniques for Regression
To find which is a better model in regression,there are many regression techniques, here we are some most commonly used evaluation metrics in machine learning
1.R-Squared
2.MSE (Mean Squared Error)
3.RMSE (Root Mean Squared Error )

**1. R – Squared**
It is also called as coefficient determination. If the R-square value is low then our model is bad. If R -square value is high then our model is good. It is a range between 0 to 1

R2  = 1 - SSresidual / SStotal  
SStotal = 1/n Σ(yi - ypred_mean)2 
SSresidual =  1/n Σ(yi - ypred)2         #SS - Sum of Squares

SSresidual = 0 then R2 = 1 ; machine learning model is good.
SStotal> SSresidual ; R2 lies in between 0 to 1.
SStotal= SSresidual ; R2 =0 is a simply mean model.
SStotal < SSresidual ; R2 is negative. so our machine learning model is worst.

**2. MSE (Mean Squared Error)**
Mean Squared Error is a technique to compute errors in regression machine learning models. It is very simple to compute and interpretable. we calculate the sum of squares of errors of model predictions.

MSE =  1/n Σ(yi - ypred)2 
Always errors or loss must be near to zero. so If MSE is high our model is worst, If MSE is low our model is good. check more about MSE here

**3. RMSE ( Root Mean Squared Error)**
It is simply the root of MSE. If RMSE is high our model is worst, If RMSE is low our model is good.

RMSE =  Root( 1/n Σ(yi - ypred)2 )
some other model evaluation techniques for Regression are out there. You can check it them also through google. But these are commonly used model evaluation techniques for regression.
