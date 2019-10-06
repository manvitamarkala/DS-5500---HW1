# Homework 1 Solutions 

## Problem 1

The question I chose from the Gapminder test is : The United Nations predicts that by 2100 the world population will have increased by another 4 billion people. What is the main reason?

I first started looking into the the overall pattern of the total population across different years predicted until 2100, because the 4 billion increase statistics was itself very fascinating for me.

I took the individual age groups files with year, geo and population and then performed data transformations by concatenation and group-by to get a single dataframe giving total population and splits by different age groups across years summed up by geos.

The total population across years is represented by Figure 1 where they have predicted that the total population will be around 11 billion by 2100 and is roughly around 7 billion in 2019.

![World population census[]{label="fig:worldpopulation"}](worldpopulation.png)
###### Figure 1: World population as predicted by United Nations


After this, I wanted to check the contribution of individual age groups towards this population over years and and see if there is shift within age groups and what are the major contributors.

![Proportion Split[]{label="fig:proportionsplit"}](ProportionSplit.png)
###### Figure 2: Proportion of population split by age groups

Figure 2 indicates that the major contributors of population every year are groups 20-59 (20-39, 40-59). But as years are passing by since the average life span is increasing, 60-plus age groups proportion shows an increase and its adjusted by 20-39 group. But still at an overall level the majority contribution comes from 20-59.

The answer for the question is that age groups 15-75 are the major contributors for that population increase because of the combined affect of population 20-59 being dominant and also the increasing population in age groups 60-plus.

## Problem 2

For the visualisation of income across time, I have considered the following excel workbook for income - ddf--datapoints--income_per_person_gdppercapita_ppp_inflation_adjusted--by--geo--time.csv. I have taken the geological information from ddf--entities--geo--country.csv

I have combined the two data sources by geo and formed a single dataframe. After that, I plotted graphs for income/person over time by continent and also the country split per continent in seperate graphs.

![Continents income[]{label="fig:ContinentsIncome"}](ContinentsIncome.png)
###### Figure 3: Income/person across continents over the years

Figure 3 depicts that Europe is the country with the largest income followed by Asia and then Americas and Africa.For a course of a few years during the end 1900's Asia has crossed Europe in terms of the income. Africa has always remained the lowest income continent and the growth over years is also very flat.Until 1960, Asia remained below Americas and Europe and then increased to a great extent after.
A deep dive into country wise split will help us understand which countries in the continent are the major contributors for this income/person.


![Europe[]{label="fig:Europe"}](Europe.png)
###### Figure 4: Income/person across different countries in Europe over the years

Figure 4 depicts that the most major contribution for Europe's income comes fro its country France.

![Asia[]{label="fig:Asia"}](Asia.png)
###### Figure 5: Income/person across different countries in Asia over the years

Figure 5 shows very peculiar trends for the income/person for countries in Asia. Most of the arab countries like Kuwait, Qatar, United Arab Emirates have shown high peaks and drops after 1960 and are following different trends per different years. They have shown higher income/person than countries compared to Europe during the late 1900's.

![Americas[]{label="fig:Americas"}](Americas.png)
###### Figure 6: Income/person across different countries in Americas over the years

Figure 6 depics that United States followed by Canada are the biggest contributors for income/person in Americas and they show a constant increase across years except a for a very few dips in a few years

![Africa[]{label="fig:Africa"}](Africa.png)
###### Figure 7: Income/person across different countries in Africa over the years

The per capita GDP in Africa is now less than it was in 1974, having declined over 11 percent. Few of the countries were higher in previous years and have been showing a decline in income/person as we progress through the years

## Problem 3

For this question I have taken data from income - ddf--datapoints--income_per_person_gdppercapita_ppp_inflation_adjusted--by--geo--time.csv, ddf--datapoints--life_expectancy_years--by--geo--time.csv and ddf--datapoints--number_of_child_deaths--by--geo--time and the geo information is taken from ddf--entities--geo--country.csv. 

I have performed data transformations and concatenated income/person, life expectancy and child births for every continent across all years

For the first plot in Figure 8, I have plotted income/person across different continents across different years.Figure 3 depicts that Europe is the country with the largest income followed by Asia and then Americas and Africa.For a course of a few years during the end 1900's Asia has crossed Europe in terms of the income. Africa has always remained the lowest income continent and the growth over years is also very flat.Until 1960, Asia remained below Americas and Europe and then increased to a great extent after.

![Continents income[]{label="fig:ContinentsIncome"}](ContinentsIncome.png)
###### Figure 8: Income/person across continents over the years

For the graph in figure 9, I have plotted life expectancy across different continents across different years.The life expectancy for all the continents have dropped roughly around 1920( most likely could be a data issue). Europe has the highest life expectancy followed by Americas, then Asia and Africa. Based on the different living conditions of these continents, one of the inferences that can be deduced is hygiene, pollution are the major contributors for long life span expectancies.

![Continents Life expectancy[]{label="fig:LifeExpectancy"}](LifeExpectancy.png)
###### Figure 9: Life Expectancy across continents over the years

For the graph in figure 10, I have plotted total number of child deaths across different continents across different years. Asia has the highest number of child deaths until very recently after which Africa has started to increase in the total number of child deaths and has crossed Asia.The infant and child mortality rate has declined remarkably in most countries since 1950.A new study says that children in sub-Saharan Africa are more than 15 times more likely to die before the age of 5 than children in high income countries. Americas has always been the least in terms of child deaths across all years.

![Child deaths[]{label="fig:ChildDeaths"}](ChildDeaths.png)
###### Figure 10: Child deaths across continents over the years

To draw a comparison between life expectancy, income and child deaths across years, I have grouped by continents and calculated the aggregates and represented in figure 11.

![Comparison[]{label="fig:Comparison"}](Comparison.png)
###### Figure 11: Life expectancy, income and child deaths over the years

Figure 11 depicts a positive relationship between income and life expectancy and they have been increasing with years and they have shown a negative relationship with child deaths as child deaths have been decreasing across years. This is a very positive sign for the world trends. Due to the advancements in medicine and genetics, the life span for human beings is increasing and child deaths decreasing which in tern increase the income/person.


## Problem 4

Firstly I have tried to check the relationship between breast cancer deaths of female and the female life expectancy acoss different continents in a particular year ( here :2012). I have taken the data from ddf--datapoints--breast_cancer_number_of_female_deaths--by--geo--time.csv and ddf--datapoints--life_expectancy_female--by--geo--time and performed transformations and grouping

![2012[]{label="fig:2012"}](2012.png)
###### Figure 12: Breast cancer deaths vs life expectancy for females in 2012

Figure 12 shows that Africa has the least life expectancy for females but also the cases for breast cancers is relatively low and the reason for shorter life spans could be other reasons like healthcare, sanitation etc. Asia and Europe potray larger cases for deaths due to breast cancer even with moderate and higher life expectancy. Among European countries, Russia and Germany show high numbers. In Asia, its India and China and the Americas has United states with large cases for breast cancer deaths. In Africa, countries like Nigeria and South Africa have high cases.


I also wanted to check how the number of breast cancer cases and average life expectancy has changed over the years at an overall level.

![Trend_females[]{label="fig:trend_females"}](trend_females.png)
###### Figure 13: Trend for breast cancer deaths and life expectancy for females

Figure 13 shows that even if there is a positive increase in the life expectancy for females, the breast cancer deaths have increased too. Breast cancer deaths have been an increasing problem recently among women and there needs to be proper caution and medication to avoid it and further increase the life span for female population

## Problem 5

I have used static plot to answer all of the previous problems so far.

Advantages of Interactive Visualisations when compared to Static Visualisations:

1) The visuals are more appealing and easier to understand when more number of variables come into picture. If there are multiple variables that need to be compared across different dimensions, static visualisation makes the graph less understandable.

2) Interactive Visualizations can be built so that all users, regardless of disability status, can access the information easily.

3) Identifying trends to find out root causes and depicting a story out of complex data gets easier with interactive visualisations

Disadvantages:

1) Static visualisations can just be exported as images and printed out and be able to access

2) Building statis visualization takes much lesser time and money when compared to Interactive Visualizations.

3) Trying to build a complicated dynamic visualisation can lead to confusion if the visuals of the metrics to be displayed and the kind of charts to be used are not well known.

4) Static visualisations are also easy to build and construct with basic libraries under any computing language

I think the difference between which visualisation should be consumed depends on a number of factors that include time, resources, the end target customers who are going to utilize this data ( Some customers prefer static whereas some want visually appealing results), data ( how complex the data is? We do not want to spend a lot of time on visualisation if the dataset is simple enough) etc.

While solving some of the previous problems in the assignment, I realised that a few of these problems can be simply answered with static graphs whereas a few of them needed good dynamic visualizations to be able to tell a story.
