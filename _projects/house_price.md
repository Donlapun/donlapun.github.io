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
