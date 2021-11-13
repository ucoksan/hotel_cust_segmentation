# Hotel's Customer Segmentation

EA four(4) star hotel located in Lisbon, Portugal, Europe gathered customer's data during 2015 to 2018 period. The data contains several information related to Hotel's bookings by Customer during the period.

## Project Task

The goal of this project are:

1. Do EDA to gain insight from the several aspect of customer behavior, and
2. Do RFM analysis for customer's segmentation classification.
3. Recommendation of action based on customer behavior.

## Data Source

1. Data can obtained from <a href="https://www.kaggle.com/nantonio/a-hotels-customers-dataset" target="_blank">Kaggle</a>
2. Data is gathered from 2015 to 2018 period
3. Details about data can be see on <a href="https://doi.org/10.1016/j.dib.2020.106583" target="_blank">this link</a>

## Data Preparation & Cleaning

1. Not all columns will be selected for analysis process, only dataframe with related dataframe will be used.
2. Check for missing value, data types, and invalid values.
3. Renaming columns name for aesthetics purpose.
4. Create additional columns (variables) to be used for analysis later (`Total Revenue`,`Months Since Last Arrival`, `Percent Canceled`)

## EDA Process

In this project we will do Analysis for several aspect, such as:
1. Customers distribution by Nationality (also for Total Revenue and Total rooms bookings).
2. Distribution of Customer population based on current Market Segment and Distribution Channel.
3. Some correlation plot for `Average Lead Time` and `Total Revenue` columns.

## RFM Analysis

For RFM analysis (Recency, Frequency, Monetary). Following columns will be use for references:
1. `Month Since Last Arrival` for `Recency Score`
2. `Successful Bookings` for `Frequency Score`
3. `Total Revenue` for `Monetary Score`

For scoring method:
1. Dividing the values of each “Month Since Last Arrival” & “Total Revenue” variables based on their distribution value
2. Because of distribution pattern, “Successful Bookings” variable cannot be grouping based on its distribution value, so we classified by several value instead.
3. Each category divided into 3 groups of score (1-3)
![alt text](https://github.com/ucoksan/hotel_cust_segmentation/blob/main/data_plot/rfm_ref.png?raw=true)
4. And RFM clustering as:
![alt text](https://github.com/ucoksan/hotel_cust_segmentation/blob/main/data_plot/rfm_table.png?raw=true)

## Analysis Insight

From the analysis, we got some points:
1. Most of the customer, bookings and revenue come from European region, which same region with the Hotel location. The customer from the other region probably less frequent to stay at the Hotel.
2. Travel Agent/ Operator is the Distribution Channel mostly used by customers while Electronic Distribution is the least.
3. The number of loyal customer is so low at this point, while the number of Customers categorized by Others and Lost Cheap Customers is very high. 
4. Most customers only 1 times stay and the customers who stay frequently is very rare compared to customers who frequently stay at the Hotel 

## Recommendation

For the better sales at the future, there are several method for sales & marketing program to be evaluate later:
 * Company can create campaign for those 1 time stay Customer to become loyal customer such as  discounted price on holiday occasion or business trip campaign.
 * Since Travel Agent/ Operator is the Distribution Channel most used by customers, company should increase campaign engagement by Travel Agent/ Operator channel.
 * Furthermore, Electronic Distribution is a things people access almost every time, engagement from Electronic Distribution can be useful for gaining engagement.
 * For future analysis, we need to know the period when the customer usually stay at Hotel, to know the effective timing to start campaign.

