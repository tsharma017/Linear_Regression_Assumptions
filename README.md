# Linear_Regression_Assumptions

Linear regression relies on several key assumptions to ensure that its estimates are reliable and that inference (like confidence intervals and hypothesis tests) is valid. Here’s a breakdown of the main assumptions:

1. Linearity
What It Means:
The relationship between the independent variables (predictors) and the dependent variable (target) should be linear. This means that the effect of a one-unit change in a predictor is constant, regardless of the level of that predictor.
How to Check:
Scatter plots of the predictor versus the outcome and residual plots can help assess linearity.

2. Independence of Errors
What It Means:
The residuals (errors) should be independent of each other. In other words, the error of one observation should not influence the error of another.
How to Check:
This is particularly important in time series data where errors can be correlated (autocorrelation). The Durbin-Watson statistic is a common test to check for autocorrelation.


3. Homoscedasticity
What It Means:
The residuals should have constant variance across all levels of the independent variables. If the spread of the residuals increases or decreases with the level of a predictor, this is called heteroscedasticity.
How to Check:
Plotting the residuals versus fitted values can reveal patterns—ideally, the spread should look like a horizontal band.

4. Normality of Errors
What It Means:
The residuals are assumed to be normally distributed. This assumption is crucial for conducting hypothesis tests and building confidence intervals.
How to Check:
Histograms, Q-Q plots of the residuals, or statistical tests like the Shapiro-Wilk test can help assess normality.


5. No (or Little) Multicollinearity
What It Means:
The independent variables should not be too highly correlated with each other. High multicollinearity can inflate the variances of the parameter estimates, making them unstable.
How to Check:
Variance Inflation Factor (VIF) is a common metric used to assess multicollinearity. VIF values above 5 or 10 (depending on the context) might indicate problematic collinearity.


6. No Influential Outliers
What It Means:
No single data point should unduly influence the model. Outliers or influential points can distort the regression estimates.
How to Check:
Diagnostic measures such as Cook’s distance, leverage statistics, and studentized residuals help identify such influential observations.
