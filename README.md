# PyBer_Analysis
## Overview
The purpose of this analysis was to show the relationship between weekly Pyber fare totals and city types using charts and graphs, and to help executives at PyBer use the data in their decision making processes.

## Results
1. The city type with the largest number of rides was urban cities, while rural areas had the lowest ride count.
![image](https://user-images.githubusercontent.com/106359572/180567532-a761cf33-adc6-4200-8a44-3ba4cfe15a76.png)

The driver counts by city type followed the same pattern as above.
![image](https://user-images.githubusercontent.com/106359572/180567668-b0dfe473-ad21-4587-8c59-6bd1a907baf8.png)

The average fare per ride and per driver are both negatively correlated with the ride counts and driver counts; i.e., urban fares averaged the lowest and rural fares the highest, both per fare and per driver.
![image](https://user-images.githubusercontent.com/106359572/180567822-c9abf2d8-061f-4ad2-b1e1-d7030e5031c2.png)

The differences in fare totals between city types were fairly consistent throughout the first four months of the year.
![image](https://user-images.githubusercontent.com/106359572/180568597-8640eaab-7f40-467b-bc19-2f157a651c8f.png)

## Summary
Based on the summary shown below, urban cities have an oversaturation of drivers.  There are three drivers competing with one another for every two rides.  The average fare per driver is also lower as a result.

Conversely, drivers in rural areas are pulling too much weight, with an average of three riders competing over every two available drivers.  

The suburban average fares seem to be a happy medium, at 1.28 rides for every driver.  

![image](https://user-images.githubusercontent.com/106359572/180568846-6e41fcde-b37a-4510-922a-8ccb2d88cbda.png)


If we do a level load rebalance between urban and rural cities, we can send  drivers in urban areas to support in rural and suburban areas to even things out.  I would recommend to start with the following adjusted driver counts per city type:

Rural: 157
Suburban: 782
Urban: 2,032

Meanwhile, I would also recommend to incorporate into our datasets the length of time that each rider had to spend waiting for a driver, as this would also be a big help in assessing whether drivers are being efficienty dispatched to their jobs.

However, even with the driver count more evenly distributed based on above recommendations, the average fare per driver would still be significantly lower for urban drivers. To address the issue of urban drivers earning significantly less per job, I would recommend to start collecting the following additional data for future analyses, to see where/why the disparity exists:
- distance traveled, and 
- length of time for each ride.

The data don't show us whether the current pricing takes into account things like rush hour traffic (i.e., extra time spent per mile), or if is is solely priced based on distance travelled.    
Ultimately, to level the playing field for urban drivers, Pyber would need to assess whether pricing should be adjusted (upwards in urban areas or downwards in rural areas, or both), and what the factors should be (time of day, duration of the ride, distance travelled, etc.) 
