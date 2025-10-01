# Data Analyst Portfolio

[Project 1: Soccer Stats - Data Exploration using an API](https://github.com/alex-milneski/penalty-kick-analysis-top-5-leagues/tree/main)

The goal of this project was to explore the expected goal (xG) metric as it pertains to penalty kicks (PK). This probabilistic outcome metric used by sports analysts and professional sports teams alike is determined by Opta Sports to be 
xG = 0.79, signifying that a penalty kick has a 79% chance of being a goal. I wanted to see how real-world data performs against the metric, and if some teams or leagues overperform or underperform their PKs.

League and season data was scraped using [FBRef's API](https://fbrapi.com/documentation) for 5 seasons from the 5 top leagues. Using Python, I automated the retrieval of the 'penalty kicks attempts' and 'penalty kicks made' from the API's JSON for all 5 leagues and seasons. I then merged and filtered the data to look at PK conversion rates by league, PK conversion by team within their respective leagues as well as within the context of all 5 leagues.

I found that overall the xG = 0.79 was well warranted but some teams and leagues noticeably overperformed/underperformed the metric. 

I created a dashboard using Tableau to illustrate Spanish La Liga's underperformance at PKs.

![alt text](https://github.com/alex-milneski/penalty-kick-analysis-top-5-leagues/blob/main/la_liga.png)



[Project 2: Karst Hydrology -](https://github.com/alex-milneski/honors-defense-water-logger-project)
