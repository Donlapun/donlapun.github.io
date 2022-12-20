---
name: Billionaire Project
tools: [Python, HTML, vega-lite, JavaScript]
image: assets/pngs/cars.png
description: What factors we shoudl thin kabout when it comes to Billionaires?
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Billionaire Status, Wealth Size, and Location from 1996-2014

In this project we will explore the Billionaire Dataset to find the meaning insights such as the association of different factors that might influence the wealth worth of the billionaires and shows in the visualizations as the findings with the writeup. The information about the dataset can be founded a the the end of the page.

## Data Citation: 
Ryan Whitcomb. CORGIS Datasets Project. ![https://think.cs.vt.edu/corgis/csv/billionaires/](https://think.cs.vt.edu/corgis/csv/billionaires/). Accessed 1 Dec. 2022.

## Team Member:
1. Donlapun (Dorothy) Wongkarnta
2. Riya Shah 
3. Ethan Wee

# Interactive Visualization 

## Interactive Visualization between the Line Graph of the Wealth Worth in Billions by Year Company Founded and the count of the Year Company Founded

#graphhh

The graph on the left is the line graph between the year company is founded in and the wealth worth in billions. 
The user can select the interval of the graph in order to see the histogram that shows the count of the year (in interval). 
We can see that there is an positive association between the year company is founded and the wealth worth in billions after 1500. 
The histogram shows the distribution of those years in more depth as it counts the how many companies are in each year. 
This helps us understand that even though there is an association between the year company is founded and the wealth worth in billions after 1500, 
the number of new companies that founded in each year does not have influence on the wealth worth in billions.

## Interactive Visualization between the Scatter Plot between the Demographics Age and Wealth Worth in Billions of the Billionaires and Histogram of the Location Region of the Billionaire Company

This interactive visualization shows the relationship between a billionaire’s demographic age and wealth worth and the region they are from. The user can select an age on the demographics age chart and the region bar graph will update accordingly, showing the number of billionaires at that age for each region. From this visualization, we can interpret that most billionaires are 50 years old or above. We can also interpret that as the age increases, a lot of billionaires are from North America, but there are also a good number of billionaires from Europe and South Asia. There is not a clear association between a billionaire’s age, wealth worth, and the region they are from, but it helps in providing context about the overall age of billionaires in different regions.

# Contextual Visualization

## Histogram of Billionaire by Gender

![]()
 
This image shows a breakdown of Billionaires’ wealth from across the world by the type of wealth they have. In this, we see that with technology billionaires, by far the largest amount of their assets is in public holdings, compared to real estate billionaires who’s largest asset type is actually private holdings. Interestingly, fully half of the share of wealth within industrial conglomerate billionaires are formed by public holdings. What this could suggest is that technology industry billionaires main source of wealth comes from their stock allocation, such as their salaries being paid for in shares of the public company they control. This makes sense as many tech CEO’s such as Elon Musk are often paid a base salary, with stock options used as incentives. This would result in CEO’s with high performing companies being compensated with valuable stock options.

### Histogram Citation:
Published by Statista Research Department, & 22, S. (2022, September 22). Billionaires: Breakdown of wealth by asset 2021. Statista. Retrieved December 2, 2022, from ![https://www.statista.com/statistics/299134/billionaires-breakdown-wealth/](https://www.statista.com/statistics/299134/billionaires-breakdown-wealth/)

## Scatter Plot of GDP per Capita by Country in 2022
![]()

This visualization provides further context to the billionaires dataset. From this chart we can see the total GDP per capita for each country during 2022. This can be used to compare the 2016 GDP in the dataset and further understand the relationship between a billionaire’s country and the GDP. It can help determine if a billionaire’s country of origin and GDP plays a factor in their status or net worth. An interesting point about this visualization is that the top three countries with the highest GDP are Singapore, Luxembourg, and Ireland instead of United States, considering a lot of billionaires are from the United States. This suggests that a country’s GDP might not be a factor in achieving billionaire status and provides a new perspective when conducting analysis.

### Scatter Plot Citation:
World Population Review. GDP per Capita by Country 2022. ![https://worldpopulationreview.com/country-rankings/gdp-per-capita-by-country](https://worldpopulationreview.com/country-rankings/gdp-per-capita-by-country). Accessed 2 Dec. 2022.


## Additional Citation:
### Interactive Visualizations:
Used code from class
- [Week 9](https://starboard.gg/jnaiman/inClass_week09_online_fall2022-noY2U59)
- [Week 10](https://starboard.gg/jnaiman/inClass_week10_online_fall2022-nrSZM7g)
### Contextual Visualizations
Histogram
Made by the team using [Python](https://starboard.gg/rshah257/IS445-final-project-python-nxupkrI)



<div class="left">
{% include elements/button.html link="https://think.cs.vt.edu/corgis/csv/billionaires/" text="Billionaire Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://starboard.gg/fahdonlapun/final_project_3.1-n0vrN1h" text="The Analysis" %}
</div>

<div class="left">
{% include elements/button.html link="https://www.statista.com/statistics/299134/billionaires-breakdown-wealth/" text="Billionaire BreakDown Data" %}
</div>

<div class="left">
{% include elements/button.html link="https://worldpopulationreview.com/country-rankings/gdp-per-capita-by-country" text="GDP Data" %}
</div>

