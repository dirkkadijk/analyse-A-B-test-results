# Analyze-A-B-Test-Results

A/B tests are very commonly performed by data analysts and data scientists. It is important to get some practice working with the difficulties of these.

For this project, you will be working to understand the results of an A/B test run by an e-commerce website. The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. Your goal is to work through this notebook to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

## Table of Contents
- Introduction
- Part I - Probability
- Part II - A/B Test
- Part III - Regression

## Part I - Probabilities

Calculation of conversion rates per Hypothesis scenario (without and with treatment page).

Outcome: A minor 1.3% **lower** conversion rate of the new treatment page suggests that there is NOT sufficient evidence to say that the new treatment page leads to **more** conversions.


## Part II - A/B Test

Let's recap the steps we took to analyze the results of this A/B test.
1.	We computed the observed difference between the metric, click through rate, for the control and experiment group.
2.	We simulated the sampling distribution for the difference in proportions (or difference in click through rates).
3.	We used this sampling distribution to simulate the distribution under the null hypothesis, by creating a random normal distribution centered at 0 with the same spread and size.
4.	We computed the p-value by finding the proportion of values in the null distribution that were greater than our observed difference.
5.	We used this p-value to determine the statistical significance of our observed difference. 


We used Z-score which is a measure of how many standard deviations below or above the population mean a raw score is.



## Part III - Regressions

We use statsmodels to fit a logistic regression model.

First we looked at the individual factors of country and page on conversion, then we looked at an interaction between page and country to see if there significant effects on conversion.


