# Country Level Analysis of Happiness and Peace with a focus on the Role of Female Heads of State

 ## Authors: 
 This project was authored by:
 
 -Syeda Naveera Fatima Rizvi (sr5752@nyu.edu) <br> 
 -Suniya Raza (sr5748@nyu.edu)  <br> 
 
The authors are students from the M.A Economics Program (Class of 2022) at the Graduate School of Arts and Sciences at New York University.

This project was prepared for the course ECONGA 4003: Data Skills for Computational Social Science which is a part of the [NYU Computational Social Science Program](https://css.as.nyu.edu) taught by Professors Thomas Sargent, Spencer Lyon and Chase Coleman.

## Project Overview and Business Understanding
In this project, Python was used to analyze the general happiness level and peace values of countries around the world. We analyzed the time trends of the average values of these indices for both the top and worse performing countries. A significant step in this project aims to see see whether countries who have a female head of state/government fare better on these indices than male led countries. 

## Programming Languages and Tools used

This project uses a combination of Exploratory Data Analysis and Linear Regression for the analysis. All code is in Python 

## Data Understanding and Source

* Data for Peace Index: This is a Global Peace Index measuring the peacefulness of a country. This index orginally ranges from 1-5, where lower values represent more peacefullness in a country. We have downloaded this dataset from the [vision of humanity website](https://www.visionofhumanity.org/). The downloaded dataset is provided as a supplementary file in this project and we simply read it for our analysis
   * This data has been produced by the Institute for Economics and Peace (IEP) under the guidance of an international panel of independent experts.


* Data for Happiness Index: This is a Cantril ladder Score which is meant to represent happiness or subjective well-being. Respondents are asked to imagine a ladder with steps numbered from 0 to 10. They are then asked to rate their current lives based on where they consider themselves to stand on the ladder, with step 0 is the worst possible life and step 10 is the best one. We download the data for the happiness index using an API request from the [World Happiness Report](https://www.worldhappiness.report/ed/2021/) published in the year 2021.
   * The World Happiness Report is a publication of the Sustainable Development Solutions Network, powered by data from the Gallup World poll and Lloyd’s Register Foundation, who provided access to the World Risk Poll. The 2021 Report includes data from the ICL-YouGov Behaviour Tracker as part of the COVID Data Hub from the Institute of Global Health Innovation


* Data for Female Head of States. This data lists female head of states and government who were appointed by a governing committee or parliament. It includes Presidents, Prime Ministers and Chancellors. The dataset includes the name of the countries these women mandated on as well as the start and end dates of the mandate. We scraped this data using Scrapy from the Wikipedia page for [List of elected and appointed female heads of state and government](https://en.wikipedia.org/wiki/List_of_elected_or_appointed_female_heads_of_state_or_government). The steps required to scrape the data are provided in the Appendix at the end of the Python Notebook

## Modelling and Evaluation

In this project we analyze the general happiness level and peace values of countries around the world. We analyze the time trends of the average values of this indices for both the top and worse performing countries. We do a special focus on Afghanistan where we see how major political events have impacted the happiness index values for this country. We also analyze the correlation between the happiness index and factors such as healthy life expectancy, log gdp per capita, social support, freedom to make life choices and perception of corruption. Finally we look at how geographical proximity plays a role in index values.

A significant step in this project aims to see see whether countries who have a female head of state/government fare better on these indices than male led countries. Following reports of how female-led countries such as New Zealand (Jacinda Ardern) and Germany (Angela Merkel) had a superior performance during the pandemic, we first focus on the year 2020. We see wether averages of the index values (both peace and happiness) differed by the gender of the head of state. We then extend our analysis to the entire 2008-2020 time period and check wether these differences have persisted across time. We also see what percentage of head of states were female in both the top and worst 10 countries (for peace and happiness seperately) in each year.

Please refer to the Raza_Rizvi_Happiness_and_Peace.ipynb file for

* The detailed analysis and report
* All code, tables and figures. 

## Key Insights

This report finds that individual time trends for average values of both peace and happiness show that low ranked countries tend to exhibit more volatility than high ranked countries. It also shows that there are infact gendered differences and female-led countries performed well not only during the pandemic year but also throughout the 2008-2020 time period

 
![Low_vs_High_Time_Trend](https://github.com/snaveerafrizvi/ECONGA4003_FINALPROJECT/blob/main/Low_vs_High_Time_Trend.png)

![Avg_Female_Vs_Male_Led](https://github.com/snaveerafrizvi/ECONGA4003_FINALPROJECT/blob/main/Avg_Female_Vs_Male_Led.png)

![time_trend_avg](https://github.com/snaveerafrizvi/ECONGA4003_FINALPROJECT/blob/main/time_trend_avg.png)



 
