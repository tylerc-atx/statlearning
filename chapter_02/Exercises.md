
# 2.4 Exercises

---

## 1

a ) BETTER: A flexible method will work because the large sample size allows it to fit many observations

b ) WORSE: A inflexible method will work the best since there are not enough observations to fully define the variation and prevent overfitting

c ) BETTER: A flexible method will work best due to the nature of the response variable (more degrees of freedom)

d ) WORSE: The variance will cause a flexible method to chase the error, so a inflexible method will work best.

---


## 2

a ) Regression (Salary), Inference (Find Factors)  
    n = 500 firms   
    p = 3, profit, # employees, industry  

b ) Classification (Success/Failure), Prediction (New product)  
    n = 20 similar products   
    p = 13, success, price, marketing budget, competition price, 10 other  
    
c ) Regression (% Change), Prediction  
    n = 52 weeks in 2012    
    p = 4, delta% dollar, delta% USmarket, delta% UKmarket, delta% DEmarket  


---

## 3

a )   
![figure 3a](https://raw.githubusercontent.com/tylerc-atx/statlearning/master/chapter_02/3_a_fig.jpg)

b )   
**Irreducible Error:** The irreducible error is inherent in the variation of the data and cannot be reduced further. It is some constant value of error on the y-axis.  

**Bias Squared:** Bias squared is the error between the model function and the true underlying function. It is reduced monotonically as the estimated function fits the data more closely to the true function.  

**Variance:** Variance is the variation in the training data that is not part of the underlying function. Variation constantly increases monotonically as flexiblity increases since the model will 'chase' the data more closely. Too much variation results in an overfit model.

**Training Error:** Training error reduces monotonically as flexibilty increases due to decreasing bias. However, overfitting the model will cause the model to 'chase' the variance in training data and overfit it; reducing the training error below the irreducible error.

**Test Error:** Test error initially decreases as bias falls when the model is fit. As the model is overfit, the variation increases will cause the test error to increase.

---

## 4

a )  

**Brand of Beer Purchased**  
Response Variable: Type of Beer  
Predictors: Region, local income-level, type of store, brands carried  
Prediction  

**What majors do students from our HS study? What predictors influence their choice of major?**  
Response Variable: College Major  
Predictors: GPA, club membership, athletic activities, gender  
Inference  

**What dish will sell most at the new restaurant?**  
Response Variable: Dish  
Predictors: Location, demographics, dishes offered  
Prediction  

b )

**What influences sales of our laptop product line?**  
Response Variable: Number of sales  
Predictors: Consumer segment, time of year, marketing budget  
Inference

**What MPG will the new car design get?**  
Response Variable: MPG  
Predictors: Cylinders, weight, 2x2 vs 4x4  
Prediction  

**GPA of student based on hobbies**  
Response Variable: GPA  
Predictors: hobbie types  
Prediction  

c ) 

**Market segments for a company's customers**  
**Social media influencer's follower types**  
**Characteristics of various web traffic types in our datacenter**  

---

## 5

A very flexible approach will fit the training data more closely, particularly for non-linear relationships where a linear approach would not eliminate as much bias. However, a very flexible approach can introduce variation if it is overfit, and requires more data to train.    

A more flexible approach is typically better for prediction purposes.

A less flexible approach is preferred for drawing inference about the relationship between the predictors and response. (higher interpretability)

---

## 6

A parametric approach creates a model that has parameters assigned to each predictor. A nonparametric approach is typically more flexible and will not assume a functional form to data.

A parametric approach has the advantage of being more interpretable. However, it cannot fit data that has alot of variation and degrees of freedom.  A parametric approach also requires less observations to fit.

---

## 7

|Obs|$X_1$|$X_2$|$X_3$|Y|
|---|---|---|---|---|
|1|0|3|0|Red|
|2|2|0|0|Red|
|3|0|1|3|Red|
|4|0|1|2|Green|
|5|-1|0|1|Green|
|6|1|1|1|Red|


a )  

|Obs|Distance|
|---|---|
|1|3|
|2|2|
|3|3.2|
|4|2.2|
|5|1.4|
|6|1.7|

b )  

Green is the K = 1 closest to (0, 0, 0)  

c )  

Red. 2/3 of the K = 3 closest neighbors are red for (0, 0, 0)

d )   

If the decision boundary is nonlinear, then a smaller K would be preferable. A smaller K will chase the data more closely and define the non-linear relationship. Smaller K is typically more flexible and has lower bias. Smaller K prediction use less points to make a decision than large ones.

