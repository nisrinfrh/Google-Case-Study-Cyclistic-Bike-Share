# Cyclistic Bike Share Analysis 
Cyclistic bike-share analysis case study is one of the capstone projects for the Google 

Data Analytics Professional Certificate which I completed in March2024.

## Introduction
This project is based on data curated for a fictional bike-sharing company called Cyclistic. 

The Company has more than 5,800 bicycles plus reclining bikes, hand tricycles and cargo bikes 

With over 600 docking stations to hold the bikes. The company has a flexible strategy that allows

Riders to unlock a bike from one station and return it to any other station anytime.


 Cyclistic  has two types of riders :-

Casual Riders  : Customers who purchase single-ride or full day passes.

Members Riders : Customers who purchase annual memberships.


**steps used for this case study**

***Ask  →  Prepare  →  Process  →  Analyze  →  Share  →  Actions***

# ASK

These questions identified the business task and considered the demands of the key stakeholders:

1-How do annual members and casual riders use Cyclistic bikes differently?

2-Why would casual riders buy Cyclistic annual memberships?

3-How can Cyclistic use digital media to influence casual riders to become members?

In our project, we will focus on the first question.

 **BUSINES Task**

Analyze the differences in bike usage Patterns between casual riders and annual members, and develop a new 

Marketing strategy  aimed at  converting  casual riders in to annual subscribers.

led by lily Morenothe the Director of Marketing, and supported by Cyclistic's Markiting analytics team.

This project will collect analyze and report data to  inform the company's strategic marketing decisions. .


**Tools Used for Analysis**

I utilized the following tools for this case study:

**RStudio**: to clean, process, and analyze the data.

**PowerBI**: to generate insightful visualizations from the analyzed data.

**GitHub**: to establish a repository for the utilized code and to create public links for the visuals produced, respectively.

These were the steps taken for data processing:

 **Limitations**

I had to remove some columns that were unnecessary for my analysis.

I had to delete rows with negative values in the duration column.



# PREPARE

I Use Cyclistic’s historical trip data to analyze and identify trends. 

I chose 2020 data  with 13 columns and 3527368  rows. 

12 CSV files of Divvy quarterly trips data are  located , stored and  organized in my computer .

 *licensing, privacy, security, and accessibility*
 
The data has been made available by Motivate International Inc under this license (https://www.divvybikes.com/data-license-agreement.)

there  is no issues with bias or credibility in this data.

**The data seems to fit the definition of ROCCC:-**

**Reliable**  the data is reliable as it is directly downloaded from the company’s servers.

**Original** the data is collected and owned by Cyclistic.

**Comprehensive** The data as stated earlier is a collection from 2013 till present. We have enough data to work with given the huge historical data.

**Current**  The data is regularly updated by the geotrackers in the bikes. So the data satisfies this property.

**Cited** -no citing needed as the data is collected and owned by the company Cyclistic itself.
 
 For the purposes of this case study, the datasets are appropriate and

  will enable me to answer the business questions.

# PROCESS

I used RStudio Desktop as the primary data processing tool for this analysis.

Firstly, I installed the necessary packages required for the analysis of these datasets.

This included the “tidyverse” package for data analysis and cleaning, “Lubridate” for

Handling date attributes, and “dplyr” for data manipulation.

Next, I uploaded the trip datasets, which were in 12 CSV format files, to

R using the ‘read_csv’ function. I then assigned each dataset a more consistent name for easier reference.

**The following steps outline the cleaning and manipulation process:-**

▪ Additional columns of data, such as day, month, and year, were added to provide additional

opportunities for data aggregation.

▪ All 12 CSV files were combined into one file named "alltrips" for comprehensive analysis.

▪ A calculated field for the length of the ride (ride_length) and the weekday was added since

The original data did not have the trip duration column.

▪ Negative values in the "ride_length" column and rows representing bikes out of circulation 

(HQ QR) were deleted.

▪ Given the removal of data, a new version of the data frame named “alltrips2” was created to

Maintain data integrity throughout the analysis.

# ANALYZE

The analysis was performed using RStudio.

After cleaning and properly formatting the data, I conducted a descriptive analysis.

The new and clean version of the data frame contained a total of 3,776,042 rows, 

with annual members accounting for 68% of Cyclistic’s total customers,

while casual members constituted only 38%.

 *CONDUCT DESCRIPTIVE ANALYSIS* on *ride_length* (all figures in Minuts)

#### Summary of ride_length:_


![Screenshot (134)](https://github.com/nisrinfrh/google_project/assets/157531427/351f8af9-00f5-4bcc-b950-2b36526adc39)


#### Compare Members and Casual users:_

![Screenshot (135)](https://github.com/nisrinfrh/google_project/assets/157531427/dd3f856d-bb6c-4137-8e95-7dbe70a9a056)

  
#### See the average ride time by each day for Members vs Casual users:

![Screenshot (137)](https://github.com/nisrinfrh/google_project/assets/157531427/0522f602-1584-4a6d-bca9-a3ae9a6772ba)

##### Analyze ridership data by Type and Weekday

*calculates the number of rides and average duration*

![Screenshot (140)](https://github.com/nisrinfrh/google_project/assets/157531427/260c80c0-d095-4fb6-848f-e52a115660b4)


## SHARE

I created insightful visualizations of the data with Power BI.

For the presentation, I focused on the usage of the service by users according to their user category.

A pie chart showing the ride type distribution of the users:

![Screenshot (147)](https://github.com/nisrinfrh/google_project/assets/157531427/c705c0cb-a86e-4bc5-98d3-8cbdeac6e167)


Then I followed by introducing a new column called start_hour that extracts the hour of the day when the users use the service.

This is an important insight because it could help the service providers know what time of day to do repairs or

Maintenance for their bikes without affecting their users negatively.

A line chart to visualize the most popular hour:


![Screenshot (153)](https://github.com/nisrinfrh/google_project/assets/157531427/c2366f20-d8ea-4ba4-95f8-2582bbeba717)


Then  I looked at how each category of users uses the service per day of the week.   

 *Clustered  bar chart  which showed clearly the most popular days.* 

![Screenshot (149)](https://github.com/nisrinfrh/google_project/assets/157531427/205d517e-a706-4f5e-a68f-ce2527d6fc72)



### *Summary of Findings*

# ACTIONS

At this phase, I took some observations from the analyzed data which turned out to be important insights and 

I also pointed out a few recommendations which will all be summarized below.

**OBSERVATIONS**

**The bike share service is  quite popular with the users as it has 62% of them as Annual Members .**

**Annual Members ride more during weekdays and  most active in the morning around 6:00 AM to 9:00 AM and early evening around 3:00 PM to 5:00 PM**

**which could indicate they use it to go to work in the morning and back home in the evening .**

**Casual riders tend to take more rides during weekends(Saturday and Sunday ).**

**and mostly start their rides after 12:00pm and after 07:00pm untill 09:00 pm.**

**Both Annual Members and Casual Riders are most active in the summer**

**Most active months for Casual and Member riders are from June to September.**

**. Streeter Dr & Grand Ave stations are the most used stations by Cyclistic riders.**

**- Casual riders ride for a longer time period with an average ride duration of 47.58 minutes.**

**Members have a shorter average ride duration of 15.14 minutes.**


 **Recommendations**

**Marketing recommendations to convert casual riders into members:**

**Enhance user experience by improving bike availability and maintenance.**

**Start promotions at the top stations and focus interaction efforts during peak times of the day.**

 **Marketing effort targeting the top 10 most popular stations for riders could include posts on social media,**
 
**print media displayed on bikes or at locking stations, and contests starting from the most popular station.**
 
 **Offer promotional memberships during the summer months and weekends.**
 
 **An incentive system to encourage more trips within a membership framework**
 
**in order to receive discounts and partnership offers.**

**Implementing targeted social media ads towards individuals who have previously utilized bike-sharing services and** 

**have expressed  interest in travel, outdoor sports, parks, museums.**

*******************************************************








