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

![Screenshot (67)](https://user-images.githubusercontent.com/58145503/96093796-376da200-0eea-11eb-84d4-9f77a4626205.png)
![Screenshot (68)](https://user-images.githubusercontent.com/58145503/96093804-39cffc00-0eea-11eb-9db2-6c8fe7be35e5.png)
![Screenshot (69)](https://user-images.githubusercontent.com/58145503/96093813-3a689280-0eea-11eb-945d-cb3de278604c.png)
![Screenshot (72)](https://user-images.githubusercontent.com/58145503/96093816-3b012900-0eea-11eb-8622-1e58ee6e898b.png)
![Screenshot (73)](https://user-images.githubusercontent.com/58145503/96093819-3b99bf80-0eea-11eb-93d7-d693ad19d72b.png)
![Screenshot (74)](https://user-images.githubusercontent.com/58145503/96093823-3ccaec80-0eea-11eb-9095-6e5d73dc4cb9.png)
![Screenshot (75)](https://user-images.githubusercontent.com/58145503/96093825-3d638300-0eea-11eb-8c0f-4338b8731d3c.png)
![Screenshot (76)](https://user-images.githubusercontent.com/58145503/96093827-3dfc1980-0eea-11eb-96bf-50e81ebbfb2e.png)
![Screenshot (77)](https://user-images.githubusercontent.com/58145503/96093831-3f2d4680-0eea-11eb-8aa9-9a557f9f18d0.png)
![Screenshot (78)](https://user-images.githubusercontent.com/58145503/96093838-3fc5dd00-0eea-11eb-88e6-941d6ac4c0ee.png)
![Screenshot (79)](https://user-images.githubusercontent.com/58145503/96093842-40f70a00-0eea-11eb-8326-f6c613298766.png)
![Screenshot (80)](https://user-images.githubusercontent.com/58145503/96093846-42283700-0eea-11eb-8909-6576d55563f3.png)
![Screenshot (81)](https://user-images.githubusercontent.com/58145503/96093850-42c0cd80-0eea-11eb-9d8e-087e585b6d7a.png)
![Screenshot (82)](https://user-images.githubusercontent.com/58145503/96093856-43f1fa80-0eea-11eb-8d89-a79f48be88ad.png)
![Screenshot (48)](https://user-images.githubusercontent.com/58145503/96093862-45232780-0eea-11eb-9218-b298b3bf99e6.png)
![Screenshot (53)](https://user-images.githubusercontent.com/58145503/96093866-45bbbe00-0eea-11eb-8429-745580b8e540.png)
![Screenshot (55)](https://user-images.githubusercontent.com/58145503/96093870-46545480-0eea-11eb-9af1-31b3f9aad8f1.png)
![Screenshot (56)](https://user-images.githubusercontent.com/58145503/96093872-47858180-0eea-11eb-9ee0-98d73d3b4b4a.png)
![Screenshot (58)](https://user-images.githubusercontent.com/58145503/96093875-48b6ae80-0eea-11eb-99d6-d0b4eaba40f4.png)
![Screenshot (59)](https://user-images.githubusercontent.com/58145503/96093876-494f4500-0eea-11eb-9507-91d5472b8dfb.png)
![Screenshot (62)](https://user-images.githubusercontent.com/58145503/96093881-4a807200-0eea-11eb-84a9-425421958732.png)
![Screenshot (64)](https://user-images.githubusercontent.com/58145503/96093888-4ce2cc00-0eea-11eb-97af-709f0b5492d7.png)
![Screenshot (65)](https://user-images.githubusercontent.com/58145503/96093892-4d7b6280-0eea-11eb-8037-f4f024619a08.png)


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
