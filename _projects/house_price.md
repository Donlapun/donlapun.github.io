---
name: Ames House Price Prediction
tools: [Python, HTML, vega-lite, JavaScript]
image: assets/pngs/scatter_billionaire.png
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
We conduct the hypothesis test as following:

$H_0 :  \mu_1 - \mu_2 = 0$

$H_1 :  \mu_1 - \mu_2 \neq 0$

 where 
 $\mu_1$ is the average year built value for residential homes that has central air condition.
 
 $\mu_2$ is the average year built value for residential homes that doesn't has central air condition.
 
 (All hypothesis conditions are met.)
