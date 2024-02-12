Ford GoBike Data Exploration
Dataset
 I Use Cyclistic’s historical trip data to analyze and identify trends.e Cyclistic
is a fictional company. For the purposes of this case study, the datasets are appropriate and
will enable me to answer the business questions. The data has been made available by
Motivate International Inc. under this license (https://www.divvybikes.com/data-license-agreement.) This is public data that I used to explore

Tools
Excel - Data Cleaning
Download here
SQL Server - Data Analysis
PowerBI - Creating reports

Data Cleaning/Preparation

In the initial data preparation phase, we performed the following tasks:

Data loading and inspection.
Handling missing values.
Data cleaning and formatting.
Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions, such as:
how different customer types are using Cyclistic bikes.
**Limitations**
I had to remove all zero values from budget and revenue columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both budget and number of votes with revenue.


Summary of Findings

In the exploration, I found that

Male users encompassed 75% of all users, female users 23%.
The bike share service is also quite popular with the users as it has 91% of them as subscribers.
Most users of the service are between 30 and 40 years old with the youngest being 21 years and the oldest being 95 years after cleaning the data.
The day with the most rides is Thursday followed closely by Tuesday, Wednesday and Friday. The days with the lowest rides are Sunday and Saturday.
Most users prefer to start their rides at 0800h and 1700h followed by 1800h and 0900h.
To measure the distance coverd by the users, I created a column for distance in kilometers, based on the longitude and latitude start and end points.It was clear from the distance covered by the users that most of them could only manage an average of 1.5km. The longest distance covered was 63km.
Most rides last an average of 11 minutes and most people don't go beyond 13 minutes.The longest ride is 1409 minutes which is about 23 hours
I went on to look at how subscribers use the service compared to the customers. The analysis indicates that

Customers use the service mostly on Thursday, Friday, Sunday, Monday and Tuesday. Subscribers however use the service mostly on weekdays and occasionally on the weekends, that is, Saturday and Sunday.
Subscribers mostly start their rides at 1700h and 0800h which could indicate they use it to go to work in the morning and back home in the evening while customers mostly start their rides at 1700h
Interestingly enough though was discovering that customers covered more distance than the subscribers which in my opinion confirms that subscribers use it for commuting to work because the usage decreases significantly on weekends while customers use it for work and other activities perhaps.
The mean for customers is 1.67 km, and the mean for subscribers is 1.46 km.
An analysis of the relationship between age of the users and the distance covered shows that the longest and shortest rides fluctuate between the older users who are above 70 years of age.

Most female customers start their rides at 1700h followed by 0800h and 1300h and 1600h
Most male customers start their rides at 1700h followed by 1600h and 0800h.
Most customers who identify as other start their rides at 1700h and 0800h
Most female subscribers start their rides at 0800h followed by 1700h and 0900h and 1800h
Most male subscribers start their rides at 1700h followed by 0800h and 0900h.
Most subscribers who identify as other start their rides at 1700h followed by 1800h and 0800h
Most users from both categories aged 34 years preferred to ride on Thursdays at 1700h.
Male customers prefer to ride on Thursdays and Fridays while female customers prefer to ride on Thursday and Sunday. Customers who identify as other prefer to ride on Thursdays and Fridays while subscribers of the same category prefer to ride on Wednesdays and Thursdays.

Key Insights for Presentation
For the presentation, I focus on the usage of the service by users according to their gender, user category and age. I start by plotting a pie chart showing the gender distribution of the users followed by introducing a new column called start_hour that extracts the hour of the day when the users use the service. This is an important insight because it could help the service providers know what time of day to do repairs or maintenance for their bikes with affecting their users negatively.

image

Afterwards, I looked at how each category of users uses the service per day and plotted it on a bar chart which showed clearly the most popular days. I went ahead and broke it down further into the most popular hour of the day and what age of users were associated with it. I used a heatmap for this and the darker shades on the heatmap provided the required insights.

image

You can view more insights by downloading and opening this file in your browse
Project Overview

This data analysis project aims to provide insights into the sales performance of an e-commerce company over the past year. By analyzing various aspects of the sales data, we seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the company's performance.

bar plot

Data Sources
Sales Data: The primary dataset used for this analysis is the ".csv" file, containing detailed information about each sale made by the company.

Tools
Excel - Data Cleaning
Download here
SQL Server - Data Analysis
PowerBI - Creating reports
Data Cleaning/Preparation
In the initial data preparation phase, we performed the following tasks:

Data loading and inspection.
Handling missing values.
Data cleaning and formatting.
Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions, such as:

What is the overall sales trend?
Which products are top sellers?
What are the peak sales periods?
Data Analysis
Include some interesting code/features worked with

SELECT * FROM table1
WHERE cond = 2;
Results/Findings
The analysis results are summarized as follows:

The company's sales have been steadily increasing over the past year, with a noticeable peak during the holiday season.
Product Category A is the best-performing category in terms of sales and revenue.
Customer segments with high lifetime value (LTV) should be targeted for marketing efforts.
Recommendations
Based on the analysis, we recommend the following actions:

Invest in marketing and promotions during peak sales seasons to maximize revenue.

Focus on expanding and promoting products in Category A.
Implement a customer segmentation strategy to target high-LTV customers effectively.
Limitations
I had to remove all zero values from budget and revenue columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both budget and number of votes with revenue.

References
SQL for Businesses by werty.
