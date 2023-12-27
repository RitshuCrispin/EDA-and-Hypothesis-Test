# EDA-and-Hypothesis-Test
Exploratory Data Analysis and Hypothesis Test with ttest_ind and levene.

# Overview

The dataset contains user and expert reviews, genres, platforms (for example, Xbox or PlayStation), and historical data on video game sales.

## Objective

To identify patterns that determine whether a game is successful or not. This will allow us to detect promising projects and plan advertising campaigns.

### Data Description

— *name*: Name of the video game

—*Platform*: Platform

—*Year_of_Release*: Game release year

—*Genre*: Genre of the game

—*NA_sales*: North American sales in millions of US dollars

—*EU_sales*: sales in Europe in millions of US dollars

—*JP_sales*: sales in Japan in millions of US dollars

— *Other_sales*: sales in other countries in millions of US dollars

—*Critic_Score*: score from 1 to 100

— *User_Score*: score from 1 to 10

—*Rating*:ESRB Rating

Data for 2016 may be incomplete.

## Libraries
- pandas
- numpy
- scipy
  - scipy: levene, ttest_ind
- matplotlib

# Conclusions
1. At the initialization of the project, we had to understand the information that each column offered us and how these were related to the project objective of identifying whether a game is successful or not based on sales by platform, genre and region.
2. During data processing, it was identified that the dataframe had incomplete information, this was probably because the data was extracted from various sources before having all the information complete, since 'tbd' data was presented that was pending qualification. Based on all this, we had to work with null values since the columns were not related to each other in order to complete this data.
3. Next, we study the statistical distribution of the games and platforms, obtaining some answers such as:
- From 1994 onwards there was a growth in the launch of new games until 2015 where it was its highest peak.
- The 3 platforms with the highest sales were the Play Station 2, X360 and the Nintendo Wii.
- The Nintendo Wii was the most popular platform and the one that generated the highest sales in 2009. After that, the most popular platforms were the X360 and the Wii.
- Some additional data regarding the platforms is that the popularity of each of them lasts approximately 5 years and their validity lasts 10 years before they begin to disappear from the market. In addition, approximately every 2 and a half years, between 2 to 3 new platforms are launched on the market.
- Currently, in 2016, the Play station 4, XOne and 3DS are the platforms that have the greatest projection and will maintain their popularity for at least 2 more years.
- On the other hand, the ratings of users and critics of the games do not have much impact on sales.
- The behavior of Japanese users with North American users differs somewhat in terms of genres, ratings and platforms.
4. Finally, 2 two-tailed hypotheses were formulated comparing the means of 2 populations where we accepted the following theses:
- Average user ratings for Xbox One and PC platforms are not the same.
- Average user ratings for Action and Sports genres are the same.
5. In general, it is concluded that a game will have higher sales depending on the platform and region in which it is launched because the end user differs depending on their context.
