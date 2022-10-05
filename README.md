## Predicting The Impact of a New Stadium on Surrounding Neighborhoods Using a k-means Clustering Algorithm

### Study Overview
In September of 2021, the Chicago Bears signed a purchase agreement for the former Arlington International Racecourse property in Arlington Heights, Illinois. The purchase of the land, at a cost of $197.2 million, is the strongest indicator yet that the ownership of the Bears is likely to move the team to a new stadium in the suburbs, roughly 30 miles northwest of the franchise's current home, Soldier Field. 

The Mayor of Arlington Heights, Tom Hayes, is already touting the “long-term economic and community-development” that he hopes will occur with the relocation of the Bears. Often, though, the introduction of a professional stadium into a neighborhood coincides with unintended consequences, including the depletion in the long-term viability and supply of low-cost housing, a deepening class polarization, and marginal damage to the local education system as the neighborhood skews towards higher-income residents. Unfortunately, the impact of a new professional stadium on a neighborhood is typically only measurable in the decades following construction.

Therefore, this paper showcases an applied predictive model that uses data from those neighborhoods previously impacted by the construction of stadiums to examine the potential impact on neighborhoods with similar attributes facing looming stadium construction – in this case, specifically, Arlington Heights.

First, I employ the use of a **k-means clustering unsupervised machine learning algorithm** and the ‘tidycensus’ package in RStudio to produce **geodemographic classification based on census tracts**. This results in coupling those census tracts with similar demographic characteristics to those tracts in Arlington Heights. Second, the model uses a standard difference-in-differences approach to suggest what may occur in Arlington Heights based on the recorded impact on similar neighborhoods by professional stadiums. Using data from Zillow’s proprietary ZTRAX database, along with data from the ‘tidycensus’ package, the model put forth in this research is able to determine the rate of growth of both home prices and average rent costs in the areas surrounding the new stadium, as well as the impact on racial demographics by constructing a multi-group segregation index and a diversity gradient.

The implications of this proposed model for practitioners in the sport industry is significant, as being able to predict the impact of a professional stadium on neighborhoods and/or communities will greatly assist in remedying, or easing, the impact of gentrification that often occurs in such scenarios.

### My Workflow

![workflow](https://user-images.githubusercontent.com/57458963/194142228-1ee8e0f0-d2e7-4101-9fe9-820d8efa7697.PNG)

### Results of Principal Component Analysis

![pca-results](https://user-images.githubusercontent.com/57458963/194142434-5bed6f42-4f65-43f9-bf42-6bd60e1dcba7.PNG)

### PCA Feature Importance

![pca-feature-importance](https://user-images.githubusercontent.com/57458963/194142604-e8aa7755-d18c-4f0e-b4b4-3bdbfe73a3dc.PNG)

### Results of Clustering Process (for Minneapolis)

![clustering-results](https://user-images.githubusercontent.com/57458963/194142880-1e291b90-4310-4f8d-8a85-778ef64c316e.PNG)

### Q-Q Plot: Sampled Quantiles vs. Theoretical Quantiles

![qqplot](https://user-images.githubusercontent.com/57458963/194143079-5a6fe177-2ce4-4325-9df1-0b06ffcd499d.PNG)

### Difference-in-Differences Regression Results

![did-results](https://user-images.githubusercontent.com/57458963/194143237-af0b059c-eaf4-4738-9edf-cb5b0a83b797.PNG)

### Visualized Estimation Of House Price Increases in Arlington Heights

![mapped-results](https://user-images.githubusercontent.com/57458963/194143403-efebb796-d324-45db-b3af-3275e1f3809c.PNG)
