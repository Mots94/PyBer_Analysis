# PyBer_Analysis
Using Python to analyze and visualize ridesharing data

## Overview
Ridesharing is a popular form of transportation which has become prevalent across our society.  In general, it is a convenient form of transportation, and in some cases it can be a more cost efficient option compared to driving one's own vehicle.  PyBer is a ridesharing company that would like to know more about the accessability of their service in different types of cities.  Factors such as number of drivers, number of rides, and average fare price for each city type were analyzed to uncover trends.  These trends may be able to guide PyBer's future business decisions, thereby making their services more affordable and widely available.

## Analysis
Upon initial inspection of the ridesharing data, three distinct city types could be identified.  The three city types were 'urban', 'suburban', and 'rural'.  Average ride fares and a count of total rides were calculated for each city type.  This data was then plotted to a bubble plot with total number of rides on the x-axis and average fare on the y-axis.  The graph appears to display a negative relationship between average fare by city and total number of ride by city.  Generally, urban cities have a higher number of total rides and lower average fare prices.  Conversely, rural cities have a lower number of total rides and higher average fare prices.  Another element of this plot is the bubble size, which correlates to driver count per city.  Noticeably, urban cities have much higher driver counts than suburban or rural cities.  Citites with more drivers appear to have lower average fares compared to cities with less drivers.  
![Fig1](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/Fig1.png)

To determine the strength of the relationship between average fairs per city and ride count per city, a pairwise correlation was run on two series containing data for each city.  There was a relatively strong negative correlation between these two variables of r = -0.58.  Additionally, this analysis was completed on average fairs per city and driver count per city.  The correlation between these variables was also fairly strong at r = -0.54.  The code used to collect these values can be seen below.
![RFC](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/rides_fare_corr.PNG) 
![DFC](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/driver_fare_corr.PNG)
