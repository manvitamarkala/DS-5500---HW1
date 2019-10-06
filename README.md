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

Figure 3 depicts that Europe is the country with the largest income followed by Asia and then Americas and Africa.For a course of a few years during the end 90's asia has crossed Europe in terms of the income. Africa has always remained the lowest income continent and the growth over years is also very flat.Until 1960, Asia remained below Americas and Europe and then increased to a great extent after.


![Europe[]{label="fig:Europe"}](Europe.png)
###### Figure 4: Income/person across different countries in Europe over the years

Figure 4 depicts that the most major contribution for Europe's income comes from 


