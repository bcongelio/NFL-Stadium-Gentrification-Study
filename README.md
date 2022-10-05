## Predicting The Impact of a New Stadium on Surrounding Neighborhoods Using a k-means Clustering Algorithm

### Study Overview
In September of 2021, the Chicago Bears signed a purchase agreement for the former Arlington International Racecourse property in Arlington Heights, Illinois. The purchase of the land, at a cost of $197.2 million, is the strongest indicator yet that the ownership of the Bears is likely to move the team to a new stadium in the suburbs, roughly 30 miles northwest of the franchise's current home, Soldier Field. 

The Mayor of Arlington Heights, Tom Hayes, is already touting the “long-term economic and community-development” that he hopes will occur with the relocation of the Bears. Often, though, the introduction of a professional stadium into a neighborhood coincides with unintended consequences, including the depletion in the long-term viability and supply of low-cost housing, a deepening class polarization, and marginal damage to the local education system as the neighborhood skews towards higher-income residents. Unfortunately, the impact of a new professional stadium on a neighborhood is typically only measurable in the decades following construction.

Therefore, this paper showcases an applied predictive model that uses data from those neighborhoods previously impacted by the construction of stadiums to examine the potential impact on neighborhoods with similar attributes facing looming stadium construction – in this case, specifically, Arlington Heights.

First, I employ the use of a **k-means clustering unsupervised machine learning algorithm** and the ‘tidycensus’ package in RStudio to produce **geodemographic classification based on census tracts**. This results in coupling those census tracts with similar demographic characteristics to those tracts in Arlington Heights. Second, the model uses a standard difference-in-differences approach to suggest what may occur in Arlington Heights based on the recorded impact on similar neighborhoods by professional stadiums. Using data from Zillow’s proprietary ZTRAX database, along with data from the ‘tidycensus’ package, the model put forth in this research is able to determine the rate of growth of both home prices and average rent costs in the areas surrounding the new stadium, as well as the impact on racial demographics by constructing a multi-group segregation index and a diversity gradient.

The implications of this proposed model for practitioners in the sport industry is significant, as being able to predict the impact of a professional stadium on neighborhoods and/or communities will greatly assist in remedying, or easing, the impact of gentrification that often occurs in such scenarios.

### My Workflow

![arlington-heights-map](https://user-images.githubusercontent.com/57458963/152689823-b059f1b4-bf95-4530-8e94-bd97e063bb67.png)

