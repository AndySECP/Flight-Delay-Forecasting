# Flight-Delay-Forecasting
2019 - Using weather, traffic and airlines' information to predict the delay of flights in California

## Objectives

The analysis is based on kaggle *2015 Flight Delays and Cancellations* dataset, combined with weather data scrapped from Iowa State University weather data. The goal is to identify the main causes of delays for Californian airplanes and to use this infomation to forecast the delay for future departures. 

## Data Visualization

Here are the flights that are used in our analysis, those are all the flights that have a departure or an arrival in California.

![flight_map](https://user-images.githubusercontent.com/38164557/57184669-a3ce2000-6e73-11e9-8b31-eb4002be99f3.PNG)

Boosted trees can be analysed to retrieve how much weight they give to each feature independently. Concerning the features that composed our dataset, the ranking of the importance of each of them, extracted from boosted trees is the following: 

![feat_imp](https://user-images.githubusercontent.com/38164557/57184721-6b7b1180-6e74-11e9-8236-107c1891c93e.PNG)

With a more in depth analysis of the main features at hand we can visualized how the choice of airline is going to influence the expected delay of the flight. On the following plot, the size of the bubble represents the number of flights and on the y-axis we can assess the avarage delay. While mainly all big airlines companies show a delay that is average, for the smaller ones we observe a way more important difference with some of them showing almost no delay on average and others that have significantly higher statistics.

![Buble_chart](https://user-images.githubusercontent.com/38164557/57184710-41295400-6e74-11e9-8288-6addd9ba9ec6.PNG)

In addition, as seen in the feature importance graph, the weather data that we added with webscrapping seem particularly important for our analysis. The following visualization describe the seasonality introduced by those features.

![Humidity_WS_DepDelay](https://user-images.githubusercontent.com/38164557/57184702-1f2fd180-6e74-11e9-804f-fda9221071b8.jpg)




**Sources**:

Kaggle dataset: https://www.kaggle.com/usdot/flight-delays?fbclid=IwAR2GJGwOFuOSK1byAFtkIdx8AH-Zr3jkQSpN0r3AVcEWt0xgj4rCvnE7k2I#flights.csv

Iowa State University weather data: https://mesonet.agron.iastate.edu/request/download.phtmlnetwork=CA_ASOS&fbclid=IwAR3XnA32GH8EI8kmlrzZq9YcukL9-S_CxK8aPdvjioQrbbN_6USAsLgQ13k
