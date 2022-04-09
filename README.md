# PyBer_Analysis
Using Python to analyze and visualize ridesharing data

![RS](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/ride_share.png)

## Overview
Ridesharing is a popular form of transportation which has become prevalent across our society.  In general, it is a convenient form of transportation, and in some cases it can be a more cost efficient option compared to driving one's own vehicle.  PyBer is a ridesharing company that would like to know more about the accessability of their service in different types of cities.  Factors such as number of drivers, number of rides, and average fare price for each city type were analyzed to uncover trends.  These trends may be able to guide PyBer's future business decisions, thereby making their services more affordable and widely available.

## Analysis
Upon initial inspection of the ridesharing data, three distinct city types could be identified.  The three city types were 'urban', 'suburban', and 'rural'.  Average ride fares and a count of total rides were calculated for each city type.  This data was then plotted to a bubble plot with total number of rides on the x-axis and average fare on the y-axis.  The graph appears to display a negative relationship between average fare by city and total number of ride by city.  Generally, urban cities have a higher number of total rides and lower average fare prices.  Conversely, rural cities have a lower number of total rides and higher average fare prices.  Another element of this plot is the bubble size, which correlates to driver count per city.  Noticeably, urban cities have much higher driver counts than suburban or rural cities.  Citites with more drivers appear to have lower average fares compared to cities with less drivers.  

![Fig1](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/Fig1.png)

To determine the strength of the relationship between average fairs per city and ride count per city, a pairwise correlation was run on two series containing data for each city.  There was a relatively strong negative correlation between these two variables of r = -0.58.  Additionally, this analysis was completed on average fairs per city and driver count per city.  The correlation between these variables was also fairly strong at r = -0.54.  Please note that these relationships are derived from each citites data rather than data grouped together by city type.  The code used to collect these values can be seen below.

![RFC](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/rides_fare_corr.PNG) 
![DFC](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/driver_fare_corr.PNG)

---
Similar to the analysis above, statistics for total rides, total drivers, and total fares were calculated for each city type.  In addition, these numbers were used to calculate the average fare per ride and average fair per driver within each city type grouping.  Rural cities have less total rides and drivers than suburban and urban cities.  Urban cities have the most total rides and drivers.  Suburban cities fall between rural and urban cities for these categories.  Overall, the total fares for rural cities is $15.028.40 less than suburban cities and $35,526.45 less than urban cities.  However, due to the low total rides in rural cities, the average fair per ride is $34.62.  This is just over $10 more on average than urban cities, and about $4.50 more on average than suburban cities.  There is an even larger disparity when looking at the numbers for average fare per driver.  In rural cities, the average fair per driver is $55.49.  This is nearly $40 more on average than urban cities and $16 more than suburban cities.

![FS](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/Fare_Summary.PNG)

---
Finally, weekly fairs for each city type between the months of January and April were plotted on a line chart to visualize this data over time. 

![TFL](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/Fig_8.png)

This graph confirms that total fares for rural cities are lower than suburban or urban cities over time.  Overall, this weekly data is fairly centered around the medians.  The medians for weekly data are $191.85 for rural citites, $1045.06 for suburban citites, and $2218.20 for urban cities.  The upper and lower bounds for rural, suburban, and urban cities can be seen below.

![LB](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/lower_bound.PNG) ![UB](https://github.com/Mots94/PyBer_Analysis/blob/main/analysis/upper_bound.PNG)
