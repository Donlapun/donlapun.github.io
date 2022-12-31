---
name: Ames House Price Prediction
tools: [Python, HTML, vega-lite, JavaScript]
image: assets/pngs/mon_price_qual_plot.png
description: Price predictive modeling according to house recommendations
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Team member
1. Donlapun Wongkarnta
2. Yunfan Hu


# Data Set

# Motivation
Supoosed that you are a residential house hunter who finds a house for client that just move to Ames, Iowa. Normally, you client usually have specific preference towards a residential home and the preferred price they want. Many customers usually request a house with central air coniditoning. Therefore, You want to know more how the residential house market in Ames, Iowa is like before you promote houses to your customers.

# Research Questions
1. What is the relationship between the Month Sold(Mo_Sold) and the Sale Price(price) in this Ames, Iwoa Housing Dataset(ames.csv)? And furthermore, how does this relationship between the Month Sold(Mo_Sold) and the Sale Price(price) change for different values of Overall Quality(Overall_Qual)?
2. Is there an association between the Central air condition(Central_Air) and the Year Built(Year_Built) in all residential homes in Ames, Iwoa?
3. Is there a linear relationship between the Sale Price(price) and the Overall Quality(Overall_Qual), the Condition of sale (Sale_Condition), the Central air condition(Central_Air), and the Year Built(Year_Built) in the sample? What about in the all residential homes in Ames, Iwoa?
4. Is there a linear relationship between the log-odds of the success level of the Central air condition(Central_Air) and the Year Built(Year_Built), the Size of Garage(Garage_Area), the Year Sold(Yr_Sold), and the Sale Price(price) in the sample? What about the all residential homes in Ames, Iwoa? What explanatory variables should we include in the model to build a parsimonious model?


## Q1: What is the relationship between the Month Sold(Mo_Sold) and the Sale Price(price) in this Ames, Iwoa Housing Dataset(ames.csv)? And furthermore, how does this relationship between the Month Sold(Mo_Sold) and the Sale Price(price) change for different values of Overall Quality(Overall_Qual)?

<vegachart schema-url="{{ site.baseurl }}/assets/json/month_price.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/qual_price.json" style="width: 100%"></vegachart>

![Month_price_Quality Plot](/assets/pngs/mon_price_qual_plot.png)


Based on the statistics summary, the compare measure of center in graph 2 and the intercept comparison in graph 3 indicates the positive relationship between house prcing and the overall quality. Measure of center and slope comparison show that most of the house pricing are not affected by which month it was sold. However, it is necessary to notice that house which has extreme high quality(10) is more likely to be sold in higher price in earlier months; conversely, house which has extreme low quality(1) is more likely to be sold in higher price in later months.

## Q2: Is there an association between the Central air condition(Central_Air) and the Year Built(Year_Built) in all residential homes in Ames, Iwoa?
We conduct the hypothesis test and calculate the p-value as following:

$H_0 :  \mu_1 - \mu_2 = 0$

$H_1 :  \mu_1 - \mu_2 \neq 0$

 where 
 $\mu_1$ is the average year built value for residential homes that has central air condition.
 
 $\mu_2$ is the average year built value for residential homes that doesn't has central air condition.
 
 (All hypothesis conditions are met.)
 
**Result:** p-value = 0
 
Since p-value = 0, we can suggest that we can reject the null hypothesis, which means that there is an association between the Central air condition(Central_Air) and the Year Built(Year_Built) in all residential homes in Ames, lwoa.

Since there is an association between the Central Air Conditioning(Central_Air) and the Year Built(Built) in all residential homes in Amer, Iowa. We would be able to estimate the approximate year that the houses start changing to have central air conditioning based on the year it is built.

*Further clarification can be found in the analysis*

## Q3: Is there a linear relationship between the Sale Price(price) and the Overall Quality(Overall_Qual), the Condition of sale (Sale_Condition), the Central air condition(Central_Air), and the Year Built(Year_Built) in the sample? What about in the all residential homes in Ames, Iwoa?

We create the Linear Regression Model to find the linear relationship between variables.

![Linear_model](/assets/pngs/linear_model_ames.png)

**Linear Regression Equation:** $\hat{price}$ = $-6.06*10^{5}$ - 6778.5689Sale_Condition[T.AdjLand] + $1.676*10^{4}$Sale_Condition[T.Alloca] -1315.9882 * Sale_Condition[T.Family] + 7645.4771 * Sale_Condition[T.Normal] + $3.038*10^{4}$Sale_Condition[T.Partial] + 4315.7593Central_Air[T.Y] + $3.991*10^{4}$Overall_Qual + 269.2409Year_Built

In order to satify more linear regression conditions, we transform the target by using log.

**New Linear Regression Model:** $\hat{ln(price)}$ = 10.3578 + 0.0516Sale_Condition[T.AdjLand] + 0.1210Sale_Condition[T.Alloca] + 0.0566Sale_Condition[T.Family] + 0.1197Sale_Condition[T.Normal] + 0.1990Sale_Condition[T.Partial] + 0.2271Central_Air[T.Y] + 0.2189Overall_Qual

After that we use inference to help identify which slopes should be non-zero. As the result, the slopes of Sale_Condition[T.Alloca], Sale_Condition[T.Normal], Sale_Condition[T.Partial], Central_Air[T.Y], and Overall_Qual have sufficient evidence to suggest that they are non-zero in the model.

This linear regression analysis helps us determine whether te Overall Quality(Overall_Qual), the COndition of Sale(Sale_Condition), the Central Air Conditioning(Central_air), and the Year Built(Year_Built) affects the Sale Price or not. From the analysis, we found that without the year built(Year_Built) variable, the model can explain more of the variability of the Sale Price(price). Therefore, considering these variables, there is a linear relationship between the Sale Price(price) and the Overall Quality(Overall_Qual), the Condition of sale (Sale_Condition), the Central air conditioning(Central_Air).

*Further clarification can be found in the analysis*

## Q4: Is there a linear relationship between the log-odds of the success level of the Central air condition(Central_Air) and the Year Built(Year_Built), the Size of Garage(Garage_Area), the Year Sold(Yr_Sold), and the Sale Price(price) in the sample? What about the all residential homes in Ames, Iwoa? What explanatory variables should we include in the model to build a parsimonious model?

We create the logistic regression to help answer thisquestion and use backward elimination to find the model with the lowest AIC score.
The model without Year Sold has the lowest AIC score

![Logistic_Model](/assets/pngs/logistic_regression_ames.png)
$\hat{numer\_air}$ = -71.3706 + 0.0356Year_Built + 0.0018Garage_Area + $3.051 * 10 ^ {- 5}$price

