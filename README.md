# NBA-Players-Salary-Prediction
Predicting NBA Player's salary using various machine learning algorithms like linear regression (Ridge, Lasso,PCA,PCR), Random Forest, Bagging, Boosting and Neural Networks using R 

## Project Title:

NBA (National Basketball Association) Player's Salary Prediction

## Motivation:
At the beginning of each season, when the salaries of pro athletes are publicized, we're always left wondering: How much each player is making? 
Let's use our machine learning skills to come to decide the driving factors to determine player's salary. 
Here, I am using various models to compare their accuracy to solve this a bit complex problem


## Data Source:

https://www.basketball-reference.com/leagues/NBA_2018_advanced.html


## Analysis Steps:

- Exploratory Data Analysis
- Models Explored:
1. Linear model
    a. Multivariant Linear Model
    b. Ridge Regression
    c. Lasso Regression
    d. Principle Component Analysis
    e. Principle Component Regression
2. Random Forest
3. Bagging 
4. Boosting
5. Neural Networks
6. Clustering + Regression


## Findings:

- With almost all the models except neural networks, the RMSE (Root Mean Square Error) of ~ $5.2Mn was obtained with ~ 58%. Even after introducing non-linearity and interactions in the linear models, variable reduction (PCA) and with ensemble (random forest). 
- However, with single layer neural nets, RMSE of 617K was obtained.

So, what did we do next?

We tried to work around it by clustering the players into different segments based on their performance parameters, which indirectly drive their salary (because salary would be unknown for the test dataset). However, the dataset only contains 550 players and due to smaller sample size, the clusters did not converge well. 

## Conclusion:

Well, the results are quite obvious!

- The salary distribution is quite skewed for NBA players. Only 4% of the players get paid very high salary (> $20Mn)
- Due to the salary cap of the players, the error is always going to be very high. No model will be able to predict player's salary accurately.

Remember, 

"All models are wrong, but some are useful" - George Box

And in our case, neural networks tunrned out to be a bit useful!

