# Data Analyst Portfolio

[Project 1: Soccer Stats - Data Exploration using an API](https://github.com/alex-milneski/penalty-kick-analysis-top-5-leagues/tree/main)

The goal of this project was to explore the expected goal (xG) metric as it pertains to penalty kicks (PK). This probabilistic outcome metric used by sports analysts and professional sports teams alike is determined by Opta Sports to be 
xG = 0.79, signifying that a penalty kick has a 79% chance of being a goal. I wanted to see how real-world data performs against the goal probability, and if some teams or leagues overperform or underperform their PKs.

League and season data was scraped using [FBRef's API](https://fbrapi.com/documentation) for 5 seasons from the 5 top leagues. Using Python, I automated the retrieval of the 'penalty kicks attempts' and 'penalty kicks made' from the API's JSON for all 5 leagues and seasons. I then merged and filtered the data to look at PK conversion rates by league, PK conversion by team within their respective leagues as well as within the context of all 5 leagues.

I created a dashboard using Tableau to illustrate Spanish La Liga's underperformance at PKs.

![alt text](https://github.com/alex-milneski/penalty-kick-analysis-top-5-leagues/blob/main/la_liga.png)

### Skills used
Python, Google collabs, Tableau, data exploration, API, dashboards, data visualization

### Results/Insights
2910 PK attempts from 25 seasons of data did in fact show a 79.45% conversion rate. Opta's xpG of 0.79 accurately predicts the conversion rate of penalty kicks in general. However, some teams and leagues noticeably overperformed/underperformed the metric. For example, 83% of penalty kicks have been scored in the last 5 years of French Ligue 1 while less than 76% have been scored in Spanish La Liga during the same period of time. The Spanish league has some of the worst performers at PKs in the top 5 leagues while also having a team with the highest success rate, Espanyol, with 15 goals from 15 attempts. 

<br>

[Project 2: Karst Hydrology - Primary Data Collection and Graphing](https://github.com/alex-milneski/honors-defense-water-logger-project)

I was tasked with cleaning, organizing and graphing data from a [HOBO water level logger](https://www.onsetcomp.com/products/data-loggers/u20l-0x) for an ongoing 5 year karst hydrology project. In total, 6 case study graphs were created with matplotlib; each illustrating different hydrological processes or temporal scales.

![alt text](https://github.com/alex-milneski/honors-defense-water-logger-project/blob/b22faf2ee050960b1312950b41ee382f0d35496a/Jaymie's%20Honor%20Defense%20Data/CS1.png)

This graph shows the relationship between precipitation and water conductivity. In karst landscapes, limestone dissolved in water causes higher water conductivity, and provides a high baseline ideal for hydrological study. The Case Study 1 graph illustrates how a rainfall event caused a dilution signature, shown by a temporary dip in specific conductance during a period of high precipitation.

### Skills Used
Python, Google Sheets, matplotlib, data cleaning, graphing, combining primary and secondary data.

### Challenges
This was my fist project working with matplotlib and primary data collection.
- I needed to visualise data combining both line and histogram charts in one plot and have 3 variables with different scales - I decided to create a twin axis and staggering it using Python's matplotlib.
- Time stamp information needed to be standardized across all datasets. This was solved with the use of the dt.floor() method from the pandas library which was able to round the time information to the nearest hour.

Project 3: Ontario Waterbirds - Spatial Analysis with R
