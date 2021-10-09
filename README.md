# Investing in Surf and Ice Cream

In this week module we are focused on the analysis of the weather in Hawaii.  This is an exploratory analysis that consideres the last 12 months, starting from the last data point registered.  This analysis would serve as backup for a bussiness plan that would be presented to a potential investor.

## Overview

Our initial analysis was designed to retrieve the last 12 months of precipitation data stored in a **SQLite** database. From the database, we have access to daily measurements of temperatures and rain precipitation registered by diverse weather stations.  Now, we need to add temperature trends to our analysis, specifically, temperature data for the months of June and December in Oahu.  This additional information would help us to determine if the surf and ice cream shop is sustainable year-round.

## Analysis

The data base called : **hawaii.sqlite** has two tables: `Measurement` and `Station`, which contains all the information about precipitation and temperatures measured yearly across a vast area covered by several weather stations. The first step in our analysis is to access to these tables by using the method `prepare` and saving in our framework their references by using their corresponding methods:  `_.classes.measurement` and `-.classes.station`.  Once we have the references to the two tables, we need to access them to retrieve all the temperatures for the month of June and December. Those temperatures are stored in Python as a list  in order to create a Dataframe and generate a summary statistics. The code written in jupyter notebook is shown in  [SurfsUp_Challenge.ipynb](https://github.com/LeidyDoradoM/SurfsUp_Challenge/blob/main/SurfsUp_Challenge.ipynb) as deliverable 1 and 2. The summary statistics are shown below:

| June Temps | Dec Temps |
| --- | ----------- |
| ![June](https://raw.githubusercontent.com/LeidyDoradoM/SurfsUp_Challenge/main/Resources/df_JuneStats.png) | ![Dec](https://raw.githubusercontent.com/LeidyDoradoM/SurfsUp_Challenge/main/Resources/df_DecStats.png) |

Figure 1. Statistics for June and December

### 1. Minimum Temperature for June and December

Miminum temperatures for June  and December differ in about 8 degrees, which shows how some day in December could reach lower temperatures than summer months as June.

### 2. Range of Temperatures for June and December

Although the minimum temperatures between the two months (June-December) differ for almost 10 degrees, the maximum temperatures are very similar (i.e. they differ only in 2 degrees). This means that the range of temperatures for December is wider compared with the month of June.  Likewise, this can be seen in their values for the standard deviation, **std**, where December has a larger value for the std.

### 3. Percentiles for June and December

Regarding the percentiles, the second quartile (50%) for June is 75F and the third quartile (75%) for December is about the same 74F.  This shows how for the month of December only about 7 or 8 days have temperatures above 74F while in June the double of days have temperatures in the upper part of the 70s degrees.

## Summary

From our analysis we can conclude that 
Precipitation Queries f
| June Temps | Dec Temps |
| --- | ----------- |
| ![June](https://raw.githubusercontent.com/LeidyDoradoM/SurfsUp_Challenge/main/Resources/df_prcpJuneStats.png) | ![Dec](https://raw.githubusercontent.com/LeidyDoradoM/SurfsUp_Challenge/main/Resources/df_prcpDecStats.png) |