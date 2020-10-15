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

![Screenshot (58)](https://user-images.githubusercontent.com/58145503/96094265-c975aa80-0eea-11eb-89fe-ebd9fe627902.png)
This even better!!

![Screenshot (59)](https://user-images.githubusercontent.com/58145503/96094257-c8447d80-0eea-11eb-8913-ffd7d6efe4ad.png)
But what if we go on roatating?? again the errror value is increased. 

There is a sweetline between horizontal and vertical line. That is called the **best fit line**

![Screenshot (62)](https://user-images.githubusercontent.com/58145503/96095067-be6f4a00-0eeb-11eb-96f0-fd06d8512ab3.png)
![Screenshot (64)](https://user-images.githubusercontent.com/58145503/96095251-042c1280-0eec-11eb-9195-f179915c5c81.png)
![Screenshot (65)](https://user-images.githubusercontent.com/58145503/96095259-05f5d600-0eec-11eb-84bc-1aeedb8bad3c.png)

__How do we find least sum of squared residual by rotating each line??__
![Screenshot (67)](https://user-images.githubusercontent.com/58145503/96095265-07270300-0eec-11eb-8fbe-54dae1ec2ab3.png)

we take derivates of each resudial and these derivates tell us slope and intercept of each sum of residual.
![Screenshot (68)](https://user-images.githubusercontent.com/58145503/96095945-e7dca580-0eec-11eb-8285-0c619af43261.png)
![Screenshot (69)](https://user-images.githubusercontent.com/58145503/96095947-e9a66900-0eec-11eb-8f1c-0641d1628308.png)
![Screenshot (72)](https://user-images.githubusercontent.com/58145503/96095949-ead79600-0eec-11eb-83d969e905a81d8a.png)
![Screenshot (73)](https://user-images.githubusercontent.com/58145503/96095951-eb702c80-0eec-11eb-8e36-0df436d47458.png)
 
 we can curves of sum of square residuals by taking slope and intercept of each line and find the optimal curve for residuals
![Screenshot (78)](https://user-images.githubusercontent.com/58145503/96096372-68030b00-0eed-11eb-8cc4-fae68694cf6f.png)
![Screenshot (74)](https://user-images.githubusercontent.com/58145503/96096375-69ccce80-0eed-11eb-903f-71ef5bf76237.png)
![Screenshot (75)](https://user-images.githubusercontent.com/58145503/96096377-6a656500-0eed-11eb-9c26-65ddf5ba5eab.png)
![Screenshot (76)](https://user-images.githubusercontent.com/58145503/96096380-6afdfb80-0eed-11eb-9679-3526389b51d2.png)
![Screenshot (77)](https://user-images.githubusercontent.com/58145503/96096386-6b969200-0eed-11eb-993423dfd384389e.png)

**There are three big important concepts in linear regression**
![Screenshot (80)](https://user-images.githubusercontent.com/58145503/96096664-b4e6e180-0eed-11eb-8f76-7952551119d6.png)
![Screenshot (82)](https://user-images.githubusercontent.com/58145503/96096675-b6b0a500-0eed-11eb-834f-5d7b426126ca.png)
![Screenshot (79)](https://user-images.githubusercontent.com/58145503/96096677-b7493b80-0eed-11eb-9f9c-f03876f04319.png)


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
