# Investing in Surf and Ice Cream

In this week module we are focused on the analysis of the weather in Hawaii.  This is an exploratory analysis that consideres the last 12 months, starting from the last data point registered.  This analysis would serve as backup for a bussiness plan that would be presented to a potential investor.

## Overview

Our initial analysis was designed to retrieve the last 12 months of precipitation data stored in a **SQLite** database. From the database, we have access to daily measurements of temperatures and rain precipitation registered by diverse weather stations.  Now, we need to add temperature trends to our analysis, specifically, temperature data for the months of June and December in Oahu.  This additional information would help us to determine if the surf and ice cream shop is sustainable year-round.

## Analysis

The data base called : **hawaii.sqlite** has two tables: `Measurement` and `Station`, which contains all the information about precipitation and temperatures measured yearly across a vast area covered by several weather stations. The first step in our analysis is to access to these tables by using the method `prepare` and saving in our framework their references by using their corresponding methods:  `_.classes.measurement` and `-.classes.station`.

### Summary Statistics for June

Once we have the references to the two tables, we need to access them to retrieve all the temperatures for the month of June. Those temperatures are stored in Python as a list  in order to create a Dataframe and generate a summary statistics. The code written in jupyter notebook is shown in  [SurfsUp_Challenge.ipynb](https://github.com/LeidyDoradoM/SurfsUp_Challenge/blob/main/SurfsUp_Challenge.ipynb) as deliverable 1. The summary statistics are shown below:

![June](https://raw.githubusercontent.com/LeidyDoradoM/SurfsUp_Challenge/main/Resources/df_JuneStats.png)

Figure 1. Statistics for June

### Summary Statistics for December

The same process is followed to get the temperatures for the month of December.  Likewise, the [SurfsUp_Challenge.ipynb](https://github.com/LeidyDoradoM/SurfsUp_Challenge/blob/main/SurfsUp_Challenge.ipynb) shows the code as deliverable 2 and the summary of the statistics for this month are shown below:

![Dec](https://raw.githubusercontent.com/LeidyDoradoM/SurfsUp_Challenge/main/Resources/df_DecStats.png)

Figure 2. Statistics for December

## Summary

