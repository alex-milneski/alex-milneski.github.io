# Data Analyst Portfolio

[Project 1: Ontario Shorebirds - Time Series Spatial Analysis with R](https://github.com/alex-milneski/ontario-shorebird-R)

The goal of this project was to explore shorebird data from the [Ontario Shorebird Survey (OSS)](https://www.canada.ca/en/environment-climate-change/services/bird-surveys/shorebird/ontario.html) to look at population trends and spatial relationships. In the end, the research resulted in a better understanding of the data gaps and limitations of the OSS and shorebird surveys as they pertain to bird science and conservation.

The latest [Birds Canada report](https://www.birdscanada.org/introducing-the-state-of-canadas-birds) estimates shorebirds in Canada have declined by 42% since 1980. The OSS was chosen not only because of the importance of shorebird research for future conservation efforts, but the OSS is conducted by skilled birders, trained biologists and the survey has been running since the 1970 - good data quality and great for time series analysis. Dahttps://naturecounts.ca/nc/default/datasets.jsp?code=PRISM-OSS) 

### Conclusions and Insights



<img src="https://github.com/alex-milneski/ontario-shorebird-R/blob/main/Data-Visualization/survey-site-frqcy.png" alt="survey site frequency" width="600" height="600"/> <img src="https://github.com/alex-milneski/ontario-shorebird-R/blob/main/Data-Visualization/survey-locations.gif" alt="time series" width="400" height="400"/>  
Fig 1: Survey frequency by survey location (1980-2024). High frequency near major urban centers.
Fig 1:Survey Site Locations where Lesser Yellowlegs have been observed (1980-2024)

Both Greater and Lesser Yellowlegs see a downwards trend in observation counts from the OSS. Highly variable counts can be explained by inconsistant survey frequency, temporal gaps in surveys at certain locations and natural variance in migratory behaviour. In the case of Lesser Yellowlegs, they are a species at risk known to return to the same sites during breeding and migration; which make them a good species to look at. However, their breeding range is fully outside of the scope of the survey (Figure 1). Much of their habitat/stop-over sites are away from urban centers which is under-represented in the survey.

Other limitations:

Nonquon Sewage Lagoons, which was the most frequently visited site, stopped being surveyed by the OSS in 2015 with some data gaps in the final years. The inconsistant survey frequency is seen within all sites for the ~50 years of data. I posit that the COVID-19 pandemic caused some data gaps in the early 2020s but also the volunteer-based nature of the project and site accessibility causing data gaps.
Natural variability of migration
Even at sites Shirley's Bay (42.007) and Andrew Haydon Park (42.003) less than 10km from eachother, bird counts can vary greatly - as seen with Lesser Yellowlegs in 1995 (Fig 2, Fig 3). 

Then, there are the limitations of using a single survey source for looking at trends. As seen with partnerships like the Program for Regional and International Shorebird Monitoring, a large scale view is necessary to confidently assess shorebird populations.

### Skills used
R, Data cleaning, Data visualization, Time Series

[Project 2: Soccer Stats - Data Exploration using an API](https://github.com/alex-milneski/penalty-kick-analysis-top-5-leagues/tree/main)

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

[Project 3: Karst Hydrology - Primary Data Collection and Graphing](https://github.com/alex-milneski/honors-defense-water-logger-project)

I was tasked with cleaning, organizing and graphing data from a [HOBO water level logger](https://www.onsetcomp.com/products/data-loggers/u20l-0x) for an ongoing 5 year karst hydrology project. In total, 6 case study graphs were created with matplotlib; each illustrating different hydrological processes or temporal scales.

![alt text](https://github.com/alex-milneski/honors-defense-water-logger-project/blob/b22faf2ee050960b1312950b41ee382f0d35496a/Jaymie's%20Honor%20Defense%20Data/CS1.png)

This graph shows the relationship between precipitation and water conductivity. In karst landscapes, limestone dissolved in water causes higher water conductivity, and provides a high baseline ideal for hydrological study. The Case Study 1 graph illustrates how a rainfall event caused a dilution signature, shown by a temporary dip in specific conductance during a period of high precipitation.

### Skills Used
Python, Google Sheets, matplotlib, data cleaning, graphing, combining primary and secondary data.

### Challenges
This was my first project working with matplotlib and primary data collection.
- I needed to visualise data combining both line and histogram charts in one plot and have 3 variables with different scales - I decided to create a twin axis and staggering it using Python's matplotlib.
- Time stamp information needed to be standardized across all datasets. This was solved with the use of the dt.floor() method from the pandas library which was able to round the time information to the nearest hour allowing for consistant comparable time information across all datasets.
